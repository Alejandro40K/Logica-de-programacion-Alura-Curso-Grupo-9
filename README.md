# Logica-de-programacion-Alura-Curso-Grupo-9
Una guía básica inicial para quien desea entrar en el universo de programación y comenzar con la creación de páginas web utilizando los lenguajes populares de HTML, CSS y JavaScript

# Para rstaurar otros commits anteriores 

Si queremos volver a un commit antiguo, podemos usar , primero usamos git log -oneline para ver el historial de comits, luego copeamos el codigo y el nombre del archivo de la siguente forma:

$ git restore --source 9a876e5 -- index.html

# Para crear otra rama

En GitHub puedes crear varias ramas, de desarrollo, pruebas etc. Para crear una nueva rama se hace lo siguente

$ git checkout -b 'desarrollo'

Para cambiar de rama se hace lo siguente:
$ git switch desarrollo

Para empujar o subir los cambios al repositorio remoto lo que hacemos  es lo siguente:
$ git status 
$ git add .
$ git commit -m "Actualizacion"
$ git push origin desarrollo 

# Para mezclar dos ramas 

Cambiamos a rama principal 
$ git switch main 
Usamos el comando merge
$ git merge desarrollo 
$ git log --oneline 
$ git push origin main

# Configurar 

git cofig --global user.name "[name]"
git config --global user.email [email]
git config --list 

# Crear repositorio 

git clone [url]
git init 

# Verificaciones 

git status -> estado de los commits 
git log -> historial de los commits
git diff -> cambios en los archivos
git branch -> ver ramas 

# Agregar 

git add .
git add [archivo]

# Mover

git commit -m "[Mensaje ]"

# Enviar o actualizr

git push 

# Bajar actualizaciones 

git pull

# Cambiar 

git checkout -b [branch-name]
git merge 
git switch 
git restore --source [hash] [archivo]

