# Sistematización del aprendizaje de docker

Ante todo es importante diferenciar entre contenedor, imagen e instancias de contenedores, cada uno
de ellos usa un ID distinto.

### Listar imagenes

> $docker images

### Listar contenedores en ejecución

> $docker ps 

### Listar todos los contenedores

> $docker ps -a


### Eliminar Contenedores

> $docker rm IDcontenedor

### Eliminar imagen

> $docker rmi IDimage

### attachar un contenedor

> $docker attach IDcontainer

### Ejecutar imagen abrir seudo tty 

> docker run -t -i imagen /bin/bash


### Ejemplo para un entorno de desarrollo de odoo v9

lo primero es montar un contenedor de PostgreSQL con la opción -p q identificara el 
puerto del equipo huesped y seguido de ":", el puerto de conexión del contenedor de la bd 
>$docker run -p 5436:5432 -d -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo --name db postgres

>$docker run -p 8069:8069 -p 8022:22 --name odoo -v /local/datastore:/host/datastore --link db:db -t odoo

``


 


Enlaces de interes y que use para aprender sobre docker
=======================================================

* [Instalación y Primeros Pasos con Docker](http://www.cristalab.com/tutoriales/instalacion-y-primeros-pasos-en-docker-c114081l/)
* [Docker en debian x Ernesto Crespo](http://blog.crespo.org.ve/2015/12/uso-de-docker-en-debian-jessie-parte-1.html)


