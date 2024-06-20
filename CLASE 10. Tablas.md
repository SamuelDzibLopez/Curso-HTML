
# 10. Tables.

Otro tipo de estructura que ***HTML*** permite realizar son la organización por ***tablas***.

Para generar una ***tabla***, se necesitan varias ***etiquetas*** para poder formarla.

Las etiquetas ***table***, ***tr***, ***th***, ***td***.

¿Como funcionan?, Simple

## table

La ***etiqueta table*** es la etiqueta principal, todo lo que ira dentro de la ***tabla*** que deseemos crear, ira dentro de esta.

Su sintaxis seria:

~~~
<table>
</table>
~~~

## tr

Después de la ***etiqueta table***, existe otra etiqueta, la ***etiqueta tr***.

Dentro de esta ***etiqueta*** ira el contenido de cada ***fila*** que tendrá la tabla. Podemos crear varios ***tr***.

## td y th

Estas etiquetas ***td*** y ***th*** representan a cada uno de los ***elementos*** dentro de los ***tr***.

Los ***td*** son un elemento común, una ***celda*** de una fila.

Los ***th*** son las ***cabeceras*** de cada una las columnas, por lo que esto significa que siempre irán en el primer ***tr***.

Por lo tanto, la sintaxis de una tabla completa es la siguiente:

~~~
<table>
	<tr>
		<th>Header 1</th>
		<th>Header 2</th>
		<th>Header 3</th>
	</tr>
	<tr>
		<td>Dato 1</td>
		<td>Dato 2</td>
		<td>Dato 3</td>
	</tr>
	<tr>
		<td>Dato 4</td>
		<td>Dato 5</td>
		<td>Dato 6</td>
	</tr>
</table>
~~~

***Nota:*** Las ***etiquetas th*** por defecto tienen un diseño diferente, tienen diseño de ***negritas*** y ***centrado***.

Estas ***etiquetas** son de tipo ***block***.

## colspan

El atributo ***colspan*** permite hacer que un elemento ***td*** o ***th*** puedan ocupar mas de una columna de largo.

El valor de este atributo, sera la ***cantidad de columnas*** que deseemos ocupar en la fila. 

Para ello, la sintaxis seria la siguiente:

~~~
<table>
	<tr>
		<th>Header 1</th>
		<th>Header 2</th>
		<th>Header 3</th>
	</tr>
	<tr>
		<td colspan="2">Dato 1</td>
		<td>Dato 2</td>
	</tr>
	<tr>
		<td>Dato 3</td>
		<td>Dato 4</td>
		<td>Dato 5</td>
	</tr>
</table>
~~~

***Nota:*** deberemos crear la cantidad de ***elementos td*** o ***th*** de modo, que coincidan con la lógica de la ***tabla***, de lo contrario, se desplazaran hacia la derecha.

## rowspan

Este atributo ***rowspan***, es similar al anterior, pero en vez de ocupar espacios en la fila, ocupara espacios en la ***columna***

Del mismo modo, el valor dentro del atributo sera la cantidad de ***elementos*** de la ***columna*** que deseemos ocupar.

La sintaxis en similar:

~~~
<table>
	<tr>
		<th>Header 1</th>
		<th>Header 2</th>
		<th>Header 3</th>
	</tr>
	<tr>
		<td rowspan="2">Dato 1</td>
		<td>Dato 2</td>
		<td>Dato 3</td>
	</tr>
	<tr>
		<td>Dato 4</td>
		<td>Dato 5</td>
	</tr>
</table>
~~~

***Nota:*** De igual forma que el ***colspan***, en ***rowspan*** debemos hacer coincidir la cantidad de elementos en la columna considerando estos cambios, para no descuadrar la tabla.

Podemos unir ambos atributos en un solo ***elemento***. para poder personalizar nuestra ***tabla*** a ***gusto***.


