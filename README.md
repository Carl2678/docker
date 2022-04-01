# docker
Dans le cadre du cours de virtualisation à l’Université Episcopal d’Haïti (UNEPH) on nous a
demandé d’installer Lamp (Linux, Apache, MySql et PHP) sur un environnement Docker et de
développer une application web dans cet environnement.
Voici les étapes que nous utilisons pour réaliser ce projet.
1- Création d’un répertoire de projet ~/docker/lamp (disons) et un répertoire html/ dans le
répertoire du projet pour conserver les fichiers du site Web (c'est-à-dire php, html, css, js,
etc.) comme suit :
$ mkdir -p ~/docker/lamp/html
Accédons au répertoire du projet ~/docker/lamp comme suit :
$ cd ~/docker/lamp
Créons un fichier php.Docker dans le répertoire du projet ~/docker/lamp. Il s'agit d'un
Dockerfile qui active les extensions mysqli et PDO php dans l'image php:7.4.3-apache de Docker
Nous avons créé 3 services web-server, mysql-server et phpmyadmin.
Nous Créons également un fichier index.php dans le répertoire html/ pour tester le serveur LAMP
Maintenant, pour démarrer les services web-server, mysql-server et phpmyadmin, exécutons la
commande suivante :
$ docker-compose up -d
7
Nous pouvons accéder à phpMyAdmin 5 et au serveur Web à partir d'un navigateur Web.
Pour accéder à phpMyAdmin 5, ouvrons un navigateur Web et visitons http://localhost:5000

Réalisation de l’application web
1- Création du répertoire de l’application
$ mkdir -p monprojet
Création du fichier docker-compose.yaml
Pour notre application web on a utilisé le CMS joomla et nous avons installer sur
l’environnement docker, en utilisant le fichier docker-compose.yaml
Installons le CMS joomla en utilisant la commande :
$ docker-compose up -d
