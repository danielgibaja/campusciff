# campusciff

# 2.1 REPOSITORIO CAMPUSCIFF (I) #
## 1. Crear un repositorio en vuestro GitHub llamado campusciff ##



# 2.2 REPOSITORIO CAMPUSCIFF (II) #
## 1. Clonar vuestro repositorio en local ##

##### $git clone git@github.com:danielgibaja/campusciff.git



# 2.3 README #
## 1. Crear (si no lo habéis creado ya) en vuestro repositorio local un documento README.md ##

##### $git add README.md ###



# 2.4 COMMIT INICIAL #
## 1. Añadir al README.md los comandos utilizados hasta ahora y hacer un commit inicial con el mensaje "commit inicial" ##

##### $git commit README.md -m "commit inicial" ###



# 2.5 PUSH INICIAL #
## 1. Subir los cambios al repositorio remoto ##

##### $git push origin master ###



# 2.6 IGNORAR ARCHIVOS (I) #
## 1. Crear en el repositorio local un fichero llamado privado.txt ##

##### $touch privado.txt

## 2. Crear en el repositorio local una carpeta llamada privada ##

##### $mkdir privada



# 2.7 IGNORAR ARCHIVOS (II) #
## 1. Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git ##

##### $echo privado.txt > .gitignore
##### $echo privada/ >> .gitignore
##### $git add .
##### $git commit -m "commit con archivos ignorados"



# 2.8 AÑADIR FICHERO 1.TXT #
## 1. Añadir fichero 1.txt al repositorio local ##

##### $echo 1 > 1.txt



# 2.9 CREAR EL TAG V0.1 #
## 1. Crear un tag v0.1 ##

##### $git tag v0.1



# 2.10 SUBIR EL TAG V0.1 #
## 1. Subir los cambios al repositorio remoto ##

####  $git add 1.txt
####  $git commit -m "tag v0.1"
####  $git push --tag origin master



# 2.11 CREAR UNA RAMA V0.2 #
## 1. Crear una rama v0.2 ##

####  $git checkout -b v0.2

## 2. Posiciona tu carpeta de trabajo en esta rama ##

####  (Ya había posicionado la carpeta de trabajo en esa rama al mismo tiempo que la creé)



# 2.12 AÑADIR FICHERO2.TXT #
## 1. Añadir un fichero2.txt en la rama v0.2 ##

####  $echo 2 > 2.txt
####  $git add 2.txt
####  $git commit -m "fichero 2.txt en v0.2"



# 2.13 CREAR RAMA REMOTA V0.2 #
## 1. Subir los cambios al reposiorio remoto ##

####  $git push origin v0.2



# 2.14 MERGE DIRECTO #
##  1. Posicionarse en la rama master ##

####  $git checkout master

##  2. Hacer un merge de la rama v0.2 en la rama master ##

####  $git merge v0.2



# 2.15 MERGE CON CONFLICTO (I) #
##  1. En la rama master poner Hola en el fichero1.txt y hacer commit ##

####  $echo Hola >> 1.txt
####  $git add .
####  $git commit -m "Hola>>1.txt"



# 2.16 MERGE CON CONFLICTO (II) #
##  1. Posicionarse en la rama v0.2 y poner Adios en el fichero "1.txt" y hacer commit ##

####  $git checkout v0.2
####  $echo Adios >> 1.txt
####  $git add .
####  $git commit -m "Adios>>1.txt"



# 2.17 MERGE CON CONFLICTO (III) #
##  1. Posicionarse de nuevo en la rama master y hacer un merge con la rama v0.2 ##

####  $git checkout master
####  $git merge v0.2 -m "merge con rama v0.2: conflicto"
####  (No se puede: Automatic merge failed; fix conflicts and then commit the result)



# 2.18 LISTADO DE RAMAS #
##  1. Listar las ramas con merge y las ramas sin merge ##

####  $git branch --merged
####  (master)
####  $git branch --no-merged
####  (v0.2)



# 2.19 ARREGLAR CONFLICTO #
##  1. Arreglar el conflicto anterior y hacer un commit ##

####  $echo 1 > 1.txt
####  $echo Hola >> 1.txt
####  $git add .
####  $git commit -m "conflicto resuelto"



# 2.20 BORRAR RAMA #
##  1. Crear un tag v0.2 ##

####  $git tag v0.2

##  2. Borrar la rama v0.2 ##

####  $git branch -d v0.2



# 2.21 LISTADO DE CAMBIOS #
##  1. Listar los distintos commits con sus ramas y sus tags ##

####  $git log



# 2.22 CUENTA DE GITHUB #
##  1. Poner una foto en vuestro perfil de GitHub ##

##  2. Poner el doble factor de autentificación en vuestra cuenta de GitHub ##

##  3. Añadir (si no lo habéis hecho ya) la clave pública que se corresponde a tu ordenador ##



# 2.23 USO SOCIAL DE GITHUB #
##  1. Preguntar los nombres de usuario de GitHub de tus compañeros de clase, búscalos, y sigueles ##

##  2. Seguir los repositorios campusciff del resto de tus compañeros ##

##  3. Añadir una estrella a los repositorios campusciff del resto de tus compañeros ##



# 2.24 CREAR UNA TABLA #
##  1. Crear una tabla en el fichero README.md con la información de varios de tus compañeros de clase ##

|   NOMBRE    | APELLIDO |               GITHUB               |
| ----------- | -------- | ---------------------------------: |
|  Alejandro  |  Diaz    |   https://github.com/adiazgalache  |
|  Carlos     |  Paz     |   https://github.com/cpazsantos    |
|  Amalia     |  Suárez  |   https://github.com/asuarezg      |



# 2.25 COLABORADORES #
##  1. Poner a github.com/asanzdiego como colaborador del repositorio campusciff ##



# 2.26 CREAR UNA ORGANIZACIÓN #
##  1. Crear una organización llamada campusciffdanielgibaja ##



# 2.27 CREAR EQUIPOS #
##  1. Crear 2 equipos en la organización campusciffdanielgibaja, ##
##     uno llamado administradores con más permisos y otro colaboradores con menos permisos ##

##  2. Meter a y a 2 de vuestros compañeros de clase en el equipo administradores ##

##  3. Meter a y a otros 2 de vuestros compañeros de clase en el equipo colaboradores ##
