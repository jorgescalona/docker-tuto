### Sistematización del aprendizaje de docker

Ante todo es importante diferenciar entre contenedor, imagen e instancias de contenedores, cada uno
de ellos usa un ID distinto.

# Listar imagenes

> $docker images

# Listar contenedores

> $docker ps 
\neste lista los que esten en ejecución
> $docker ps -a
lista todos los contenedores en el equipo

# Eliminar Contenedores

> $docker rm IDcontenedor

# Eliminar imagen

> $docker rmi IDimage

# attachar un contenedor

> $docker attach IDcontainer

# Ejecutar imagen abrir seudo tty 

> docker run -t -i imagen /bin/bash

Enlaces de interes y que use para aprender sobre docker
=======================================================

* [http://www.cristalab.com/tutoriales/instalacion-y-primeros-pasos-en-docker-c114081l/](http://www.cristalab.com/tutoriales/instalacion-y-primeros-pasos-en-docker-c114081l/)


