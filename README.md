# MyT IoT Platform

This program will allow the user to deploy a number of services onto a vm on AWS, Azure, GCP, Openstack etc. That will allow the user to graph data. This is aimed mostly for Sensor data. Docker will be used on the machine for each of the services installed on the machine.  

Services:
1. Database
2. MQTT broker
3. Graphing Techology(Grafana)
4. Data processing section user can customize.


The aim of this application that will allow the user press one button have all of their infrastructure deployed. Simply point the application at the vm or cloud platform of choice, and your infrastructure will be there and it will be reliable and secure.

## Requirements

1. Ansible roles and docker-compose files to install and configure services on a machine.
2. Application for use to deploy/manage IoT stack Desktop(Python/wxPython).
3. Docker compose files to manage containers.
4. Terraform code to create new infrastructure.

#### Ansible Roles
These will cover the management side of the deployment. The user will point at a resouces in the cloud and ansible will install the required packages on the machine. At the moment it is just the docker install, as well as other server config 

#### Docker files
The docker-compose file will spin up all of the required services and host them in their own containers. 

#### Python Destop Application
This application will allow the user to configure the infrastructre, select cloud platform, services required, passwords, credentials etc. 

This will also be a management console for the user. 

This will need to be backed up by a web backend to handle user support.

#### Terraform
Terraform will be used for users who don't know how to spin up their own infrastructe. This will automatically spin up infrastructure on the users selected cloud platform. Also configre the security groups etc. It will automatically gather the information for the ansible roles to install the required pacakges.


## To Do list

- [x] Ansible Playbook to Deploy Docker.
- [ ] Docker files to install/Configure services.
- [ ] Application to deploy stack.
- [ ] Terraform code to spin up infrastructure (Openstack).
- [ ] Imporve Application.
	- [ ] User Support. 
	- [ ] More service deployment options/customization.
	- [ ] Management pannel.
- [ ] Terraform support for AWS, Azure and GCP (At least 2).


 
