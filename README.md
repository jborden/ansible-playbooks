# Introduction

This is a set of [Ansible](https://github.com/ansible/ansible) tasks to compose a playbook for initializing a server with nginx to host a Java WAR file.

The architecture is composed of multiple docker containers that are linked and managed via docker-compose. The architecture is as follows:

nginx   - HTTP proxy
certbot - for HTTPS
$name   - container which hosts the Clojure Web App

# Initialization of Digital Ocean host

1. If you've changed servers (e.g. deleted and created a new one) you will need to delete current entry from ~/.ssh/known_hosts


