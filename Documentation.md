
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

