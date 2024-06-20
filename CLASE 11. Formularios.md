
# 11. Forms.

Los ***formularios*** permiten al usuario poder ingresar datos a nuestra ***pagina***, para poder recibirla, para ya sea, almacenar esos datos o realizar acciones dependiendo de las posibles opciones programadas.

Al igual que las tablas, los ***formularios*** tienen una ***etiqueta*** principal, ***form***

~~~
<form action="" method="">
</form>
~~~

Dentro de esta etiqueta, irán todos los ***campos*** y ***etiquetas*** necesarias para que el ***cliente*** ingrese sus ***datos*** y poder ***capturarlos***.

***Nota:*** La ***etiqueta form*** tiene por defecto ***2 atributos***, ***action*** y ***method***:

	action: Recibe la URL hacia donde se enviaran los datos del formulario.
	method: Metodo por el cual se envian los datos, existen 2 metodos, POST y GET.

Dependiendo de las ***tecnologías*** que se utilicen, estos ***atributos*** pueden utilizarse o no.

## inputs

Los ***inputs*** son los campos donde el usuario puede ***interactuar*** para poder ingresar los datos.

La ***sintaxis*** de una etiqueta ***input*** es la siguiente:

~~~
<input type="">
~~~

***Nota:*** Siempre esta etiqueta va acompañada de su atributo ***type***, el cual define el tipo de dato que sera ***valido*** a ingresar por el usuario en el ***campo***. 

Existen diferentes tipos de ***inputs***:

	- text
	- number
	- tel
	- password
	- email
	- color
	- range
	- date
	- time
	- datetime-local
	- file
	- radio
	- checkbox
	- reset
	- submit
	- button

Ademas de estas, existen otras ***etiquetas*** que no son ***inputs***, pero son campos de ingreso de datos, tales como:

	- select
	- textarea
	- button

Estas ***etiquetas*** son de tipo ***inline***.

### text

Esta es la etiqueta por defecto, permite el ingreso de texto, incluyendo ***letras***, ***números*** y ***caracteres especiales***.

La sintaxis es:

~~~
<input type="text">
~~~

### number

Dentro de este tipo de campo. solo se permite el ingreso de ***números***.

La sintaxis es:

~~~
<input type="number">
~~~

### tel

Este tipo de ***input*** permite el ingreso de texto, incluyendo ***letras***, ***números*** y ***caracteres especiales***.

Es similar al ***text***, pero tiene una ***semántica*** respecto a datos del usuario para ***telefono*** o ***celular***.

Sintaxis:

~~~
<input type="tel">
~~~

### password

Con contexto a su nombre, se utiliza para ***contraseñas***, ocultando el contenido de este campo.

Su sintaxis:

~~~
<input type="password">
~~~

***Nota:*** Dependiendo del ***browser*** en ocasiones este campo mostrara un botón extra para poder visualizar el contenido de la contraseña.

### email

Este campo permite el ingreso de cadenas de texto con expresión de ***correo electrónico***.

Su sintaxis es la siguiente:

~~~
<input type="email">
~~~

***Nota:*** Si esta ***expresión regular*** no se cumple, el ***formulario*** no se enviara hasta cumplirse en el campo.

### color

Este ***input*** permite visualizar una paleta de ***colores***, donde el usuario podra elegir un ***tono de color***.

Su sintaxis:

~~~
<input type="color">
~~~

### range

Este tipo de ***input*** permite elegir un ***numero*** con base a la visualización de una ***barra de rango***.

Este ***input*** tiene otros ***2 atributos*** extra, para poder definir este ***rango***.

Un ejemplo de su sintaxis, con un ***rango*** de ***0-100***:

~~~
<input type="range" min="0" max="100">
~~~

### date

Este ***input*** permite el ingreso a su campo datos de tipo ***fecha***.

Dentro de este campo se muestra un ***calendario*** para ayudar al ***cliente***, pero tambien 

El ***formato*** del valor es: 

	mm/dd/yy (mes/dia/año)

Su sintaxis es la siguiente:

~~~
<input type="date">
~~~

### time

muy similar al ***date***, pero su diferencia es que ***time*** recibe dato de tipo ***tiempo*** o ***hora***.

Con un ***formato***:

	hh:mm:PM (horas:minutos:rango)

Su sintaxis es:

~~~
<input type="time">
~~~

### datetime-local

El ***input datetime-local*** es la unión de los ***inputs date*** y ***time*** en uno.

con un ***formato***:

	mm/dd/yy, hh:mm:PM 

Su sintaxis es:

~~~
<input type="datetime-local">
~~~

### file

Permite el ingreso de ***archivos***, independientemente de su extensión.

***Nota:*** Es ***IMPORTANTE*** para la ***seguridad*** poder controlar el tipo de ***archivos*** aceptados, para ello, la etiqueta de este ***tipo***, tiene un atributo especial, ***accept***.

Aun así, es importante, validar esta seguridad de otras diferentes formas

Su sintaxis es la siguiente, configurando que acepte únicamente, ***.pdf***:

~~~
<input type="file" accept=".pdf">
~~~

***Nota:*** Para que estos tipos de ***inputs*** funcionen, es necesario colocar a nuestra ***etiqueta form*** el siguiente ***atributo***:

~~~
enctype="multipart/form-data"
~~~

Que permitirá leer y procesar ***archivos file***.

### radio

