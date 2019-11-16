# Linux server configuration
This app and the server have been setup as projects for [Udacity Full Stack Developer Nanodegree Program](https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd0044)

## Table of Contents
- [Server Details](#server-details)
- [Softwares Installed](#softwares-installed)
- [Configurations Made](#configurations-made)
- [Resources](#resources)

### Server Details
* IP-address: `52.59.208.241`
* URL: `http://udacity.schinina.eu/`
* SSH port: `2200`
* Server hosted by [Amazon Lightsail](https://lightsail.aws.amazon.com/)

### Softwares Installed
* Apache2 and wsgi module
* Postgres

### Configurations Made
* Updated all currently installed packages
* Changed the SSH port from 22 to 2200
* Configured the UFW to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
* Created a new user, `grader`, given sudo permissions, configured SSH authorisation access
* Configured the local timezone to UTC
* Installed and configured Apache to serve a Python mod_wsgi application
* Installed and configured PostgreSQL:
	* Created a new database user named catalog that has limited permissions to my catalog application database


### Resources
* [Udacity Full Stack Developer Nanodegree Program](https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd0044)
* [Ubuntu documentation - Sudoers](https://help.ubuntu.com/community/Sudoers)
* [DigitalOcean - How To Install and Use PostgreSQL on Ubuntu 18.04](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04)
* [Linode - How to Configure a Firewall with UFW](https://www.linode.com/docs/security/firewalls/configure-firewall-with-ufw/)
* [Flask documentation - mod_wsgi (Apache)](https://flask.palletsprojects.com/en/1.1.x/deploying/mod_wsgi/)
