
1-¿Que version tiene instalada?
docker --version

2-Crear una imagen
Docker hub

3-¿Como ver que imagenes tengo creadas?
docker images

4-¿Como borrar imagenes?
docker rmi hello-world  'Se borra por id o por nombre de la imagen'


¿Como crear una imagen?
+Ingresar en docker hub
+Buscar la imagen 'Para este caso el hellow world'
+Copiar docker pull hello-world

¿Como crear contenedor con nombre personalizado?
docker create --name contenedorMysql mysql


Salida:
C:\Users\Developer>docker pull hello-world
Using default tag: latest
latest: Pulling from library/hello-world
4f55086f7dd0: Pull complete
d5e71e642bf5: Download complete
Digest: sha256:c567b231f65614688711a75f31518a064258a51d442117a3e771a3a8fdba78ef
Status: Downloaded newer image for hello-world:latest
docker.io/library/hello-world:latest

+¿Como ver que contenedores tengo?
docker ps -a

+¿Como crear contenedores? SIN ARRANCAR
C:\Users\Developer>docker create hello-world
d0a66c1b733798cfc3d53f7ad06a835502e46b7723cd976b8275a06ffa06fa22


+Estados de los contenedores:
created → creado, nunca arrancado.
running → corriendo.
paused → pausado.
exited → terminó o se detuvo.
restarting → reiniciándose.
dead → error, no se pudo limpiar.

Administración de iamges 'Comandos'
--Listar iamgenes:
    docker images

--Buscar imagenes:
    docker search mysql 'mysql es solo busqueda'

C:\Users\Developer>docker search mysql
NAME                  DESCRIPTION                                     STARS     OFFICIAL
mysql                 MySQL is a widely used, open-source relation…   16195    [OK]


--Crear una imagen .net 'consultar la pagina de Microsoft'
mcr.microsoft.com/dotnet/aspnet:9.0

--Crear una imagen
docker pull mcr.microsoft.com/dotnet/aspnet:9.0

C:\Users\Developer>docker pull mcr.microsoft.com/dotnet/aspnet:9.0
9.0: Pulling from dotnet/aspnet
59a759afbd82: Pull complete
dd051e1b8c92: Pull complete
4db8edfb30f9: Pull complete
5a33d25ae2e7: Pull complete
4e85db303a63: Pull complete
d17f285ff202: Pull complete
Digest: sha256:c5d96442d3fc5b9a85380922a174692c8a9899bc1efa5d1bf5a540dcd2079f5c
Status: Downloaded newer image for mcr.microsoft.com/dotnet/aspnet:9.0
mcr.microsoft.com/dotnet/aspnet:9.0



C:\Users\Developer>docker pull mysql
Using default tag: latest
latest: Pulling from library/mysql
63751bcf6dad: Pull complete
335c0ba6129f: Pull complete
3594eab1df5f: Pull complete
c3e99775cc39: Pull complete
969334aca9fa: Pull complete
37fa2793f15f: Pull complete
781b429d34a1: Pull complete
3ba4d3770669: Pull complete
83d647c7d3d0: Pull complete
811578fcdc4f: Pull complete
24df5f010ba6: Download complete
891cff0835d5: Download complete
Digest: sha256:3819b2b23835c4a73c8b022fafc33c8095c0f81c929a8b7a84613d2fba6c52f5
Status: Downloaded newer image for mysql:latest
docker.io/library/mysql:latest

C:\Users\Developer>

¿Como saber si esta la ultima vr de esa imagen?
latest