Este ***input*** es diferente a los anteriores, ya que ***NO*** es un ***campo de texto*** donde el usuario coloca ***texto***.

Un ***input radio*** es un ***botón boolean*** el cual puede ***activarse*** o ***desactivarse***.

La sintaxis es la siguiente:

~~~
<input type="radio" value="1">
~~~

***Nota:*** Al no ser un ***campo de texto***, este tipo de ***input*** debe contener el ***atributo value*** con el valor que desea tener el ***input activado*** , a pesar de no estar visible, este ***valor*** se envía cuando se haga el ***submit***.

Este tipo de ***input*** suele ser usado cuando solo se puede elegir ***una opcion***, por lo que para ello, debemos colocarles un atributo si tenemos varios ***radio***.

El ***atributo*** clave es ***name***.

Supongamos que tenemos ***3 radio*** pero solo uno debe poder elegirse, para ello, damos el mismo valor en el ***atributo name*** a los 3.

~~~
<input type="radio" value="1" name="nombre">
<input type="radio" value="2" name="nombre">
<input type="radio" value="3" name="nombre">
~~~

De este modo, al seleccionar uno, si ya esta seleccionado otro, se desactivará.

### checkbox

Es muy similar a un ***input radio***, pero este se usa, cuando podemos elegir ***varias opciones*** de una lista de ellas.

Al igual, ***NO*** es un ***campo de texto***, por lo que debe contener su ***atributo value***, el cual se mandara, si se encuentra seleccionado.

Su sintaxis es:

~~~
<input type="checkbox">
~~~

### resert

Este tipo de ***input***, ***NO*** es un ***campo de texto***, es un ***botón***, pero tiene una configuración de funcionamiento redefinido.

Su función es ***resetear*** un ***formulario*** al hacer ***click*** en ***él***.

Para ello, la sintaxis es la siguiente:

~~~
<input type="reset">
~~~

Por defecto, este ***input/botón*** tiene un texto, pero, podemos cambiarlo con el atributo ***value***.

~~~
<input type="reset" value="Limpiar">
~~~

***Nota:*** No olvidemos colocar este ***input*** dentro de la etiqueta ***form***, al igual a los otros ***inputs*** que serán ***afectados***.

### submit

Igual a ***resert***, el ***input*** de tipo ***submit*** es un ***botón***, pero con una configuración predeterminada.

Su ***función*** es ***enviar*** los ***datos*** del ***formulario***.

Su sintaxis es:

~~~
<input type="submit">
~~~

Al igual, que al ***input*** anterior, este necesita estar dentro de la etiqueta ***form*** para activarse, y todos los otros ***inputs*** que desean enviarse sus ***values***.

Y al igual, podemos cambiar el texto por defecto 

### button

Un ***input button*** es un simple ***boton***, a diferencia de ***reset*** y ***submit***, este no tiene una configuración predefinida, por lo que es ***util*** para configuraciones personalizadas.

Su sintaxis es:

~~~
<input type="button" value="Botón">
~~~

***Nota:*** Este ***input*** no tiene un texto definido, por lo que es necesario colocarle un valor al ***value***.


## Otras etiquetas

Existen otros ***campos*** y ***etiquetas*** que no son de sintaxis ***input*** pero son útiles para poder ingresar datos en un ***formulario***.

### select

Esta es una ***etiqueta*** que permite mostrar al ***cliente*** una serie de opciones elegidas por un despliegue.

La ***etiqueta select*** es la principal.

Su sintaxis es la siguiente:

~~~
<select>
</select>
~~~

Y dentro de esta etiqueta, van las ***etiquetas de las opciones***.

## option

La ***etiqueta option*** representa cada una de ellas, acompañada de su ***atributo value*** y su valor a enviar si la ***opcion es seleccionada***.

Cuya sintaxis es la siguiente:

~~~
<option value="MX">Mexico</option>
~~~

***Nota:*** No olvidemos, que el ***valor*** y ***contenido*** son ***diferentes***.

En un ***select*** se codificaría de la siguiente manera, con un ejemplo:

~~~
<select>
	<option value=""></option>
	<option value="MX">Mexico</option>
	<option value="USA">Estados Unidos</option>codificaria
	<option value="ESP">España</option>
</select>
~~~

***Nota:*** Por lo general, se suele colocar una ***opción vacía*** como campo vacío para no elegir alguno, casualmente al ***inicio***.

## textarea

Esta ***etiqueta*** es a simple vista igual a un ***input text***, pero este permite ***textos amplios*** y ***saltos de linea***, útil para el uso de ***descripciones*** y ***comentarios***.

Su sintaxis es la siguiente:

~~~
<textarea>
</textarea>
~~~

## button

Esta etiqueta es la simplificación de las etiquetas ***input*** de tipo ***button***, ***submit*** y ***reset***.

Por ejemplo, se hace el cambio de :

~~~
<input type="button" value="Botón">
~~~

A la etiqueta ***button***, esto representa lo mismo

~~~

<button type="button">Botón</button>
~~~

Lo mismo sucede con ***reset*** y ***submit***.

***Nota***: Si dentro de un ***form*** se encuentra un ***button*** que no tiene definido un ***type*** se entiende por el ***navegador*** que es de tipo ***submit***.

Estas son la ***gran mayoría*** de ***etiquetas útiles*** en un ***formulario***; Ahora, veamos unos ***atributos útiles*** para ellas.  

## Atributos 
### value

### placeholder

### maxlenght
### minlength

### requerid


