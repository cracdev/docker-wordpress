# Docker - Wordpress 

## Setup

1. Download and setup [docker-compose for mac](https://store.docker.com/editions/community/docker-ce-desktop-mac)
2. The official [WordPress container](https://hub.docker.com/_/wordpress/) will clone it for you.
3. The official [mariadb image](https://hub.docker.com/_/mariadb/)
4. Run the docker-wordpress.sh script

## Getting Wordpress image

~~~bash
$ docker pull wordpress
~~~

## Getting mariadb image

~~~bash
$ docker pull mariadb 
~~~

## Run the docker-wordpress script

~~~bash
$ ./docker-wordpress.sh
~~~

## Run and Connect

Now you can create your containers and run them.

~~~bash
$ docker-compose up -d
~~~

If you want to see the output of the containers (to monitor for errors), follow their logs:

~~~bash
$ docker-compose logs -f
~~~

If you ever want to stop and restart your containers just run

~~~bash
$ docker-compose stop && docker-compose up -d
~~~

