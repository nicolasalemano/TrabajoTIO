
# Mejores practicas css
## 1. Sea Organizado
    * Una de las mejores practicas es tener el código, en lugar de escribir en cualquier lugar es bueno tener un orden, esto ayuda a mantener el concepto de cascada
    * Declaración de artículos mas genéricos primeros, luego los que no es tan genérico y así sucesivamente. Esto permite que su CSS herede correctamente los atributos y lo hace mucho más fácil.
    * Utilice una estructura que funciona mejor para usted, manteniendo ediciones futuras y otros cambios futuros.
        * Resets y overrides
        * Enlaces y type
        * Diseño principal
        * Estructuras de diseño secundarias
        * Elementos de formulario
        * Demás diseño

## 2. Título, Fecha Y Signos
	* Agregar una firma en el archivo css para que otros sepan quien escribio el código y como contactarlo.

## 3. Mantener Una Biblioteca De Plantillas
	*Una vez que se decida por una estructura para usar, quitar todo lo que no es genérico y guarde el archivo como una plantilla CSS para su uso posterior.
	*Puede guardar varias versiones para múltiples usos: un diseño de dos columnas, un diseño de blog, de impresión, móviles y así sucesivamente. Es una perdida de tiempo y conllleva mas trabajo tener que volver a escribir cada una de sus hojas de estilo desde el principio, sobre todo cuando se está utilizando las mismas convenciones y metodologías en cada uno.

## 4 Utilice Convenciones de nomenclatura de interés
	* Utilizar nomenclaturas que hagan referenica a lo que se esta aplicando un estilo, ejemplo: en vez de llamar col-a que se quiere que este alineada a la izquierda o derecha seria conveniente llamar col-izq o col-der, esto ayudaria mucho en un fututuro para poder realizar alguna cambio.
	* Una de las principales ventajas del CSS es la capacidad de separar estilos de contenido. Puede rediseñar completamente su sitio con sólo modificar el CSS sin tener que tocar el código HTML . Así que no arruinar definitivamente el CSS mediante el uso de nombres de limitantes. Utilice convenciones de nomenclatura más versátiles y coherentes.
	* En lo posible hacer referencia a lo que hace la clase, ejemplo link-blue con dos simples palabras se puede saber que aplicando esa clase el color de un link va a ser azul.


## 5. Guiones En Lugar De Under Lines

	* Para una mejor compatibilidad con versiones anteriores de los navegadores, es mejor entrar en el hábito de usar guiones en su lugar de los conocidos sub rayados ó under lines. Use #col-alpha en lugar de #col_alpha.
	
	
## 6. No Repitas Código

	* La re utilización de atributos es útil, siempre que sea posible mediante la agrupación de elementos en lugar de declarar los estilos de nuevo. Si su h1 y h2  utilizan el mismo tamaño de fuente, color y márgenes, agruparlos mediante una coma, de la siguiente manera:

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

	* También debe hacer uso de los atributos en linea siempre que sea posible. Siempre estar en la búsqueda de oportunidades para los elementos del grupo y utilizar los métodos abreviados de declaración. Por ejemplo:

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

