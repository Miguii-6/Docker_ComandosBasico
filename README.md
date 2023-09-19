# Docker Comandos Básicos

## 1. Descargamos a imagen "ubuntu" co siguiente comando:

Con este comando procederemos a descargar la imagen si no estaba localmente descargada.
- docker run ubuntu

Y con este otro comando comprobaremos si de verdad esta descargada.

- docker image ls -a

## 2. Crea un contenedor sin ponerle nombre y ver si funciona:
Con este comanddo crearemos el contenedor:

- docker run ubuntu

Ahora usaremos este comando para saber si de verdad esta creado

- docker ps -a

Co resultado da terminal de:

|Contairner ID|Image|Command|Created|Status|Ports| Names |
|-------|-------|-------|-------|-------|-------|-------|
|2e425d732bbc|ubuntu|"/bin/bash"|6 minutes ago|Exited (0) 5 minutes ago| |  determined_goldberg|

