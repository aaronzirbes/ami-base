# Base AMI Build

This project builds a base AMI for use in all other builds.
This AMI contains the following items:

* Ansible
* Java
* Consul
* Docker
* Userify Shim
* Userify Credentials from User Data Upstart
* Peoplenet Consul Configuration
* Stackdriver Agent & API Key
* Logstash default logging configuration

## Notes

This project declares it's own `image.json` file.
This is a copy of the default template in `packerw` but includes the installation of Ansible on the machine before executing the Ansible provisioner.
