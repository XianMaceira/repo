# Practica Git 1

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
```bash
git config --global user.name "Your-Full-Name"
```
```bash
git config --global user.email "your-email-address"
```
```bash
git config --global color.ui auto
```
```bash
git config --list
```

# Creacion
```bash
git init 
```
--> Iniciar repo
```bash
git add .
```
--> Añadir todos los cambios
```bash
git commit -m "Texto ejemplo"
```
--> Comentario sobre los cambios realizados
```bash
git commit --amend -m "Texto ejemplo" 
```
--> Modifica el commit

```bash
git log 
```
--> Registro de todos los cambios 
```bash
git show 
```
--> Muestra la diferencia de contenido entre los commit
```bash
git diff 
```
--> Muestra las diferencias entre commits


# Practica Git 2

# Ejercicio 1
Mostrar el historial de cambios del repositorio.
Crear la carpeta capitulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto.

Añadir los cambios a la zona de intercambio temporal.
Hacer un commit de los cambios con el mensaje “Añadido capítulo 1.”
Volver a mostrar el historial de cambios del repositorio.

# Ejercicio 2
Crear el fichero capitulo2.txt en la carpeta capitulos con el siguiente texto.

Añadir los cambios a la zona de intercambio temporal.
Hacer un commit de los cambios con el mensaje “Añadido capítulo 2.”
Mostrar las diferencias entre la última versión y dos versiones anteriores.

# Ejercicio 3
Crear el fichero capitulo3.txt en la carpeta capitulos con el siguiente texto.

Añadir los cambios a la zona de intercambio temporal.
Hacer un commit de los cambios con el mensaje “Añadido capítulo 3.”
Mostrar las diferencias entre la primera y la última versión del repositorio.

# Ejercicio 4
Añadir al final del fichero indice.txt la siguiente línea:

Añadir los cambios a la zona de intercambio temporal.

Hacer un commit de los cambios con el mensaje “Añadido capítulo 5 al índice.”.

Mostrar quién ha hecho cambios sobre el fichero indice.txt.

# COMANDOS

```bash
git reset --hard "codigo"
```
---> Nos devuelve al commit que tenga ese codigo
```bash
git remote remove origin
```
---> Borramos la conexion con el servidor de github
```bash
git diff HEAD~2..HEAD
```
---> ver diferencia entre el head actual y dos commits padres anteriores(se puede usar para otras versiones).
```bash
git annotate indice.txt
```
---> Una especie de historial, nos dice cuando quien y que cambios han sido realizados.
```bash

```

```bash

```

```bash

```

```bash

```

v



