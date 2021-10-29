# Prueba_git
Prueba de las funciones principales de GIT

#Primero 
Descargar el Git bash para utilizar en la terminal (CMD, Terminal)

Link http://msysgit.github.io/

#Segundo
Crear un nuevo repositorio de forma local
git init

-Si ya cuenta con un repositorio en GitHub, lo que se debe hacer es lo siguiente:
    #para crear una copia local del repositorio 
  1- git clone https://github.com/rortizs/Prueba_git.git

  #servidor remoto
  2- git clone username@host:/path/para/repositorio

  #flujo de trabajo
  Tu repositorio local esta compuesto por tres árboles administrador por git.
  El Primero es tu Directorio de Trabajo, el cuál contiene los archivos.
  El Segundo es el INdex que acuta como una zona intermedia. 
  El Tercero es el HEAD que apunta al último commit realizado.

  #add & commit
  --Si solo vamos a agregar un solo archivo se usa el comando
  git add <filename>

  --si vamos a agregar todos los archivos se usa el comando'
  git add .

  #commit
  para subir el flujo de trabajo vamos a hacer commit a estos cambios.

  git commit -m "Mensaje para indentificar ese commit"

  #Agregar al repositorio remoto
  git remote add origin https://github.com/Prueba_git2.git

  #ramas
  ---------> master 
     -->rama2 (user3)
       -->rama3 (user2)

#que comando se usar para las ramas
Crear una nueva rama 
git chekout -b rama2

Borrar la rama
git branch -d rama2

Para volver a la rama principal
git checkout master

#Actualizar o Fusionar
para actualizar el repositorio local al commit 
git pull

#fusionar la rama activa con la rama master
git merge master

#agregar los archivos que se van a fusionar
git add .

#antes de fusionar vamos a revisar los cambios

git diff master rama2