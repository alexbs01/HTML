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
Las etiquetas del interior de BODY se pueden clasificar en etiquetas para texto, para listas, para tablas, para multimedia (de estas solo imágenes) y para formularios.
