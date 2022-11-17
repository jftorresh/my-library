# Paso a paso

Tener en cuenta, que como es un proyecto en comunidad, al tener dos personas acceso al proyecto, se requiere siempre traer primero los posibles cambios realizados por una de las dos personas

##### 1. Abrir proyecto desde el explorador de archivos

Desde el explorador de archivos de WIndows, nos dirigimos a la carpeta contenedora del proyecto, en mi caso se visualiza de este modo: 

![](https://jftorresh.github.io/my-library/assets/images/step-1.png)

##### 2. Abrir CMD del proyecto

Desde el explorador de archivos dentro del proyecto, realizaremos un click derecho en un espacio en blanco, desplegaremos las opciones del menu y seleccionamos una de las dos opciones siguientes disponibles.

![](https://jftorresh.github.io/my-library/assets/images/step-2.png)

En mi caso seleccione _**"Abrir la ventana de PowerShell aqui"**_, sin embargo cualquiera de las dos opciones funciona.

##### 3. Traer posibles cambios realizados en el sitio web

A continucacion redactaremos unas cuantas lineas de codigo dentro de la consola de comandos, es imperativo realizar el paso a paso correctamente, para no cometer ningun error

- Verificamos que nos encontramos en la rama **"Master"** con el comando **"git branch"**

```cmd
c:\path\of\the\project> git branch
```

Deberia de aparecer algo como lo siguiente

![](https://jftorresh.github.io/my-library/assets/images/step-3.png)

- Procedemos a traer los posibles cambios del sitio web con el comando **"git pull origin master"**

```cmd
c:\path\of\the\project> git pull origin master
```

![](https://jftorresh.github.io/my-library/assets/images/step-4.png)

Deberia de aparecer algo como esto en la mayoria de los casos, pero si no es asi, no hay lio, todo va segun lo planeado.

##### 3. Agregar un nuevo libro

Abrimos el editor de **Mobirise** y nos dirigimos a una de las secciones disponibles para agregar nueva documentación a nuestro proyecto.

- Menu lateral

![](https://jftorresh.github.io/my-library/assets/images/step-5.png)

- Paginas disponibles

![](https://jftorresh.github.io/my-library/assets/images/step-6.png)

- Fuentes bibliograficas en este caso

![](https://jftorresh.github.io/my-library/assets/images/step-7.png)

- Nos dirigimos a cualquiera de los items disponibles y posamos el cursor encima del item, donde apareceran las siguientes opciones.

![](https://jftorresh.github.io/my-library/assets/images/step-8.png)

- Seleccionamos la opcion _**"Add items"**_
- Seleccionamos la imagen de nuestro nuevo documento, si la tenemos disponible en la biblioteca existente, sino navegamos ne nuestro PC y la agregamos

![](https://jftorresh.github.io/my-library/assets/images/step-9.png)

- Una vez agregada, con la imagen seleccionada, cambiamos el enlace del documento al cual nos redirige

![](https://jftorresh.github.io/my-library/assets/images/step-10.png)

- Navegamos entre los documentos disponibles o lo agregamos desde nuestro PC, y lo insertamos en el enlace

![](https://jftorresh.github.io/my-library/assets/images/step-11.png)
![](https://jftorresh.github.io/my-library/assets/images/step-12.png)

- Seleccionamos el titulo y lo cambiamos por el nombre de nuestro libro

![](https://jftorresh.github.io/my-library/assets/images/step-13.png)

- Una vez hechos todos los anteriores cambios, procedemos a publicar el sitio web. Primero es necesario guardar los cambios realizados dentro del repositorio

![](https://jftorresh.github.io/my-library/assets/images/step-14.png)

- Navegamos hasta donde tenemos guardado el proyecto, deberia de verse algo como esto
- Oprimimos en **"Publicar"**, y esperamos a que se guarden correctamente los archivos

![](https://jftorresh.github.io/my-library/assets/images/step-15.png)

##### 4. Consola de comandos, y publicacion del proyecto

- Una vez se guardaron los cambios, nos redirigimos a la carpeta contenedora de nuestro proyecto por medio del explorador de windows
- Procedemos a abrir de nuevo el git bash o la consola de comandos de windows

![](https://jftorresh.github.io/my-library/assets/images/step-16.png)

- Verficamos que nuestros cambios si se hayan agregado al repositorio con el comando **"git status"** 

```cmd
c:\path\of\the\project> git status
```

![](https://jftorresh.github.io/my-library/assets/images/step-17.png)

- Digitamos el comando **" git add . "** (Es imperativo el punto al final del comando, esto le indica a la maquina que debe de tener en cuenta todos los cambios realizados) y verficamos una vez mas con el comando **"git status"**, deberia de parecerse a algo como esto

```cmd
c:\path\of\the\project> git add .
c:\path\of\the\project> git status
```

![](https://jftorresh.github.io/my-library/assets/images/step-18.png)

- Si todo es correcto, digitamos el comando **' git commit -m "Some text explaining the changes made" '**, se deberia de ver algo como esto: (La explicacion del commit no es necesaria en ingles, puede ser en cualquier idioma, yo lo hago por costumbre, pero puede ser cualquiera)

```cmd
c:\path\of\the\project> git commit -m "Some text explaining the changes made"
```

![](https://jftorresh.github.io/my-library/assets/images/step-19.png)

- Finalmente nuestro ultimo comando, digitamos **"git push origin master"**, deberiamos de ver algo como esto

```cmd
c:\path\of\the\project> git push origin master
```

![](https://jftorresh.github.io/my-library/assets/images/step-20.png)

##### 5. Conclusión

Si todo fue correcto, y no se cometio ningun error durante el proceso, deberiamos de ver los cambios reflejados en el [sitio web](https://jftorresh.github.io/my-library/)
