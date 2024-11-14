# PPS-Unidad0Actividad4-David 
Vamos a hacer una nueva actividad con git. En esta ocasión crearemos un pequeño proyecto de una página web que podremos visualizar creando un pequeño servidor con php. Como en la actividad anterior el producto a realizar será el repositorio en github.




### CONFIGURACIÓN GIT

Configura el editor de comandos. Yo por simplicidad utilizaría nano git config — global core.editor nano



Vamos también a configurar para que cuando utilicemos git dif o git log se nos muestre todo el mensaje sin entrar en editor. Para ello `git config — global core.pager ' ' .


Comprueba qué valor tienen las variables de configuración de git. Puedes utilizar la ayuda git config --help.



Ajusta los valores de las variables de Git:

color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto

### CREACIÓN DE PROYECTO Y REPOSITORIO.


Creamos un nuevo repositorio en GitHub a través del terminal que sea público:

Antes creamos el repositorio en GitHub sin README.md. Nos saldrá lo siguiente:


Hacemos lo primero que nos pide.









Editamos en fichero README.md y le añadimos una descripción del ejercicio.









Comprobamos el resultado.



### IGNORANDO ARCHIVOS.

Creamos una carpeta con nombre Excluded. En ella vamos a colocar la documentación que no queremos que sea rastreada y subida al repositorio.



Para comprobar que funciona crea algún archivo vacío allí y también crea un archivo con nombre excluido.txt en el directorio principal del repositorio.



Crea un archivo con nombre .gitignore en el cual vamos a poner los archivos y directorios que no queremos que se rastreen.

Indica en el .gitignore que los archivos con extensión .txt y el directorio Excluded no deben de ser rastreados ni sincronizados.





Comprueba el estado del proyecto y comprueba que no nos indica nada del seguimiento de dichos archivos.



Y añadió los cambios y lo subimos al repositorio.



### TRABAJO CON GIT

Crea un archivo con nombre index.html.
Introduce el código html para que nos muestre un mensaje de Hola mundo con tu nombre. Uno sencillo sería este:
  <H1>Hola $USER¡¡¡ ¿Qué tal te encuentras?</H1>





Visualiza el estado del proyecto ( puedes hacer también un git status corto git status --s` o `git status --short).

Puedes ver como te indica que tienes varias operaciones por hacer: git add, git commit...
Añade el archivo index.html al proyecto (git add).

Haz un commit (Puedes hacer ``commit -am "commentario del commit"` de esta manera se añaden las modificaciones de archivos y se hace el commit con el mensaje indicado sin abrir el archivo y tener que escribir nosotros).


Vuelve a comprobar el estado del proyecto. Puedes ver como ya debería de estar todo en orden.

Vuelve a subir los cambios a tu repositorio de github (git push)


### CREACIÓND DE NUESTRO SERVIDOR WEB Y VISUALIZACIÓN DE NUESTRO PROYECTO

En una nueva pestaña de terminal y en el mismo directorio, ejecuta php -S 0:8080 para lanzar un servidor con la página html que has creado.

Visualiza la página creada Puedes acceder a ella en tu navegador en el puerto 8080 de tu equipo: 127.0.0.1:8080



### SEGUIMOS TRAAJANDO CON GIT

Haz una copia del archivo local index.html con el nombre index.html.save. Modifica el fichero index.html para que cambie el texto mostrado en la página web.

Verifica el estado del proyecto.

Comprueba las diferencias de los archivos que no han sido añadidos (git diff)

(No me sale nada)
Refresca el navegador para comprobar que ha cambiado el contenido de nuestra página web.

Vuelve a la versión anterior del archivo index.html (git restore).

Vuelve a refrescar navegador para ver como vuelve a versión inicial.

Utiliza el comando git mvpara sobreescribir el archivo index.html con index.html.save


Mira el estado del proyecto y confirma todos los cambios.


Para pull y push, haz un push y comprueba cómo han subido los archivos a github.com.



Modifica el archivo index.php desde la página de github.com y haz un pull y comprueba cómo se ha modificado la página web en nuestro navegador.





### GIT LOG

Mira la página de (Git Book sobre los comandos git log)[https://git-scm.com/book/es/v2/Fundamentos-de-Git-Ver-el-Historial-de-Confirmaciones]
Muestra los logs

Muestra los logs de los últimos 3 commits

Muestra los logs utilizando el modificador ``--pretty`

Muestra los logs de los últimos 2 commits donde se vean las diferencias de cada una de las entradas.

Muestra los logs de las modificaciones realizadas en el último día


### RAMAS

Lista las ramas existentes.

Crea una nueva rama con nombre Vers1 a partir de la rama actual.



Haz una modificación del index.html y guardas modificaciones.



Sube los cambios al respositorio remoto a la rama Vers1 git push origin Vers1 (En este caso podemos ver cómo el index.html de la rama m̀ain y Vers1 son diferentes.


