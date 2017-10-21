
# Mejores practicas css
## 1. Sea Organizado
    * Una de las mejores practicas es tener el c�digo, en lugar de escribir en cualquier lugar es bueno tener un orden, esto ayuda a mantener el concepto de cascada
    * Declaraci�n de art�culos mas gen�ricos primeros, luego los que no es tan gen�rico y as� sucesivamente. Esto permite que su CSS herede correctamente los atributos y lo hace mucho m�s f�cil.
    * Utilice una estructura que funciona mejor para usted, manteniendo ediciones futuras y otros cambios futuros.
        * Resets y overrides
        * Enlaces y type
        * Dise�o principal
        * Estructuras de dise�o secundarias
        * Elementos de formulario
        * Dem�s dise�o

## 2. T�tulo, Fecha Y Signos
	* Agregar una firma en el archivo css para que otros sepan quien escribio el c�digo y como contactarlo.

## 3. Mantener Una Biblioteca De Plantillas
	*Una vez que se decida por una estructura para usar, quitar todo lo que no es gen�rico y guarde el archivo como una plantilla CSS para su uso posterior.
	*Puede guardar varias versiones para m�ltiples usos: un dise�o de dos columnas, un dise�o de blog, de impresi�n, m�viles y as� sucesivamente. Es una perdida de tiempo y conllleva mas trabajo tener que volver a escribir cada una de sus hojas de estilo desde el principio, sobre todo cuando se est� utilizando las mismas convenciones y metodolog�as en cada uno.

## 4 Utilice Convenciones de nomenclatura de inter�s
	* Utilizar nomenclaturas que hagan referenica a lo que se esta aplicando un estilo, ejemplo: en vez de llamar col-a que se quiere que este alineada a la izquierda o derecha seria conveniente llamar col-izq o col-der, esto ayudaria mucho en un fututuro para poder realizar alguna cambio.
	* Una de las principales ventajas del CSS es la capacidad de separar estilos de contenido. Puede redise�ar completamente su sitio con s�lo modificar el CSS sin tener que tocar el c�digo HTML . As� que no arruinar definitivamente el CSS mediante el uso de nombres de limitantes. Utilice convenciones de nomenclatura m�s vers�tiles y coherentes.
	* En lo posible hacer referencia a lo que hace la clase, ejemplo link-blue con dos simples palabras se puede saber que aplicando esa clase el color de un link va a ser azul.


## 5. Guiones En Lugar De Under Lines

	* Para una mejor compatibilidad con versiones anteriores de los navegadores, es mejor entrar en el h�bito de usar guiones en su lugar de los conocidos sub rayados � under lines. Use #col-alpha en lugar de #col_alpha.
	
	
## 6. No Repitas C�digo

	* La re utilizaci�n de atributos es �til, siempre que sea posible mediante la agrupaci�n de elementos en lugar de declarar los estilos de nuevo. Si su h1 y h2  utilizan el mismo tama�o de fuente, color y m�rgenes, agruparlos mediante una coma, de la siguiente manera:

	*h1,h2 {
	margin : 1em 2em 0;
	font-size: 1em;
	color : #222
	}

	* Es mas eficiente que esto:

	* h1 {
	margin : 1em 2em 0;
	font-size: 1em;
	color : #222
	}

	* h2 {
	margin : 1em 2em 0;
	font-size: 1em;
	color : #222
	}

	* Tambi�n debe hacer uso de los atributos en linea siempre que sea posible. Siempre estar en la b�squeda de oportunidades para los elementos del grupo y utilizar los m�todos abreviados de declaraci�n. Por ejemplo:

	* h1{
	margin-top: 1em;
	margin-bottom: 2em;
	margin-left: 0;
	margin-right: 0
	}

	*Es equivalente a esto:

	* h1{
	margin: 1em, 2em, 0, 0;
	}

