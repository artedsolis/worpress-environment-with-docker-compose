# A WordPress environment 
## with docker-compose
![](https://github.com/artedsolis/docker-compose-for-worpress-environement/blob/master/docker-compose-wp.png "docker-compose and wordpress logos")


## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)

## General info
This repository mainly hosts a sample of .yaml file for running docker-compose with WordPress.

Once docker-compose command line runned, WordPress image will pull its file structure.

Finally, you will be able to start running WordPress and phpmyadmin on localhost.
	
## Technologies
Project is created with:
* mysql:5.7
* phpmyadmin
* WordPress: latest version
* Run on: Linux ubuntu 20.04
	
## Setup
1. Clone this repo:

**$ git clone https://github.com/artedsolis/worpress-environement-with-docker-compose.git**

2. go inside the repo with:

**$ cd [name_of_the repo]**

3. type de following command on your terminal:

**$ docker-compose up -d**

**Note**: 
- __this WordPress image uses apache, so that's why volumes are as following__ _volumes: ['./:/var/www/html/']_
- __the image will link WordPress files into your repo's folder__        

4. finally go to your: 
http://localhost:8000
&
http://localhost:8080

5. you're donne for installation!

6. to stop docker-compose for runnig type:

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
