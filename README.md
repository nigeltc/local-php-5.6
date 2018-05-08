# local-php-5.6 - Docker local development environment for PHP 5.6

This is a skeleton for a web project using PHP 5.6 on a Debian Jesse base. I use it as an alternative to installing XAMPP or LAMPP on my development box. It also lets me specify the version of PHP I use which can be closer to the target environment.

The layout is very simple:

        * docker
	      * Dockerfile
    	* docker-compose.yml
    	* LICENSE
    	* README.md
    	* www
    	  * index.php

The ```www``` directory gets mapped to ```/var/www/html``` so you can edit files locally and they are automatically available to the web server running in the container.

To run the container:

        $ sudo docker-compose up -d

To stop the container:

        $ sudo docker-compose stop

