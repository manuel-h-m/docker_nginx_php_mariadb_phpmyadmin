# Nginx + PHP + MariaDB + PhpMyAdmin docker-compose file.
Docker-compose file with Nginx, PHP, MaríaDB and PhpMyAdmin ready to use as local development environment.

## Getting Started
### Prerequisites
You only need Docker and docker-compose installed.

### Instalation
Just download the proyect and you will have a directory with the docker-compose file ready to raise the environment.

## Using docker_lnmp
To raise the environment, run:

$ docker-compose up

Then you will have de followin URL available:

* [http://localhost](http://localhost)  (your awsome web app)
* [http://localhost:8080](http://localhost:8080)  (phpmyadmin)

The proyect has this directory and file structure:

<pre>
./README.md                           (this file)
./docker-compose.yml
./lnmp
  ├ conf                              (nginx virtualhost configuration file)
  └ mariadb                           (mariadb data files, persistence)
./src
  ├ html                              (document-root)
  |  └ index.php                      (change with your own web app files)
  └ your-out-of-document-root-files   (projects may need files out of the document-root, i.e. config files)
</pre>

