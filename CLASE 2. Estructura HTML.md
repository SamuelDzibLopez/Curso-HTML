
# 2. HTML Structure.

***HTML*** no es mas que el código de la ***Estructura*** de un sitio web, Todo lo relacionado a diseño y estilos, los da ***CSS**.

Eso significa, que desde ***HTML*** solo se hace la parte de los ***elementos*** y ***componentes***.

Sin embargo, eso no quiere decir que sea fácil, ***HTML***, esta relacionado a la maquetación

	La Maquetación es la piedra angular de la estructura WEB.

Eso lo iras aprendiendo con el paso de la practica,... ***mucha practica***.

## ¿Qué es un etiqueta?

***HTML*** funciona con ***elementos*** que son llamadas ***Etiquetas***, pero, ¿Porque?...

Es simple, es como un supermercado, donde todo tiene que estar etiquetado, para poder saber que tipo de producto es cada cosa.

Lo mismo sucede con las ***etiquetas***, cuando deseemos darle diseño, podremos clasificaras gracias a los diferentes tipos de estas.

Un ejemplo:

	Supongamos que tenemos una etiqueta para parrafos, cuando querramos darle un diseño a los parrafos, podremos encontrarlos, gracias a su etiqueta, pero si uno no tiene la etiqueta, no podremos encontrarlo.

La estructura básica de una etiqueta es la siguiente:

~~~
<nombre>
	contenido
</nombre>
~~~

Que es igual a:

~~~
<nombre>contenido</nombre>
~~~

Se clasifica en ***3 partes importantes:***

	1. Etiqueta de inicio (<nombre>)
	2. El contenido
	3. Etiqueta de cierre (</nombre>)

Donde el ***contenido*** que en su mayoría es el texto a mostrar en pantalla, ira entre las 2 etiquetas de esta.

Un ejemplo de una etiqueta real (para un titulo) es:

~~~
<h1>Titulo 1</h1>
~~~

Existen otro tipo de etiquetas, las cuales se escriben de la siguiente manera

~~~
<br>
~~~

***Nota:*** Esta etiqueta se usa para dar un espaciado.

~~~
<hr>
~~~

***Nota:*** Esta etiqueta se usa para dibujar una linea separadora

Sin una etiqueta de cierre, esto se debe a que no tienen contenido dentro de ellas, por lo que solo basta con definirías, a diferencia de las otras, donde muestran texto variado.

## ¿Qué es un atributo?

Dentro de las etiquetas pueden ir datos que se necesitan para su funcionamiento o ser afectados.

A estos se les llama ***atributos***, y van dentro de la ***etiqueta de inicio***.

Por ejemplo:

~~~
<h1 id="titulo1">Titulo 1</h1>
~~~

La etiqueta ***h1*** tiene el atributo ***id*** con valor ***titulo1.

El valor de un atributo siempre ira dentro de ***" "***.

***Nota:*** El atributo ***id*** sirve para poder identificar con un nombre unico esta etiqueta, por ello, no puede haber una etiqueta con un ***id*** que tanga de valor el mismo que otro.

Existen otros tipos de ***atributos***

como los siguientes:

~~~
<img src="img.png" alt="imagen de gato">
~~~

Esta es una etiqueta ***img***, que sirve para poder agregar una imagen a nuestro documento.

***Nota:*** El ***atributo src*** en la etiqueta ***img*** permite colocar la ***URL*** donde se ubica el archivo imagen, debe colocarse junto con su respectiva extensión.

***Nota:*** El ***atributo alt*** sirve para poder escribir una breve descripción de la imagen, información útil para el navegador.

Cada ***etiqueta*** puede ***necesitar o no*** de ***atributos**, y no todos los ***atributos*** son compatibles con todas las ***etiquetas***.

### Atributos booleanos

Existen atributos especiales, los cuales basta con colocar el nombre del atributo y no tienen un valor como los otros, sino que afectan simplemente con ser declarados en las etiquetas.

A estos se les conoce como ***booleanos*** o ***booleans***.

Un ejemplo:

~~~
<h1 hidden>Titulo 1</h1>
~~~

***Nota:*** El ***atributo hidden*** funciona para que la etiqueta no se muestre en el contenido al momento de mostrarse.
## Estructura básica de HTML

Todo documento ***html*** tiene una ***estructura básica***.

La cual es la siguiente: 

~~~
<!DOCTYPE html>
<html lang="es">
	<head>
		<meta charset="UTF-8">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<title>Curso HTML</title>
	</head>
	<body>
		
	</body>
</html>
~~~

Parece algo dificil de entender, pero si lo simplificamos podemos dejarlo asi:

~~~
<html>
	<head>
	
	</head>
	<body>
		
	</body>
</html>
~~~

Si nos damos cuenta, esta estructura no es mas que una serie de ***etiquetas*** dentro de otra

 La ***etiqueta html*** es la principal, por lo tanto, todo se encontrará dentro de esta.

La única etiqueta fuera es:

~~~
<!DOCTYPE html>
~~~

La cual se encuentra el principio del documento, para que nuestro ***navegador*** pueda identificar que se trata de un documento ***html***.

Dentro de la etiqueta ***html*** principal se encuentran otras 2 etiquetas:

	1. head
	2. body

### head

Dentro de la ***etiqueta Head*** colocaremos toda la ***información*** y ***etiquetas*** que nos ayudan a dar formato y personalización a nuestro documento ***HTML***, la gran
mayoría de estos datos son invisibles para el lector de la página a simple vista.

Algunas de estas etiquetas ayudan a:

	- Colocar nombre a la pestaña de nuestra pagina
	- Colocar un icono o imagen en la pestaña
	- Enlazar archivos .css, .js, librerias, etc
	- Colocar información de ayuda.

Como las siguientes como ejemplo:

~~~
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Curso HTML</title>
~~~

### body

Dentro de esta ***etiqueta*** se encuentra todo el contenido textual y visible, otras ***etiquetas*** que se ven cuando se visualice

Como:

	- Parrafos de texto
	- Imagenes
	- Enlaces
	- Botones
	- Etc.

Para poder iniciar esta etiqueta, es necesario cerrar primero la etiqueta anterior
***head***, así que se puede decir que la etiqueta ***body*** se encuentra después de la etiqueta ***head***.

## Comentarios

Para poder escribir comentarios, como cualquier lenguaje, usamos la sintaxis simple

Es similar a una etiqueta:

~~~
<!--comentario-->
~~~

Donde abrimos y cerramos la etiqueta de ***comentario***.

***Nota:*** Esta sintaxis acepta comentarios de varias lineas.




