# ELK-Docker
This is a repo of the ELK (Elasticsearch, Logstash, Kibana) stack that was made for Docker and run via Docker compose.

## Disclaimer:
This is **not a production level** ELK stack instance, **security is disabled** in the elasticsearch container and therefore would make this **unsafe** to use in a production environment.

## Purpose:
This was made so the ELK stack could be spun up in a quick manner to allow for learning purposes. Such learning includes dashboards, visualizations, exploring the discovery tab and working with logs in general.


## Example Environment:
- Download VirtualBox
- Create a NAT Network, example ELK-stack
- Create a machine for the docker containers to run on, have the network be the created network
- Create a machine that will deliver logs via Filebeat, have the network be the created network
- Install/Configure Filebeat on the machine that will send the logs
- Start webservers (apache2, nginx) on the machine that will sends logs

## To Run
- Place all files in a directory
- Install Docker on the machine you want the containers to be ran on
- Run ` docker compose up ` on the command line in the project directory
