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

## 4. Comprueba que ip tiene y si puedes hacer un ping a google.com
Dentro del contenedor 'dam_ubu1', instalas las herramientas necesarias:

- apt update
- apt install net-tools
- apt install iputils-ping

Miramos nuestra ip con `ifconfig`

Y ahora para hacer ping usaremos el comando `ping google.com`, de esta manera hacemos ping con google, para parar el ping le daremos al Ctrl + C

## 5. Crea un contenedor con el nombre 'dam_ubu2'. ¿Puedes hacer ping entre los contenedores?

1. Crear un contenedor 'dam_ubu2':
<br>
Ejecuta este comando en la terminal de Docker para crear el segundo contenedor:

- docker run -di --name dam_ubu2 ubuntu 

2. Hacer ping entre los contenedores: <br>
Encuentra la dirección IP del contenedor 'dam_ubu2' utilizando un método similar al utilizado previamente. Una vez tengas esa dirección IP, desde el contenedor 'dam_ubu1', intenta hacer ping al 'dam_ubu2' utilizando su dirección IP. Esto te permitirá confirmar si hay conectividad entre los contenedores.
