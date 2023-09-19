# Docker Comandos Básicos

<br>

## 1. Descargamos a imagen "ubuntu" co siguiente comando:

Con este comando procederemos a descargar la imagen si no estaba localmente descargada.
- docker run ubuntu

Y con este otro comando comprobaremos si de verdad esta descargada.

- docker image ls -a

<br>

## 2. Crea un contenedor sin ponerle nombre y ver si funciona:
Con este comando crearemos el contenedor:

- docker run ubuntu

Ahora usaremos este comando para saber si de verdad esta creado

- docker ps -a

Co resultado da terminal de:

|Contairner ID|Image|Command|Created|Status|Ports| Names |
|-------|-------|-------|-------|-------|-------|-------|
|2e425d732bbc|ubuntu|"/bin/bash"|6 minutes ago|Exited (0) 5 minutes ago| |  determined_goldberg|

<br>

## 3. Crea un contenedor con el nombre 'dam_ubu1 y lo compruebo:

Con el siguiente comando crearemos el contenedor y le pondremos el nombre:

- docker run -it --name dam_ubu1 ubuntu

Y para comprobar si se creó se usa:

- docker ps -a

|Contairner ID|Image|Command|Created|Status|Ports| Names |
|-------|-------|-------|-------|-------|-------|-------|
|3ffb933c4095|ubuntu|"/bin/bash"|2 minutes ago| Exited (0) About a minute ago| |dam_ubu1|

