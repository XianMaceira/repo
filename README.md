# Practica Git

# Creacion de repo
Creamos e configuramos un repositorio.

# Ej1
Configurar Git definiendo el nombre del usuario, el correo electrónico y activar el coloreado de la salida. Mostrar la configuración final.

# Ej2
Crear un repositorio nuevo con el nombre libro y mostrar su contenido.

# Ej3
Comprobar el estado del repositorio.

Crear un fichero indice.txt con el siguiente contenido:

# Ej4
Realizar un commit de los últimos cambios con el mensaje “Añadido índice del libro.” y ver el estado del repositorio.

# Ej5
Cambiar el fichero indice.txt para que contenga lo siguiente:

Mostrar los cambios con respecto a la última versión guardada en el repositorio.

Hacer un commit de los cambios con el mensaje “Añadido capítulo 3 sobre gestión de ramas”.

# Ej6
Mostrar los cambios de la última versión del repositorio con respecto a la anterior.
Cambiar el mensaje del último commit por “Añadido capítulo 3 sobre gestión de ramas al índice.”
Volver a mostrar los últimos cambios del repositorio.

# COMANDOS

# Configuracion

git config --global user.name "Your-Full-Name"

git config --global user.email "your-email-address"

git config --global color.ui auto

git config --list


# Creacion
git init --> Iniciar repo

ls -la / ls -h

git status

git add

git commit -m "Texto ejemplo"

git commit --amend -m "Texto ejemplo" --> Modifica el commit

git log 

git show --> Muestra la diferencia de contenido entre los commit

git diff --> Muestra las diferencias

