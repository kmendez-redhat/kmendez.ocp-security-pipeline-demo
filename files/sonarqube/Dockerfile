FROM docker.io/sonarqube:latest
RUN sed -i 's/chown -R sonarqube:sonarqube $SONARQUBE_HOME//' $SONARQUBE_HOME/bin/run.sh
RUN usermod sonarqube -aG 0
RUN wget https://github.com/SonarQubeCommunity/sonar-build-breaker/releases/download/2.2/sonar-build-breaker-plugin-2.2.jar -O /opt/sonarqube/lib/bundled-plugins/sonar-build-breaker-plugin-2.2.jar
RUN chgrp -R 0 /opt/sonarqube && chmod -R 770 /opt/sonarqube 
