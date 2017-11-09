# elmsln-docker
Converting the ELMSLN project to utilize containers.

ELMSLN Project site: https://www.elmsln.org/
ELMSLN Git Repo: https://github.com/elmsln/elmsln

ELMSLN comprises of 3 primary components:
	Apache
	PHP-FPM
	MariaDB

The Base OS that these containers will run on will be CentOS Atomic Host SIG.  

Primary Application containers:
  ** Apache -> https://hub.docker.com/_/httpd/
	httpd:2.4-alpine

  ** PHP -> https://hub.docker.com/_/php/
	php:7.1-fpm-alpine

  ** MariaDB -> https://hub.docker.com/_/mariadb/
	mariadb:10.2
Persistant Storage Containers:
  ** Database

  ** Application Code

Build Out Plan:
Phase 1: 
  * Getting all Docker containers to build and configured for ELMSLN

Phase 2:
  * Creation and modification of scripts for automated build and deployment

Phase 3:
  * Integration with Kubernetes
