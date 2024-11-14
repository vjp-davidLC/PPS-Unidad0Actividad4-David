# PPS-Unidad0Actividad4-David 

*Realizado por: David López Castiñeira*

Vamos a hacer una nueva actividad con git. En esta ocasión crearemos un pequeño proyecto de una página web que podremos visualizar creando un pequeño servidor con php. Como en la actividad anterior el producto a realizar será el repositorio en github.


### CONFIGURACIÓN GIT

1. Configura el editor de comandos. Yo por simplicidad utilizaría nano git config — global core.editor nano

![img1](img/img1.PNG)

2. Vamos también a configurar para que cuando utilicemos git dif o git log se nos muestre todo el mensaje sin entrar en editor. Para ello `git config — global core.pager ' ' .

![img2](img/img2.PNG)

3. Comprueba qué valor tienen las variables de configuración de git. Puedes utilizar la ayuda git config --help.

![img3](img/img3.PNG)

4. Ajusta los valores de las variables de Git:

color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto

![img4](img/img4.PNG)

### CREACIÓN DE PROYECTO Y REPOSITORIO.


Creamos un nuevo repositorio en GitHub a través del terminal que sea público:

Antes creamos el repositorio en GitHub sin README.md. Nos saldrá lo siguiente:

![img5](img/img5.PNG)

Hacemos lo primero que nos pide.

![img6](img/img6.PNG)

![img7](img/img7.PNG)

![img8](img/img8.PNG)

![img9](img/img9.PNG)

Editamos en fichero README.md y le añadimos una descripción del ejercicio.

![img10](img/img10.PNG)

![img11](img/img11.PNG)

![img12](img/img12.PNG)

![img13](img/img13.PNG)

Comprobamos el resultado.

![img14](img/img14.PNG)

### IGNORANDO ARCHIVOS.

1. Creamos una carpeta con nombre Excluded. En ella vamos a colocar la documentación que no queremos que sea rastreada y subida al repositorio.

![img15](img/img15.PNG)

2. Para comprobar que funciona crea algún archivo vacío allí y también crea un archivo con nombre excluido.txt en el directorio principal del repositorio.

![img16](img/img16.PNG)

3. Crea un archivo con nombre .gitignore en el cual vamos a poner los archivos y directorios que no queremos que se rastreen.

4. Indica en el .gitignore que los archivos con extensión .txt y el directorio Excluded no deben de ser rastreados ni sincronizados.


![img17](img/img17.PNG)

![img18](img/img18.PNG)

5. Comprueba el estado del proyecto y comprueba que no nos indica nada del seguimiento de dichos archivos.

![img19](img/img19.PNG)

Y añadió los cambios y lo subimos al repositorio.

![img20](img/img20.PNG)

### TRABAJO CON GIT

1. Crea un archivo con nombre index.html.
2. Introduce el código html para que nos muestre un mensaje de Hola mundo con tu nombre. Uno sencillo sería este:
  `<H1>Hola $USER¡¡¡ ¿Qué tal te encuentras?</H1>`

![img21](img/img21.PNG)

![img22](img/img22.PNG)

3. Visualiza el estado del proyecto ( puedes hacer también un git status corto git status --s` o `git status --short).

![img23](img/img23.PNG)

4. Puedes ver como te indica que tienes varias operaciones por hacer: git add, git commit...
5. Añade el archivo index.html al proyecto (git add).

![img24](img/img24.PNG)

6. Haz un commit (Puedes hacer `commit -am "commentario del commit` de esta manera se añaden las modificaciones de archivos y se hace el commit con el mensaje indicado sin abrir el archivo y tener que escribir nosotros).

![img25](img/img25.PNG)

7. Vuelve a comprobar el estado del proyecto. Puedes ver como ya debería de estar todo en orden.

![img26](img/img26.PNG)

8. Vuelve a subir los cambios a tu repositorio de github (git push)

![img27](img/img27.PNG)

### CREACIÓND DE NUESTRO SERVIDOR WEB Y VISUALIZACIÓN DE NUESTRO PROYECTO

1. En una nueva pestaña de terminal y en el mismo directorio, ejecuta php -S 0:8080 para lanzar un servidor con la página html que has creado.

![img28](img/img28.PNG)

2. Visualiza la página creada Puedes acceder a ella en tu navegador en el puerto 8080 de tu equipo: 127.0.0.1:8080

![img29](img/img29.PNG)

### SEGUIMOS TRAAJANDO CON GIT

1. Haz una copia del archivo local index.html con el nombre index.html.save. Modifica el fichero index.html para que cambie el texto mostrado en la página web.

![img30](img/img30.PNG)

2. Verifica el estado del proyecto.

![img31](img/img31.PNG)

3. Comprueba las diferencias de los archivos que no han sido añadidos (`git diff`)

![img32](img/img32.PNG)
(No me sale nada)

4. Refresca el navegador para comprobar que ha cambiado el contenido de nuestra página web.

![img33](img/img33.PNG)

5. Vuelve a la versión anterior del archivo index.html (`git restore`).

![img34](img/img34.PNG)

6. Vuelve a refrescar navegador para ver como vuelve a versión inicial.

![img35](img/img35.PNG)

7. Utiliza el comando git mvpara sobreescribir el archivo index.html con index.html.save

![img36](img/img36.PNG)

8. Mira el estado del proyecto y confirma todos los cambios.

![img37](img/img37.PNG)

9. Para pull y push, haz un push y comprueba cómo han subido los archivos a github.com.

![img38](img/img38.PNG)

![img39](img/img39.PNG)

10. Modifica el archivo index.php desde la página de github.com y haz un pull y comprueba cómo se ha modificado la página web en nuestro navegador.

![img40](img/img40.PNG)

![img41](img/img41.PNG)

![img42](img/img42.PNG)

### GIT LOG

*Aquí he cambiado la variable core.pager para que funcione bien los ejercicios*

1. Mira la página de (Git Book sobre los comandos git log)[https://git-scm.com/book/es/v2/Fundamentos-de-Git-Ver-el-Historial-de-Confirmaciones]
   
2. Muestra los logs

![img43](img/img43.PNG)

3. Muestra los logs de los últimos 3 commits

![img44](img/img44.PNG)

4. Muestra los logs utilizando el modificador ``--pretty`

![img45](img/img45.PNG)

5. Muestra los logs de los últimos 2 commits donde se vean las diferencias de cada una de las entradas.

![img46](img/img46.PNG)

6. Muestra los logs de las modificaciones realizadas en el último día

![img47](img/img47.PNG)

### RAMAS

1. Lista las ramas existentes.

![img48](img/img48.PNG)

2. Crea una nueva rama con nombre Vers1 a partir de la rama actual.

![img49](img/img49.PNG)

![img50](img/img50.PNG)

3. Haz una modificación del index.html y guardas modificaciones.

![img51](img/img51.PNG)

![img52](img/img52.PNG)

4. Sube los cambios al respositorio remoto a la rama Vers1 git push origin Vers1 (En este caso podemos ver cómo el index.html de la rama m̀ain y Vers1 son diferentes.

![img53](img/img53.PNG)

![img54](img/img54.PNG)
