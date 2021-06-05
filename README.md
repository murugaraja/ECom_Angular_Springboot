### RESTful services (Spring boot)
#### API build for an E-Commerce Application, provides below services for Admin & Customer CRUD operations and also handles authenticted user sessions 
docker run --detach --name=mysql --env="MYSQL_ROOT_PASSWORD=my_password" --publish 3306:3306 --volume=/root/docker/mysql/conf.d:/etc/mysql/conf.d --volume=/storage/docker/mysql-data:/var/lib/mysql mysql
mysql -uroot -p my_password

create database webservice;
use webservice;

Run Active MQ
docker run -p 61616:61616 -p 8161:8161 rmohr/activemq

Register user in UI and activate them using below query
update User set is_enabled=0x01;

give permision in Authorities table
insert into Authorities (authority, username) values ('ROLE_ADMIN','a@a.com');
insert into Authorities (authority, username) values ('ROLE_USER','b@b.com');
