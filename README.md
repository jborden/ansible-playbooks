# Introduction

This is a set of (Ansible)[https://github.com/ansible/ansible] tasks to compose a playbook for initializing a server with nginx to host a Java WAR service. In particular, for hosting Clojure Web Apps compiled into a WAR file.

The architecture is composed of multiple docker containers that are linked and managed via docker-compose. The architecture is as follows:

nginx   - HTTP proxy
certbot - for HTTPS
$name   - container which hosts the Clojure Web App

# Notes

https://stackoverflow.com/questions/43609132/ansible-how-to-call-a-playbook-from-another
