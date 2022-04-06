# docker01
Aula 01



docker build -t mysql-image -f services\db\DockerFile .

### Inicia 
docker run -d --rm --name mysql-container mysql-image

### Roda Script sql
docker exec -i mysql-container mysql -uroot -pimpacta < services/db/script.sql


### Acessa o Container
docker exec -it mysql-container /bin/bash

### Acessar o Mysql
mysql -uroot -pimpacta


### MYSQL
show databases;<br/>
use IMPACTA_DATABASE;<br/>
show tables;<br/>
SELECT * FROM CLIENTE;
