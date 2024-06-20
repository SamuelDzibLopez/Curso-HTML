
# 1. HTML Fundaments.

***HTML*** significa ***(Hypertext Markup Language)*** o en español  ***Lenguaje de Marcado de Hipertexto***.

	HTML ES UN LENGUAJE,... PERO

	HTML NO ES UN LENGUAJE DE PROGRAMACION.

Es el lenguaje que permite al usuario poder visualizar el contenido dentro de la ***web***, por medio de lo que llamamos ***navegadores*** o ***browsers***; Reemplazando por innovación a ***XML***.

La web funciona por medio de un protocolo denominado ***HTTTP***, que no es mas que la petición de código a un servidor llamado ***dominio***, para poder luego ser interpretado y visualizado.

Dentro de este, se manejan ***2 estructuras*** llamadas ***front-end*** y ***back-end***, también conocidas como ***cliente*** y ***servidor***.

***HTML*** se clasifica en la estructura dentro del ***front-end*** o ***cliente***.
## Archivos básicos

Para la vista del cliente, se utilizan 3 principales tipos de archivos:

	- Archivos .html (Estructura).
	- Archivos .css (Estilos y Diseño).
	- Archivos .js (Interactividad y funcionalidad)

Existen otros tipos de archivos, en especial si se utilizan ***librerías*** o ***frameworks***, pero son una variedad de los anteriores.
## Nombres de archivos

Por regla ***general*** y ***estándar***, se suele llamar de una manera a los archivos principales, para poder identificarlos de manera sencilla.

### index.html

El primer documento básico es:

~~~
index.html
~~~

Este es el nombre que suele darse al documento que presenta el contenido principal del sitio, es decir la vista principal al que el ***usuario*** sera redirigido al momento de ingresar al dominio. 

***Nota:*** Actualmente, algunos hostings ya permiten nombrar este archivo de manera diferente y configurarlo como el principal sin la necesidad de esta regla.

### style.css

Para los estilos, existe un estandar:

~~~
style.css
~~~

Este no es un nombre obligatorio o tiene un funcionamiento por ello, simplemente es un nombre que identifica el contenido de los ***estilos*** de manera general.

Dentro de este suelen colocarse los ***estilos*** principales del ***index.html***  y las reglas generales de todo el resto de las paginas o módulos.

Dentro de nuestros archivos ***.html*** podemos enlazar un archivo ***.css*** que hallamos creado, con el nombre que elegimos.

***Nota:*** En general este documento suele tener todas las reglas que se efectuan en nuestro sitio completo y podemos crear otro documento exclusivo para un modulo en concreto después.

### script.js

~~~
script.js
~~~

Este es el nombre por ***defecto*** que se le suele llamar a los archivos enlazados al ***.html***.

Al igual que los documentos ***.css***, no afecta a la funcionalidad

Su nombre deriva principalmente debido a que la manera coloquial de llamar a que agregar funcionalidad a algo se suele llamar ***script***, y debido a que los documentos ***,js*** son exactamente lo que hacen con los elementos ***html***, por eso se llaman así.

Pero en general, también suelen llamarse por el nombre de la funcionalidad que realizan.

Por ejemplo, si tenemos un elemento ***js*** que hace funcionar un carrusel, podemos llamarle:

~~~
carrusel.js
~~~

O si es para un formulario...

~~~
formulario.js
~~~

***Nota:*** Una buena practica es nombrar en ***ingles***.


