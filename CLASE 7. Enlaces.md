
# 7. Links.

Los ***enlaces*** son una de las piezas más importantes de un sitio web, permiten redirigir al ***usuario*** a otra pagina o sitio con un solo click.

Para ello hacemos uso de la etiqueta ***a***.

~~~
<a href="pagina.html">Haz click aqui</a>
~~~

Para el ***funcionamiento*** de esta ***etiqueta***, siempre va acompañada de su ***atributo href***, en el cual se ingresa la ruta hacia el archivo al cual ***rediriguir***.

Dentro de la etiqueta, en el contenido que deseamos que se muestre en pantalla

Esta ***etiqueta*** es de tipo ***inline***.
## Tipos de enlaces

Existen ***2 tipos*** de enlaces:

	- Relativos
	- Absolutos

### Enlaces relativos

Los ***enlaces relativos*** son aquellos donde la URL de la ***direccion*** puede variar, por lo general, estos suelen ser los ***enlaces*** que tenemos para ***dentro de nuestro sitio interno***.

Por ejemplo: un ***enlace relativo***, podría ser:

~~~
<a href="paginas/pagina.html">Haz click aqui</a>
~~~

Debido a que nosotros podríamos mover el documento a donde redirecciona, mover el enlace y seguiría sin cambios.

### Enlaces absolutos

A diferencia de los anteriores, los ***enlaces absolutos*** son aquellos enlaces en los que no podemos hacer cambios, mayormente ***enlaces*** de ***sitios externos***.

~~~
<a href="www.google.com">Haz click aqui</a>
~~~

## Abrir enlaces en otras pestañas

Si se desea que al ***hacer click*** en un ***enlace*** este se abra en una pestaña nueva, para no perder la pagina actual, podemos hacer uso del atributo ***target*** con el atributo ***_blank***.

Un ejemplo:

~~~
<a href="https://www.youtube.com/" target="_blank">Haz click aqui</a>
~~~

Los ***enlaces*** no solo pueden redirigir a otro sitio web sino que también, puede redirigir a otros lugares, para facilitar al usuario, ciertas acciones, como poder incitar a enviar un correo, mensaje, whatsapp, etc.

## Enlaces para correo

Podemos agregar un enlace para mandar ***emails***.

Con la etiqueta a podemos usarla, con el valor del atributo ***href*** como
***mailto:***(dirección del correo electrónico).

~~~
<a href="mailto:correo@gmail.com">Enviar correo</a>
~~~

Donde ***correo@gmail*** es cambiado por el correo electronico. 

Podemos agregarle el atributo ***title***, el cual nos sirve pata poder ver información al pasar el ***cursor*** por el ***enlace***.

~~~
<a href="mailto:correo@gmail.com" title="Enviar correo">Enviar correo</a>
~~~

Como el ***ejemplo*** anterior.

## Enlaces para whatsapp

También podemos enviar a ***whatsapp***.

Para ello, modificamos el ***a*** de la siguiente manera:

~~~
<a href="whatsapp://send?phone=+numero>Enviar WhatsApp</a>
~~~

donde ***numero*** cambiamos al numero de ***whatsapp***.
## Enlace para SMS

~~~
<a href="sms:+1234567890?body=Hola,%20este%20es%20mi%20mensaje">Enviar SMS</a>
~~~

donde ***numero*** cambiamos al numero ***telefónico***.

***Nota:*** Estos enlaces, piden permiso al usuario, para poder acceder a las ***apps***.

