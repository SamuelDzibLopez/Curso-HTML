
# 8. Lists.

En ***HTML*** podemos escribir texto en forma de ***listas***; Muy útiles cuando se quiere mostrar ***contenido organizado***.

Existen ***2 tipos de listas*** diferentes:

	- Ordenadas
	- Desordenadas

Las ***listas*** en ***HTML*** son usadas mayormente para hacer menús de navegación o índices.

## Listas ordenadas

Las ***listas ordenadas*** son listas que podemos crear las cuales están ***enumeradas*** por defecto.

Podemos hacer uso de la etiqueta **ol** para crear la ***lista enumerada*** y la ***etiqueta li*** para crear los puntos.

La sintaxis sera la siguiente:

~~~
<ol>
	<li>
		Punto 1
	</li>
	<li>
		Punto 2
	</li>
	<li>
		Punto 3
	</li>
	<li>
		Punto 4
	</li>
</ol>
~~~

## Listas desordenadas

Para crear listas desordenadas usaremos la etiqueta ***ul*** y las etiquetas ***li***

La etiqueta ***ul*** nos creara la lista en general, mientras que la etiqueta ***li*** (dentro de ***ul***) para los títulos dentro de esta.

Un ejemplo de la sintaxis:

~~~
<ul>
	<li>
		Punto
	</li>
	<li>
		Punto
	</li>
	<li>
		Punto
	</li>
	<li>
		Punto
	</li>
</ul>
~~~

Este tipo de ***listas*** es utilizada para hacer elementos de ***navegación***.

***Nota:*** Podemos agregar etiquetas ***a*** de ***enlaces*** dentro del contenido de los ***li*** para hacer una ***lista de enlaces***, tanto en ***listas ordenadas*** o ***listas desordenadas***.

~~~
<ul>
	<a href="">
		<li>
			Punto 1
		</li>
	</a>
	<a href="">
		<li>
			Punto 2
		</li>
	</a>
	<a href="">
		<li>
			Punto 3
		</li>
	</a>
</ul>
~~~

***Nota:*** También podemos ***anidar*** listas dentro de elementos de otras, sin importar si son ***ordenadas*** o ***desordenadas***.

Estas ***etiquetas*** son de tipo ***block***.
