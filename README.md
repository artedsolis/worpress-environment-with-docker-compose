# docker-compose-for-worpress
## a WordPress environement
![](https://github.com/artedsolis/docker-compose-for-worpress-environement/blob/master/docker-compose-wp.png "docker-compose and wordpress logos")


## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)

## General info
This repository mainly hosts a sample of .yaml file for running docker-compose with WordPress.

Once docker-compose command line runned, it will start a WordPress with its file structure and pesistent mysql.

Finally, you will be able to start running WordPress and phpmyadmin on localhost.
	
## Technologies
Project is created with:
* mysql:5.7
* phpmyadmin
* WordPress: latest version
* Run on: Linux ubuntu 20.04
	
## Setup
To run this project, install it locally using docker-compose CLI:

1. **$ docker-compose up -d**

2. then go to: 
http://localhost:8000
&
http://localhost:8080

to stop docker-compose run:

**$ docker-compose down**

then, if you want to unmount your volume:

**$ docker-compose down --volume** 

## Child Theme
A way to use a WordPress child theme, once you've runned **docker-compose up -d**.
You have to unzip the parent theme + child theme into wp-content>themes folder (sure you have to deal with some permissions first)

## Resources
* [How to change directory permissions in Linux](https://www.pluralsight.com/blog/it-ops/linux-file-permissions)
* [Quickstart: Compose and WordPress](https://docs.docker.com/compose/wordpress/)
* [Child Themes](https://developer.wordpress.org/themes/advanced-topics/child-themes/)
