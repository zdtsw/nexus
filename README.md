# nexus
Nexus + Ansible

A repo for install nexus (version no earlier than 3.1.0) and upgrade
This is only for version after 3.0.2 since, from 3.0.2 to later version Nexus structure has been changed and also $karaf is replaced by $jetty in some cases


Default port 8081
Customer ssl port 8443
Change port number in roles/nexus/files/nexus.properties

if you have customer cert files, update the path in roles/tasks/main.yml

if you do not need ssl, remove jetty-https.xml from roles/nexus/files/nexus.properties
