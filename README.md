# HTML

## Que es HTML

HTML son las siglas en inglés de HyperText Markup Language, que en castellano significa Lenguaje de Marcas de HipertTexto. Se usa para crear el cuerpo de una pagina web y como su propio nombre indica es un lenguaje de marcas, que para codificar un documento incorpora etiquetas de apertura y cierre, o que se cierran en la misma etiqueta de apertura.  

## Estructura básica de HTML

La estructura minima de un HTML es:

```html
<html>
	<head>
		<title>Nombre que aparece en la pestaña</title>
	</head>
	<body>
		<p>Texto que aparece en la propia página</p>
	</body>
</html>
```

Como se puede ver, la unica diferencia entre una etiqueta de apertura y una de cierre es la **/**. Todo el codigo del HTML irá entre dos etiquetas, \<html> y \</html>.  
Dentro de esta iran \<head> y \<body>, dentro de HEAD habrá información necesaria del documento, ya sea el título que aparece en la pestaña del navegador, que codificado de caracteres tiene esa página, cada cuanto tiempo se recarga la página, etc.  
Dentro de BODY irá el contenido de la página web, imágenes, textos, links, formularios, etc. Todo lo necesrio para mostrar información al lector de la página.  
Los comentarios pueden ir en cualquier sitio porque no se ejecutan, estos se hacen de la siguiente forma: ```<!-- -->```.

-----

## Etiqueta HEAD

Contiene la información relevante de la página. En head se pueden incluir otras etiquetas como TITLE o META.  

- **\<title>Nombre\</title>**: En esta etiqueta se pone el nombre de la página web que aparecerá en la pestaña del navegador.  

- **\<meta attributes="..."/>**: Esta es una etiqueta que se cierra en la misma etiqueta de apertura, contiene atributos en su interior que ayudan a definir el comportamiento de la página.  

	- **Atributos de META**:  
	**http-equiv="refresh" content="5;URL=https://www.google.com"** a los *cinco* segundos de abrir la página en el navegador, esta se refreca y te redirige hacia la dirección indicada. Si no ponemos una URL, recarga la propia página.  
	**charset="utf-8"** especifica la codificación del documento html, ya que sin este atributo no se podría poner caracteres como la Ñ o letras acentuadas. Los valores más comunes para este atributo son *utf-8* e "iso-8859-1".  
	
## Etiqueta BODY  

- **\<body>...\</body>**: Es el cuerpo de la página, contiene todo lo necesario para mostrar la información que se quiere mostrar a los visitantes de la web, contiene el resto de las etiquetas. Tiene cinco atributos que modifican el texto y el fondo de la página.  

	- **Atributos de BODY**:  
	**background=./images/photo1.png**: Pone de fondo la imagen de la ruto que pongamos, puede ser una ruta absoluta, relativa o una URL del navegador.  
	**bgcolor="#99AABB"**: Pone un color de fondo, dicho color se pone con la nomenclatura RGB en sistema hexadecimal con una almohadilla al principio y las letras en mayúsculas, también se puede poner el nombre del color en inglés sin la almohadilla, solo que así perdemos mucho rango de elección a la hora de escoger colores.  
	**text="#99AABB"**: Cambia el color al texto.  
	**link="#99AABB"**: Cambia el color a los links de la web.  
	**vlink="#99AABB"**: Cambia el color de los links que ya fueron usados en la página (visited link).  
	
### Etiquetas del interior de BODY

Las etiquetas del interior de BODY se pueden clasificar en etiquetas para **texto**, para **listas**, para **tablas**, para **multimedia** (de estas solo imágenes), para **formularios** y para **dividir la web por secciones**.  
**1. De texto**: Crean titulares, links, distintos tipos de fuentes, tamaños y colores, ayudan a dividir el texto por parrafos...  
**2. De listas**: Para crear listas de elementos de forma ordenada o desordenada, indicandando que caracteres se utilizarán para crear dicha lista.  
**3. De tablas**: Para crear tablas de ciertos tamaños, colores, líneas divisorias, etc.  
**4. De multimedia**: Para incluir archivos de audio, video y fotografía.  
**5. Para formularios**: Para recoger información de los usuarios.  
**6. De división por secciones**: Hay determinadas etiquetas que no muestran ningún contenido, si no que ayudan al desarrollador web como dividir la página para que sea más fácil de editarla y crear cambios en ella, estas etiquetas pueden ser los DIV, HEADER, NAV, SECTION, ASIDE, ARTICLE, FOOTER, FIGURE o FIGCAPTION.  

#### Etiquetas de texto y sus atributos

- **Titulares**: Para se usa la etiqueta **\<hN>...\</hN>**, donde se sustituye la N por un número entre el uno y el seis, siendo el H1 el más grande y el H6 el más pequeño. A la hora de hacer titulares se recomienda usar una única vez el H1 por temas de SEO.

	- **Atributos de los titulares**:  
	**align="A"**: Sustituyendo la A por **right**, **left** o **center**, según donde queramos que esté alineado el títular.  
	
- **Párrafos**: Para crear los párrafos se usa la etiqueta **\<p>...\<p>**, el texto va entre estas dos etiquetas, cuando se cierra la etiqueta, el texto da un salto de línea para saltar a un nuevo párrafo.  

	- **Atributos de los párrafos**:  
	**align="A"**: Tiene la misma función que con los titulares, se puede sustituir la A por **right**, **left**, **center** y también por **justify**, esta nueva forma para alinear el texto es el "justificado" que procura no dejar espacios en blanco al principio ni al final de las líneas.  
	
- **Saltos de línea**: La etiqueta \<br/> da un salto de línea de la misma forma que si pulsaramos la tecla ENTER, se puede usar en el interior de los párrafos para crear saltos de línea sin dividir el bloque P.  

- **Barra horizontal**: Crea una barra horizontal que se puede utilizar para separar párrafos y hacer la página más estética.

	- **Atributos de la barra horizontal**:  
	**color="C"**: Le da un color sustituyendo la C por un color en inglés o por su nombre en sistema hexadecimal usando la almohadilla.  
	**align="A"**: Alinea la barra sustitutyendo por **right**, **left** o **center**.  
	**noshade**: Este atributo al ponerlo hace que la barra se vea lisa, eliminando el efecto tridimensional que se crea por defecto.
	**width="W"**: Modifica la anchura de la barra, poniendo un número de pixeles fijo para todas las pantallas o un porcentaje para que se acomode a cada pantalla.  
	**size="S"**: Cambia la altura de la barra, de la misma forma que con la anchura, se puede poner un número fijo de pixeles o un porcentaje, aunque en las alturas es recomendable **no usar** porcentajes.  
	
- **Dar formato al texto**: Dar formato al texto significa cambiar la fuente, el tamaño de las letras o el color, y para ello se utiliza la etiqueta **\<font>...\</font>**. Esta etiqueta se puede usar para modificar cualquier tipo de texto, desde titulares, a párrafos enteros o fragmentos de estos.  

	- **Atributos de FONT**:  
	**face="F"**: Cambia la fuente del texto por la fuente que le indiquemos (Comic Sans MS, Arial, Courier...).  
	**color="C"**: Cambia el color de texto que esté marcando, se puede poner en inglés o hexadecimal con con la almohadilla delante.  
	**size="S"**: Cambia el tamaño de la letra por el que le asignemos, también se puede aumentar o reducir en un número determinado de puntos que le asignemos para que el tamaño cambie dinámicamente en función del tamaño de fuente predeterminado que tenga la persona que habra la página. Esto se puede hacer poniendo +2 o -2, o el número de puntos que queramos aumentar o disminuir la fuente.  
	
- **Negrita, cursiva y subrayada**: Para aplicar alguno de estos formatos basta con poner, **\<b>bold\</b>** para negrita, **\<i>italic\</i>** para cursiva,**\<u>underlined\</u>** para subrayado, **strong** hace lo mismo que **b** y **em** lo mismo que **i**, solo que tienen un signigicado distinto para el documento. Estas etiquetas se pueden usar a la vez pero se recomienda hacerlo de forma ordenada.  

- **Links o enlaces**: Los links o enlaces son un elemento de la página que hace que podamos navegar entre varias webs o a través de la propia página con solo hacer clic en determinados links. Un link se crea con la etiqueta **\<a>...\</a>** y el texto que va entre las etiquetas será el enlace.  

	- **Atributos de los links**:  
	**href="H"**: Sustituyendo la H por una URL de Internet o una dirección de una carpeta si la página está en el localhost, indicará el destino de ese link.  
	**name="N"**: Se utiliza para hacer un ancla, se le asigna un nombre a la línea, palabra o texto que sea, para poder ir directamente al lugar del documento en el que esté situada esta ancla desde el link correspondiente. Para hacer que un enlace te lleve a un sitio estpecífico hay que poner una almohadilla antes del nombre del ancla. Por ejemplo: En una misma página (<a href="#indice">Vuelta al índice</a>), y un link que te lleva a un ancla sería (<a href="https://miweb.com/index#indice">Vuelta al índice<a/>).  
	**target="_T"**: Indica de que forma se abrirá el link, sustituyendo la T (la **_** es obligatoria ponerla) por **blank** se abrirá en una pestaña nueva y poniendo **self** se abrirá en la misma pestaña que en la que abrimos el enlace.  
	
#### Las listas y sus atributos
Existen tres tipos de listas, ordenadas, desordenadas y de definición, las primeras siguen un orden llevado por números decimales, números romanos en minúculas o mayúsculas, leras en minúscula o mayúscula... Mientras que las listas desordenadas no llevan ningún tipo de caracter que te indique que posición de la lista estamos, se marca con un punto, un cuadrado, etc. Las listas de definición se usan para definir palabras.  

- **Listas ordenadas**: Estas siguen un orden, y para indicar que queremos este tipo de lista lo haremos con la etiqueta **\<ol>\</ol>** de *ordered list*.  

	- **Atributos de las listas ordenadas**:  
	**type="T"**: Indica con que tipo de caracter queremos que marcar el orden. *A* con letras mayúsculas, *a* con letras minúsculas, *1* con número decimales, *I* con números romanos en mayúsculas e *i* con número romanos en minúculas.  
	**start="S"**: Indica con número en de la lista quieres empezar.  
	**reversed**: Con este atributo indicamos que es una lista en orden inverso.  
	
	- Para crear un elemento de la lista se usa la etiqueta **\<li>...\</li>**.  
	
- **Listas desordenadas**: No están enumeradas, en su lugar llevan un signo que identifica a cada elemento de la lista. Se hacen con la etiqueta **\<ul>...\</ul>** de *unordered list*.  

	- **Atributos de las listas desordenadas**:  
	**type="T"**: Indica con que forma se designará cada elemento de la lista. Sus valores pueden ser **circle**, **square** o **disc**.  
	
	- Para crear un elemento de la lista se usa la etiqueta **\<li>...\</li>**.  
	
- **Listas de definición**: Se usan para definir términos, palabras, expresiones, etc. Para indicar que vas a hacer una lista de definición se usa la etiqueta **\<dl>...\</dl>**.  

	- **Término a definir**: Para indicar la palabra que vamos a definir se usa la etiqueta **\<dt>...\</dt>**.
	- **La definición**: La definición se hace con la etiqueta **\<dd>...\</dd>**, que se indenta automáticamente.  
	
#### Las tablas y sus atributos

Las tablas están constituidas por filas y columnas, en las que si no indicamos ninguna medida es el propio navegador el que se encarga de ajustar las celdas en función del contenido de estas, una tabla también puede llevar incluido un título pero es opcional.  

- **La tabla**: Para indicar que lo que vas a escribir pertenece a una tabla se usa la etiqueta **\<table>...\</table>**.  

	- **Atributos de TABLE**:  
	**border="B"**: Se debe poner un número para definir el ancho del borde de la tabla, ya que por defecto el borde vale 0 y no se muestra.  
	**cellspacing="C"**: Se debe poner un número que definirá la distancia entre dos casillas de la tabla.  
	**cellpadding="C"**: Se debe poner otro número, solo que en este caso indica la distacia que hay desde el borde de la casilla hasta el contenido de la misma.  
	**width="W"**: Poniendo un número o porcentaje se designa el ancho de la tabla.  
	**heigth="H"**: Poniendo un número o porcentaje se designa la altura de la tabla, aunque en las alturas es recomendable no utilizar los porcentajes.  
	**bgcolor="B"**: Se pone un color en inglés o en hexadecimal para poner color a toda la tabla.  
	**align="A"**: Alinea la tabla a la izquierda, al centro o a la derecha, según le pongamos **left**, **center** o **right**.  
	
- **El título**: Para poner un título a la tabla se utiliza la etiqueta **\<caption>...\</caption>**, poniendo entre las dos etiquetas el título que le queramos poner a la tabla.  

	- **Atributos de CAPTION**:  
	**align="A"**: CAPTION se puede alinear en la parte superior o inferior de la tabla, poneiendo **top** para la parte superior o **bottom** para la parte inferior.  
	
- **Las filas o tuplas**: Para definir una fila se utiliza la etiqueta **\<tr>...\</tr>**, en la que en su interior se alojarán las etiquetas que definirán la cantidad de celdas que habrá.  

	- **Atributos de TR**:  
	**align="A"**: Establece la alineación de los elementos de esa tupla hacia el lado que designemos con **left**, **right** o **center**.  
	**valign="V"**: Establece una alineación vertical de los elementos siendo los posibles valores **top** de arriba, **middle** al centro y **bottom** abajo.  
	**bgcolor="B"**: Asigna un color a la tupla sobrescribiendo al color que se pudiera designar en la etiqueta de TABLE.  
	**height="H"**: Poniendo un número se define la altura de la fila.  
	
- **Las celdas o casillas**: Para establecer una o varias celdas dentro de una fila se utiliza la etiqueta **\<td>...\</td>** o si lo que va dentro es como si fuera un titular y queremos que vaya en negrita usaremos la etiqueta **\<th>...\</th>**.  

	- **Atributos de TD y TH**:  
	**align="A"**: Se usa para escoger a que lado se alinerá dicha celda, podemos usar **left**, **center** o **right**.  
	**valign="V"**: Es el alineamiento vertical pudiendo alinearse hacia **top**, **middle** y **bottom**.  
	**bgcolor="B"**: Con este atributo se puede escoger el color de la celda, teniendo preferencia sobre el de la etiqueta TABLE y el de su tupla TR.  
	**width="W"**: Si en las tuplas podíamos escoger el alto de cada fila, en las celdas podemos escoger un ancho para cada una, además de poder poner un porcentaje que será relativo a la tabla.  
	**nowrap**: Hace que el texto de una celda no se pueda dividir en varias líneas, por lo que aparecerá en una única línea.  
	**rowspan="R"**: Solo se puede aplicar a las celdas y significa *expadir fila*, por lo que indicandole un número, esa casilla pasará a ocupar el número de celdas que se le indiquen siempre hacia abajo.  
	**colspan="C": Si el otro se expandía a través de las filas, este se expande a través de las columnas siempre hacia la derecha.  
	
También se pueden agrupar las distintas filas de una tabla con las etiquetas **\<thead>...\</thead>** para la cabecera de la tabla, **\<tbody>...\</tbody>** para lo que es el cuerpo de la tabla y **\<tfoot>...\</tfoot>** para el pie de la tabla. A estas tres posibles agrupaciones se le pueden aplicar todas las modificaciones de los *align*, los *valign*, los *bgcolor* y el *height*, es decir, todos los atributos pertenecientes a las tuplas de la etiqueta TR.  

#### Los archivos multimedia

- **Las imágenes**: Entre todos los recursos multimedia, las imágenes son las más usadas y se ponen con la etiqueta **\<img />**.  

	- **Los atibutos de IMG**:  
	**src="S"**: Este atributo es OBLIGATORIO, ya que con el definimos de donde sale la imágen que empleamos, puede ser una dirección absoluta o relativa del ordenador o una dirección de Internet.  
	**alt="A"**: Con el podemos definir un texto que acompañará a la imágen que estamos definiendo con *src*.  
	**width="W"**: Podemos asignarle un ancho fijo poniendo los pixeles o con un porcentaje.  
	**height="H"**: Y con este atributo se designa una altura, aunque es recomendable no utilizar los porcentajes.  
	**usemap="#U"**: Este atributo se utiliza para usar el mapeado que se define con la etiqueta MAP, la almohadilla es obligatoria ponerla, y si el mapeado pertenece al de otra página se pondrá la ruta del mapa con la almohadilla y el nombre al final.  
	
- **El mapeado de imágenes**: Se utiliza para crear links sobre las imágenes o parte de estas con la etiqueta **\<map>...\</map>**.  

	- **Atributos de MAP**:  
	**name="N"**: Designa un nombre al mapeado que se usará en el atributo *usemap* de las imágenes.  
	
- **El área del mapaeado**: Para designar una zona o zonas que tendrán enlaces a lo que nosotros queramos se usa la etiqueta **\<area>...\</area>** dentro de MAP.  

	- **Atributos de AREA**:  
	**shape="S"**: Define la figura del mapeado **rect** para rectágulos o cuadrados, **poly** para otros polígonos (triángulos, rombos, pentagonos,etc) o **circle** para círculos entre otros.  
	**coords="C"**: En este atributo se difinen las coordenadas X e Y de cada punto. Para *rect* se marca una esquina y su opuesta (por ejemplo, la superior derecha y la inferior izquierda), para *poly* se marcan todas las esquinas del polígono yendo por orden, y para *circle* se marca el centro y el radio del círculo.  
	**href="H"**: Establece la dirección del enlace a la que llevará esa sección del mapeado.  
