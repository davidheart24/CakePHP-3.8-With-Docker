# CakePHP 3.8 with docker
## Overview
Build this repo's docker environment on local to try the [official tutorial](https://book.cakephp.org/3.0/en/tutorials-and-examples.html).

* Apache 2.4.10
* php 7.1.5
* CakePHP 3.8.*
* MySQL 5.6.36 


## How to build
* Build docker containers and start a CakePHP project

Clone this repo<br>
`$ git clone https://github.com/davidheart24/CakePHP-3.8-With-Docker.git`

Go in the folder and launch <br>
`$ docker-compose up --build -d`

Check the docker containers if created succcessfully<br>
$ docker container ps or docker ps<br>

Result👁

```
ebd4e52fa6bf        phpmyadmin/phpmyadmin   "/docker-entrypoint.…"   8 seconds ago   Up 8 seconds   0.0.0.0:8094->80/tcp   david_phpmyadmin_1
2a032a64b8c6        devstage2_cakephp       "docker-php-entrypoi…"   8 seconds ago   Up 8 seconds   0.0.0.0:4000->80/tcp   david_cakephp_1
3a5b3e14efb7        mysql:5.6.36            "docker-entrypoint.s…"   8 seconds ago   Up 8 seconds   306/tcp                david_mysql_1
```

Then visit http://localhost:4000 to see the welcome page.