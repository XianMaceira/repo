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

# Practica Git 3. Deshacer cambios.

# Ejercicio 1

Eliminar la última línea del fichero indice.txt y guardarlo.
Comprobar el estado del repositorio.
Deshacer los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero.
Volver a comprobar el estado del repositorio.

# Ejercicio 2

Eliminar la última línea del fichero indice.txt y guardarlo.
Añadir los cambios a la zona de intercambio temporal.
Comprobar de nuevo el estado del repositorio.
Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el directorio de trabajo.
Comprobar de nuevo el estado del repositorio.
Deshacer los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero.
Volver a comprobar el estado del repositorio.

# Ejercicio 3

Eliminar la última línea del fichero indice.txt y guardarlo.
Eliminar el fichero capitulos/capitulo3.txt.
Añadir un fichero nuevo captitulos/capitulo4.txt vacío.
Añadir los cambios a la zona de intercambio temporal.
Comprobar de nuevo el estado del repositorio.
Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el directorio de trabajo.
Comprobar de nuevo el estado del repositorio.
Deshacer los cambios realizados para volver a la versión del repositorio.
Volver a comprobar el estado del repositorio.

# Ejercicio 4

Eliminar la última línea del fichero indice.txt y guardarlo.
Eliminar el fichero capitulos/capitulo3.txt.
Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Borrado accidental.”
Comprobar el historial del repositorio.
Deshacer el último commit pero mantener los cambios anteriores en el directorio de trabajo y la zona de intercambio temporal.
Comprobar el historial y el estado del repositorio.
Volver a hacer el commit con el mismo mensaje de antes.
Deshacer el último commit y los cambios anteriores del directorio de trabajo volviendo a la versión anterior del repositorio.
Comprobar de nuevo el historial y el estado del repositorio.

# COMANDOS

```bash
git checkout -- indice.txt
```
---> devuelve el fichero a su versión anterior.

```bash
git clean
```
---> elimina los archivos sin seguimiento en un directorio de trabajo del repositorio

```bash
git reset --soft
```
---> deshace el anterior "git commit"

```bash
git reset(mixed)
```
---> deshace el anterior "git commit" y todo lo realizado anteriormente a ese commit

```bash
git reset --hard
```
---> eshacer los cambios locales en el estado de un repositorio de Git(comando peligroso).

# Practica git 4. Ramas

# Ejercicio 1

Crear una nueva rama bibliografia y mostrar las ramas del repositorio.

# Ejercicio 2

Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente

Añadir los cambios a la zona de intercambio temporal.
Hacer un commit con el mensaje “Añadido capítulo 4.”
Mostrar la historia del repositorio incluyendo todas las ramas.

# Ejercicio 3

Cambiar a la rama bibliografia.

Añadir los cambios a la zona de intercambio temporal.
Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.”
Mostrar la historia del repositorio incluyendo todas las ramas.

# Ejercicio 4

Fusionar la rama bibliografia con la rama master.
Mostrar la historia del repositorio incluyendo todas las ramas.
Eliminar la rama bibliografia.
Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.


# Ejercicio 5

Crear la rama bibliografia.
Cambiar a la rama bibliografia.
Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:

Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.”
Cambiar a la rama master.
Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:

Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.”
Fusionar la rama bibliografia con la rama master.
Resolver el conflicto dejando el fichero bibliografia.txt con las referencias:

Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Resuelto conflicto de bibliografía.”
Mostrar la historia del repositorio incluyendo todas las ramas.

# COMANDOS

```bash
git branch 
```
---> Crear ramas.

```bash
git branch -av
```
 ---> Ver ramas.

```bash
git checkout "Nombre rama" 
```
---> Situarnos en la rama solicitada.

```bash
git merge "rama"
```
---> Fusionamos las otras ramas a la rama actual (normalmente la principal).

```bash
git branch -d "rama"
```
 ---> Eliminar la rama

