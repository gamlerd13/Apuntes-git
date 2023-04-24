# APUNTES PARA GIT

---

> Comandos basicos de git

- git init
- git add :Esto es para agregar al area de trabajo
- git status :Para ver el estado de nuestos archivos
- git commit
- git push
- git pull
- git clone

---

### Para configurar los usuarios locales

> git config --global user.email "gamlerd13@gmail.com"

> git config ---global user.name "gamlerd13"

Par ver que usuario tenemos en local: git config user.name
lo mismo para ver el email

---

### Para mostrar todos lo commits git log

> git log : para mostrar los commits, la hora de creacion y el autor.

> git log --pretty=oneline --abbrev-commit : Para ver todos los commits resumidos, mejor visualizacion.

> git log --stat : Esto hace que muestra los commits completos y se agrega el numero total de archivos y lineas modificadas.

> git log -p // git log --patch : Muestra los cambios que hemos realizado, no se usa mucho i think

## Para mostrar los commimt con autor especifico

> git log --author="gamlerd13"

---

## git commit:

> git commit :Aqui se podemos guardar los commit pero se abrirá un editor de texto para poner los mensajes del commit

Para guardar el commit sin entrar el editor nano i vin:

> git commit -m "mensaje del commit"

Para editar el ultimo commit

> git commmit --amend :editar desde nano o vim

> git commmit --amend -m "Este commit fue editado" :editar desde terminal

## Para volver al ultimo commit sin haber commiteado a los archivos que estamos guardando con [ctrl + s] en el editor.

> git checkout -- nombreArchivo.html :Si modificas tu archivo sin haber hecho commit, este codigo lo que hará es volver al
> ultimo commit del archivo.

> git checkout . :Este regresa a todos los archivos modificado sin commit al ultimo commit hecho

## Para poder ver las diferencias de los cambios hechos en un archivo o en todos los archivos

> git diff archivos.html :Este me muestra lo que he cambiado en el archivo, it's important 'cause show us before and after

> git diff . :I think show us the all changes modified for us

## Para ignorar archivos y carpetas

Aqui solo hace falta crear un archivo .gitignore y dentro escribir en cada fila la carpeta
o el nombre del archivo que no deseas hacer commit. me deja hacer commits ilimitados creo xd

## Ramas

### Para ver lista de ramas y en que rama estamos

> git branch

### para crer una nueva rama

> git branch nombreRama :ejmplo: git branch version-1.0

### para cambiar de rama

> git checkout nombreRama : ejemplo: git checkout main
