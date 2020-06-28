This package enables you to access php-7.2 apache2 and nodejs latest servers in
2 different containers.

i. install docker

* check your linux os distro and version

$ lsb_release -a

if ubuntu

https://docs.docker.com/engine/install/ubuntu/

else if debian

https://docs.docker.com/engine/install/debian/



ii. install docker-composer

https://docs.docker.com/compose/install/  follow linux steps



iii. clone this package into your machine

$ git clone https://github.com/Flutter-Stack/docker-compose-node-php-services.git


$ cd docker-compose-node-php-services


iv. Run below command to create the services

$ docker-compose up -d

You can see runing container using

$ docker ps






## node-backend:  ##

you can access nodejs at http://0.0.0.0:8082/

remove files inside project-code with your project code.

replace command: npm start dev   if required.

you can verify log of node-backend container

$ docker logs node-backend

login to node-backend contianer

$ docker exec -it node-backend /bin/bash





## php-backend: ##


you can access nodejs at http://0.0.0.0/test.php

remove files inside www with your project code.


you can verify log of php-backend container

$ docker logs php-backend

login to php-backend contianer

$ docker exec -it php-backend /bin/bash
