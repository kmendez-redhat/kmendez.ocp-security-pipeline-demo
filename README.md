kmendez.ocp-security-pipeline-demo
=========

After provisioning the RHPDS OCP 3.9 cluster, logon to the bastion and run the following commands:

    sudo su -
    git clone https://github.com/kmendez-redhat/kmendez.ocp-security-pipeline-demo.git
    cd kmendez.ocp-security-pipeline-demo.git
    ansible-playbook config.yml

Passwords:

gogs: developer / Welcome1!

Jenkins: admin / password

Nexus: admin / admin123

SonarQube: admin / admin

Requirements
------------


Role Variables
--------------


Dependencies
------------


Example Playbook
----------------


    - hosts: master1
      include_role:
         name: kmendez.ocp-security-pipeline-demo

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
