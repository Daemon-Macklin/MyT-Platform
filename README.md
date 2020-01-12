# MyT IoT Platform

MyT is a cloud agnostic orchestration and management tool which allows users to design an IoT platform and then deploy it on a cloud service or server of their choice. Allowing the user to customize some aspects of their platform. For example different database solutions offer different features and are typically designed for different data. If a user has very structured data they will be more suitable for a relational database. On the other hand, if the user does not have structured data, or does not know what data they will be collecting they would be more suited to a NoSQL solution. This will provide an IoT platform that will suit the needs of the user. The MyT application will be a front end to manage the users platforms. Automating parts of maintaining your own IoT stack, allowing the user to focus on the rest of their IoT system.

## Services:
1. Database chosen by user
2. RabbitMQ messaging broker
3. Grafana data visualization
4. User defined data processing written in Python.

## Requirements

1. Terraform scripts to create new infrastructure.
2. Ansible playbooks configure a machine.
3. Docker compose files to create Docker containers for applications.
4. Application to deploy/manage IoT platforms.

## Git Repos

 1. [Deployment demo](https://github.com/Daemon-Macklin/MyTDeploymentDemo)
 2. [Data Processing Application](https://github.com/Daemon-Macklin/MyTPlatformDataProcessingContainer)
 3. [MyT Platform Docker Compose](https://github.com/Daemon-Macklin/MyTPlatformDataProcessingContainer/blob/master/docker-compose.yml)
