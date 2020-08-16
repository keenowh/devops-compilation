### Docker Postgres Database

Initialize mysql
    docker run -d --name <myName> -p 3306: 3306 -e MYSQL_ROOT_PASSWORD=root mysql

SSH into the container (Not really ssh equivalent)
    docker exec -it <myName> bash

To enter the command center (No space after p)
    mysql -u root -p<password>

Query if you anything you want
    docker run --name pg -p 5432:5432 -v /TargetDirectory:/var/lib/postgresql/data postgres