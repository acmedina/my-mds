# Diseño de Páginas Web en HTML y Wordpress

## Índice General
1. [HTML](#html-hyper-text-markup-language)
1. [CSS](#css-cascading-style-sheet)
1. [WordPress](#wordpress)

# HTML Hyper Text Markup Language
**(Lenguaje de Marcado de Hiper Texto)**

![HTML](http://bextlan.com/img/para-cursos/html5-logo.png)

## Índice HTML
1. [Estructura y Contenido](#estructura-y-contenido)
1. [Etiquetas HTML](#etiquetas-html)
1. [Semántica](#semántica)
1. [Estructura Básica HTML5](#estructura-básica-html5)
1. [Más Info](#más-info)

**[⬆ regresar al índice general](#diseño-de-páginas-web-en-html-y-wordpress)**


## Estructura y Contenido

* Lenguaje de marcado basado en etiquetas y atributos, nos define estructura y contenido
* El contenido es el Rey
* Planear bien nuestra estructura de HTML (uso de etiquetas)
* Trabajar la semántica
* La semántica de nuestras etiquetas la define el contenido y su distribución
* Los motores de búsqueda son ciegos, si tu contenido esta bien estructurado, tu contenido será bien posicionado

**[⬆ regresar al índice HTML](#html-hyper-text-markup-language)**


## Etiquetas HTML

[Tabla periódica de las etiquetas HTML](http://zqsmm.qiniucdn.com/data/20110511083224/index.html)
![Tabla de las Etiquetas de HTML](http://bextlan.com/img/para-cursos/periodic-table.png)

**[⬆ regresar al índice HTML](#html-hyper-text-markup-language)**


## Semántica

La semántica es sólo una de las 8 implementaciones de [HTML5](https://www.w3.org/html/logo/)

Con las etiquetas semánticas mejoramos la definición de nuestro contenido, es más entendible tanto para humanos como para máquinas(algoritmos de buscadores)

Recuerda que las etiquetas semánticas no tienen una posición fija en el layout, quien determina la estructura es el contenido

### Etiquetas semánticas y estructurales

* **`<section>`**: Contenido genérico estructurado
* **`<article>`**: Contenido estructural distribuible de manera independiente
* **`<aside>`**: Contenido secundario relacionado o que acompaña o complementa a otro
* **`<header>`**: Contenido introductorio suele tener elementos de navegación y encabezados (h1...h6)
* **`<footer>`**: Sección que contiene información acerca del documento o página
* **`<nav>`**: Sección relativa a enlaces dentro del documento o página
* **`<main>`**: Contenido principal
* **`<figure>`**: Sección de contenido visual, múltiples medios
* **`<figcaption>`**: Leyenda o pié relativo al contenido visual de FIGURE, uno FIGCAPTION por cada FIGURE, puede contener semántica

### Ejemplo de semántica HTML5

![Semántica HTML5](http://bextlan.com/img/para-cursos/semantic-html5.jpg)

**[⬆ regresar al índice HTML](#html-hyper-text-markup-language)**


## Estructura Básica HTML5
```HTML
<!DOCTYPE html>
<html lang="es">
<head>
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<meta charset="UTF-8">
	<title>Título de mi documento, este deberá ser único max 65 caracteres</title>
	<meta name="description" content="Breve descripción de lo que los usuarios 
	encontrarán en este documento, deberá ser única max 156 caracteres">
	<link rel="stylesheet" href="estilos.css">
</head>
<body>
	<h1>Estructura de Documento HTML5</h1>
	<!-- 
		AQUÍ EL CONTENIDO HTML
		Esto es un comentaerio HTML
	-->
	<script src="codigos.js"></script>
</body>
</html>
```

**[⬆ regresar al índice HTML](#html-hyper-text-markup-language)**


## Más Info
* [Guía de Referencia HTML en MDN](https://developer.mozilla.org/es/docs/Web/HTML)
* [Introducción a HTML](http://librosweb.es/libro/xhtml/)
* [Guía de Buenas Prácticas en Código Front end](http://mdo.github.io/code-guide/)
* [La dieta del Navegador](https://browserdiet.com/es/)
* [Can I Use](http://caniuse.com/)

**[⬆ regresar al índice HTML](#html-hyper-text-markup-language)**


# CSS Cascading Style Sheet
**(Hojas de Estilo en Cascada)**

![CSS](http://bextlan.com/img/para-cursos/css-logo.jpg)

## Índice CSS
1. [Sintaxis](#sintaxis)
1. [Selectores](#selectores)
1. [Unidades de Medida](#unidades-de-medida)
1. [Colores](#colores)
1. [Tipografías](#tipografías)
1. [Características CSS3](#características-css3)
1. [Prefijos Navegadores](#prefijos-navegadores)
1. [Modelo de Caja](#modelo-de-caja)
1. [Posicionamiento](#posicionamiento)
1. [Visualización](#visualización)
1. [Técnicas de Maquetación](#técnicas-de-maquetación)
1. [Componentes Modulares](#componentes-modulares)
1. [Patrones de Diseño](#patrones-de-diseño)
1. [Frameworks](#frameworks)

**[⬆ regresar al índice general](#diseño-de-páginas-web-en-html-y-wordpress)**


## Sintaxis
Lenguaje de Presentación basado en reglas con una sintaxis de atributo valor

Provee presentación (diseño) al contenido HTML

Su principal objetivo es separar el contenido (HTML) de su presentación (CSS)

~~~~~~~~~~~~~~
selector {
    atributo-1: valor-1;
    atributo-2: valor-2;
    ...
    atributo-n: valor-n;
}
~~~~~~~~~~~~~~

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Selectores
Elemento(s) al que se le aplican reglas CSS

### Selectores Básicos:
* **De Etiquetas** `p { ... }`
* **Identificadores** `#menu { ... }`
* **Clases** `.item { ... }`
* [Más info](http://librosweb.es/libro/css/capitulo_2.html)

### Selectores Avanzados
* **Universal** `* { ... }`
* **Descendiente (espacio en blanco)** `.menu a { ... }`
* **de Hijos** `.menu > li { ... }`
* **de Hermanos** `section ~ article { ... }`
* **Adyacentes** `h1 + h2 { ... }`
* **de Atributos** `input[type="text"] { ... }`
* [Más Info](http://librosweb.es/libro/css_avanzado/capitulo_3.html)
    
### Pseudo-selectores
Nos ayudan a aplicar estilos especiales a nuestros elementos HTML, dependiendo de su contexto, posición o estado

Existen 2 tipos:
* Pseudo-clases
* Pseudo-elementos

#### Pseudo-clases
* **Estatus de Enlaces** `:link :visited`
* **Interacciones del Usuario** `:active :hover :focus`    
* **Elementos de Formularios** `:checked :disabled :in-range :invalid :out-of-range :required :target :valid`
* **Posición del Elemento** `:first-child :first-of-type :last-child :last-of-type :nth-child() :nth-last-child() :nth-of-type() :only-child :only-of-type :default`
* **CSS3** `:dir() :empty :first :fullscreen :indeterminate :lang() :left :not() :optional :read-only :read-write :right :root :scope`
* [Más info](https://css-tricks.com/examples/nth-child-tester/)

#### Pseudo-elementos
* **`::after { content:" " }`**
* **`::before { content:" " }`**
* **`::first-letter`**
* **`::first-line`**
* **`::selection`**

### Especificidad
Es lo que determina que estilo será el que acabará aplicandose a un elemento determinado

Cuando a un elemento se le aplica más de un selector con reglas que actúan sobre la misma propiedad, es la especificidad la encargada de resolver este conflicto

A grandes rasgos podemos ordenar los diferentes tipos de selectores de menor a mayor peso específico de la siguiente manera:

1. Selectores de elemento
1. Selectores contextuales
1. Clases
1. IDs

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Unidades de Medida
* **Absolutas** `px, pt, pc, cm, mm, in`
* **Relativas**
    * **al Contenedor** 
        * `% (Porcentajes)`
    * **a la Tipografía**
        * `em` basada en la anchura de la letra M del contenedor
        * `ex` basada en la altura de la letra X del contenedor
        * `rem` es el em del elemento raiz (html)
    * **al Viewport**
        * `vw` anchura del viewport
        * `vh` altura del viewport
        * `vmax` entre vw y vh toma el que tenga mayor valor
        * `vmin` entre vw y vh toma el que tenga menor valor

### Equivalencias entre unidades
* **`100% = 1em = 16px = 12pt`**
* [pxtoem](http://pxtoem.com/)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Colores
Sistemas de Colores:
* **CMYK**: Medios Impresos
* **RGB**: Medios Digitales

En HTML el RGB se maneja en código hexadecimal
* Base 16
* Dígitos del 0-9 y de la A-F
* 6 dígitos, una pareja por cada canal de color
* [HTML Color Codes](http://html-color-codes.info/)

![Colores en HTML](http://bextlan.com/img/para-cursos/colores-hexadecimal.png)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Tipografías
* Locales:
    * Con [@font-face](http://caniuse.com/#search=font-face) y [.woff](http://caniuse.com/#search=woff)
    * [Convertidor de Fuentes](http://www.fontsquirrel.com/tools/webfont-generator)

* Externas:
    * [Google Fonts](https://www.google.com/fonts)
    
* Icónicas
    * [Font Awesome](http://fortawesome.github.io/Font-Awesome/)
    * [IcoMoon](https://icomoon.io/)
    * [FlatIcon - Buscador de Íconos](http://flaticon.com/)
    * [Fontello - Generador de Fuentes Icónicas](http://fontello.com/)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Características CSS3
* [Bordes, colores RGBA, fuentes tipográficas, unidades relativas, sombras y gradientes](http://www.youtube.com/watch?v=p-ZjVEhMt2U)
* [Ajuste de texto, texto en columnas, tamaño de caja, fondos múltiples, área, origen y tamaño de fondo](http://www.youtube.com/watch?v=QYOujpsVvXE)
* [Transformaciones 2D y 3D, transiciones y animaciones](http://www.youtube.com/watch?v=yj93AWX0P_k)

![CSS](http://bextlan.com/img/para-cursos/header-css3.jpg)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Prefijos Navegadores
Cuando los navegadores soportan parcialmente un atributo CSS en ocasiones es necesario aplicar los prefijos:

* **`-ms-`** para Internet Explorer y Edge
* **`-moz-`** para Firefox
* **`-webkit-`** para Chrome, Safari, Opera, iOS y Android Browsers

#### Ejemplo
    -ms-border-radius: 20px;
    -moz-border-radius: 20px;
    -webkit-border-radius: 20px;
    border-radius: 20px;

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Modelo de Caja
El modelo de caja o "**box model**" es una de las característica más importante de CSS, ya que condiciona el diseño de la web; hace que todos los elementos de un documento HTML se representen mediante cajas rectangulares. 

CSS controla el aspecto de todas las cajas (contenedores), permite definir la altura y anchura de cada caja, el margen existente entre cajas y el espacio de relleno interior que muestra cada una; además controla la forma en la que se visualizan pero la mayoría no muestran ningún color de fondo ni borde, no son visibles a simple vista

### Partes del modelo de caja:
1. **Contenido**: `content`
1. **Relleno**: `padding`
1. **Borde**: `border`
1. **Imagen de fondo**: `background-image`
1. **Color de fondo**: `background-color`
1. **Margen**: `margin`

![Modelo de Caja](http://bextlan.com/img/para-cursos/modelo-caja-css.jpg)

### Propiedades importantes del modelo de caja:
* **Border**: Borde, es la linea que delimita los elementos divide el margin del padding
* **Padding**: Relleno, distancia interna que hay entre los márgenes del elemento(top,right,bottom,left) y su contenido
* **Margin**: Margen, distancia externa que hay entre los elementos y los márgenes del documento u otros elementos (top,right,bottom,left)
* [Más info](http://librosweb.es/libro/css/capitulo_4.html)

#### Ejemplos de `border`:
    border-width: thin | thick | medium | 10px | 1em;
    border-style: solid | dashed | dotted;
    border-color: #F60 | orange;
    border: thin solid #F60; (shorthand)

#### Ejemplos de `margin` y `padding`:
* 4 márgenes / bordes
* top / bottom = verticales
* left / right = horizontales
* 1 valor = Se aplica a los 4 lados
~~~~~~~~~~~~~~~~~~~~~~~~~~~
    margin: 1em;
    padding: 1em;
~~~~~~~~~~~~~~~~~~~~~~~~~~~
* 2 valores:
    * 1° es para top y bottom
    * 2° es para left y right
~~~~~~~~~~~~~~~~~~~~~~~~~~~
    margin: 1em 2em;
    padding: 0 1em;
~~~~~~~~~~~~~~~~~~~~~~~~~~~
* 3 valores:
    * 1° es para top
    * 2° es para left y right
    * 3° es para bottom
~~~~~~~~~~~~~~~~~~~~~~~~~~~
    margin: 1em auto 2em;
    padding: 2em 0 .5em;
~~~~~~~~~~~~~~~~~~~~~~~~~~~
* 4 valores: En sentido de las manecillas del reloj
    * 1° es para top
    * 2° es para right
    * 3° es para bottom
    * 4° es para left
~~~~~~~~~~~~~~~~~~~~~~~~~~~
    margin: 1em 3em 2em 0;
    padding: 2em 1em 0 .5em;
~~~~~~~~~~~~~~~~~~~~~~~~~~~
* Especificando cada lado
~~~~~~~~~~~~~~~~~~~~~~~~~~~
    margin-top | margin-right | margin-bottom | margin-left
    padding-top | padding-right | padding-bottom | padding-left
~~~~~~~~~~~~~~~~~~~~~~~~~~~

> **Nota**: Los atributos del modelo de caja (`border`, `margin` y `padding`) por defecto aumentarán el ancho (`width`) y alto (`height`) de la misma, es decir el [tamaño de caja](https://css-tricks.com/box-sizing/) (`box-sizing`)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Posicionamiento
* **Estático**: Es el que viene por defecto, un elemento detrás del otro
* **Relativo**: Se desplaza respecto de su posición original
* **Absoluto**: Se desplaza respecto de:
    * la posición del body del documento o 
    * del primer elemento padre relativo que tenga
* **Fijo**: Permite mantener fijo un elemento
* **Flotante**: Convierte un elemento en flotante desplazándolo hasta la zona más a la izquierda o más a la derecha de la posición en la que originalmente se encontraba
* **Pegajoso**: Posicionamiento experimental, permite que el elemento sea relativo o fijo dependiendo del area donde se visualiza
* [Más info](http://librosweb.es/libro/css/capitulo_5.html)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Visualización
* **Visibility:** Afecta la visualización del contenido de una caja
* **Display:** Afecta la visualización de la caja
    * **Tipos de Display Básicos**
        * **`block`:** Ocupa todo el ancho disponible
        * **`inline`:** Ocupa sólo el ancho requerido
        * **`none`:** Quita la caja de la visualización del documento

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Técnicas de Maquetación
* **`float: left | right;`**
    * [Más Info](http://librosweb.es/libro/css/capitulo_5/posicionamiento_flotante.html)
* **`display: inline-block;`**
    * [Puedo usarlo](http://caniuse.com/#search=inline-block)
    * [Más Info](https://www.w3.org/TR/2011/REC-CSS2-20110607/visudet.html)
* **`display: table;`**
    * [Puedo usarlo](http://caniuse.com/#search=table)
    * [Más Info](https://www.w3.org/TR/CSS21/tables.html)
* **`display: flex;`**
    * [Puedo usarlo](http://caniuse.com/#search=flex)
    * [Guía Completa de CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
    * [Más Info Propiedad Flex en CSS-Tricks](https://css-tricks.com/almanac/properties/f/flex/)
    * [Más Info W3C](https://www.w3.org/TR/css-flexbox/)
    * [Más Info MDN](https://developer.mozilla.org/es/docs/Web/CSS/CSS_Flexible_Box_Layout/Usando_las_cajas_flexibles_CSS)
* **`display: grid;`**
    * [Puedo usarlo](http://caniuse.com/#search=grid)
    * [Guía Completa de CSS-Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)
    * [Grid by Example](http://gridbyexample.com/presentations/)
    * [Más Info W3C](https://www.w3.org/TR/css-grid-1/)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Componentes Modulares
> “It's a repeating visual pattern, that can be abstracted into an independent snippet of HTML, CSS and possibly JavaScript.”
> > [Nicole Sullivan](https://vimeo.com/72759139)

* Son un fragmento de la interfaz que cumple una única función
* Son independientes, tanto de su contexto como del resto de componentes
* Son reutilizables
* Son autocontenidos, no filtran estilos a otros componentes

![Componentes Modulares](http://bextlan.com/img/para-cursos/componentes-css.png)

### Atomic Design
* Metodología basada en: Átomos, Moléculas, Organismos, Plantillas y Páginas
* [Tabla periódica de las etiquetas HTML](http://zqsmm.qiniucdn.com/data/20110511083224/index.html)
* [Artículo](http://bradfrost.com/blog/post/atomic-web-design/)
* [Slides](http://es.slideshare.net/bradfrostweb/atomic-design)
* [Libro](https://github.com/bradfrost/atomic-design)
* [Laboratorio de Patrónes](http://patternlab.io/)
* [Ejemplos](http://demo.patternlab.io/)
![Atomic Design](http://bextlan.com/img/para-cursos/atomic-design.png)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Patrones de Diseño
Los patrones de diseño son la base para la búsqueda de soluciones a problemas comunes en el desarrollo de software y otros ámbitos referentes al diseño de interacción o interfaces.

Un patrón resulta ser una solución a un problema. Para que una solución sea considerada patrón debe:
* Comprobar su efectividad resolviendo problemas similares
* Ser reutilizable, lo que significa que es aplicable a diferentes problemas en distintas circunstancias

**¿Por qué usar Patrones en CSS?**
* Construimos sistemas, no páginas
* Necesidad de modularidad
* Mejora flujo de trabajo
* Ya han sido probados y validados
* Si trabajamos en equípo mantiene el órden
* Promueven la filosofía DRY **(Don't Repeat Yourself)**

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


## Frameworks
* [960 Grid System](http://960.gs/)
* [Bootstrap](http://getbootstrap.com/)
* [Foundation](http://foundation.zurb.com/)
* [Skeleton](http://getskeleton.com/)
* [Pure CSS](http://purecss.io/)
* [jQueryMobile](https://jquerymobile.com/)
* [Materialize](http://materializecss.com/)
* [MUI](https://www.muicss.com/)
* [Semantic UI](http://semantic-ui.com/)
* [Flexbox Grid](http://flexboxgrid.com/)
* [Responsimple](http://jonmircha.github.io/responsimple/) :heart_eyes:
* [Comparativas entre Frameworks](http://responsive.vermilion.com/compare.php)

**[⬆ regresar al índice CSS](#css-cascading-style-sheet)**


# WordPress
![WordPress](http://bextlan.com/img/para-cursos/wordpress.jpg)


## Índice WordPress
1. [Slides](http://bextlan.com/slides/wordpress/)
1. [Links importantes sobre WP](#links-importantes-sobre-wordpress)
1. [Taxonomía de WP](#taxonomía-de-wordpress)
1. [Instalación de WP](#instalación-de-wordpress)
1. [Temas en WP](#temas-en-wordpress)
1. [The Loop](#the-loop)
1. [Plantillas en WP](#plantillas-en-wordpress)
1. [Hooks en WP](#hooks-en-wordpress)
1. [Plugins en WordPress](#plugins-en-wordpress)
1. [Widgets en WordPress](#widgets-en-wordpress)
1. [Importación / Exportación de WP](#importación--exportación-de-wordpress)

**[⬆ regresar al índice general](#diseño-de-páginas-web-en-html-y-wordpress)**


## Links importantes sobre WordPress
* [WordPress.org](http://wordpress.org)
* [WordPress.com](http://wordpress.com)
* [WordPress.org en Español](http://es.wordpress.org)
* [WordPress.com en Español](http://es.wordpress.com)
* [Empezando con WordPress](https://codex.wordpress.org/es:Getting_Started_with_WordPress)
* [Codex WordPress](http://codex.wordpress.org/)
* [Developers WordPress](https://developer.wordpress.org/)
* [Embeds](https://codex.wordpress.org/Embeds)
* [Roles y Capacidades en WordPress](https://codex.wordpress.org/es:Roles_y_Capacidades#Subscriber)
* [Tabla de Roles y Capacidades en WordPress](https://codex.wordpress.org/Roles_and_Capabilities#Capability_vs._Role_Table)
* [Buenas Prácticas de PHP en WordPress](https://make.wordpress.org/core/handbook/coding-standards/php/)
* [Recuperar passwords de Usuarios WordPress](http://www.wpbeginner.com/beginners-guide/how-to-reset-a-wordpress-password-from-phpmyadmin/)
* [Herramienta para resetear passwords de Usuarios WordPress](http://pajhome.org.uk/crypt/md5/)
* [Curso de WordPress en Bextlán](https://www.youtube.com/playlist?list=PLvq-jIkSeTUZDOcKsQz79wnYlTvmAdLkj)

**[⬆ regresar al índice WordPress](#wordpress)**


## Taxonomía de WordPress
Es la forma en como WP estructura el contenido de nuestro sitio y lo hace a través de:
* Categorías
* Etiquetas
* Entradas
* Páginas

### Categorías (Clasifican el contenido)
Son la tabla de contenidos de tu sitio web. Son utilizadas para agrupar tus contenidos y mantener una clasificación.

Deben ser la base de la organización ya que conservan un orden jerárquico, y podemos generar sub-categorías.

### Etiquetas (Palabras clave, para búsquedas internas)
Se utilizan como microdatos que describen detalles específicos del contenido.

Sirven como keywords para el SEO de nuestras publicaciones.

### Entradas (Publicaciones)
Es el contenido final de nuestras páginas o secciones, pueden tener asociadas más de una categoría, si no le especificamos una, se guardaran como parte de la categoría que trae WP por defecto "Sin Categoría". Podemos agregarles tantas etiquetas como sean necesarias.

### Páginas (Contenido estático)
Son contenidos que difícilmente van a cambiar, por ejemplo la sección de contacto o acerca, no se pueden asociar a categorías ni a etiquetas

### Ejemplos de Taxonomías:

	Taxnomía de Sitio de Perros
		Home(loop)
		El Perro(p)
		Comportamiento(p)
		Sentidos(p)
		Videos(p)
		Razas(c)
		En esta categoría podrás encontrar una clasificación de los perros, basada en su tamaño.
			Gigantes(sc)
			Esta categoría esta destinada a los perros gigantes.
				Bobtail(e)
				Dogo de Burdeos(e)
				Gran Danés(e)
				Mastín Napolitano(e)
				San Bernardo(e)
				Terranova(e)
			Grandes(sc)
			Esta categoría esta destinada a los perros grandes.
				Boxer(e)
				Dálmata(e)
				Dóberman(e)
				Husky Siberiano(e)
				Labrador(e)
				Pastor Alemán(e)
			Medianos(sc)
			Esta categoría esta destinada a los perros medianos.
				Basset Hound(e)
				Beagle(e)
				Border Collie(e)
				Bull Dog(e)
				Cocker Spaniel(e)
				Staffordshire Bull Terrier(e)
			Pequeños(sc)
			Esta categoría esta destinada a los perros pequeños.
				Bichón(e)
				Chihuahua(e)
				Pug(e)
				Schnauzer(e)
				Xoloitzcuintle(e)
				Yorkshire(e)
			Sin Raza(sc)
			Esta categoría esta destinada a los perros sin raza.
				Únicos(e)

	Taxonomía Sitio Bextlan v4
		Home (loop)
		Cursos (c)
			Responsive Design (e)
			jQuery (e)
			WordPress (e)
			Node.JS (e)
		Tutoriales (c)
			HTML5(e)
			JS(e)
			PHP(e)
			AS3(e)
			Vlog(e)
		Acerca (p)
		Servicios (p)
		FAQ's (p)
		Anualidad (p)

	Taxonomía Sitio mejorenvo.com
		Inicio (loop)
		Series(c)
			Temporadas (e)
		Películas(c)
			Película (e)
		FAQ(p)
		Manuales(p)
		Contacto(p)

	Taxonomía Sitio mundoheroes.net
		Home(loop)
		VideoClips(p)
		ReporteFallos(p)
		Series(c)
			Serie(e)
		Películas(c)
			Película(e)
		Comics(c)
			Comic(e)
		Marvel(et)
		DC Comics(et)
		Otras(et)

**[⬆ regresar al índice WordPress](#wordpress)**


## Instalación de WordPress

1. Descargar WordPress [http://es.wordpress.org/](http://es.wordpress.org/)
1. Descomprimir WordPress en la carpeta **xampp/htdocs/**
1. Crear una  BD en MySQL para nuestro WordPress desde [http://localhost/phpmyadmin](http://localhost/phpmyadmin)
1. Ejecutar la carpeta del sitio en el navegador **http://localhost/carpeta-sitio-wp**
1. Llenar la información de la instalación:
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion1.png)
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion2.png)
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion3.png)
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion4.png)
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion5.png)
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion6.png)
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion7.png)
![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion8.png)
1. Una vez instalado:
	* Para ver wp como user:
		* **http://localhost/carpeta-sitio-wp**
	* Para ver wp como admin:
		* **http://localhost/carpeta-sitio-wp/wp-admin**

**[⬆ regresar al índice WordPress](#wordpress)**


## Temas en WordPress
Un Tema WordPress es una colección de archivos que trabajan juntos para producir un interfaz gráfica con un diseño unificado para el sitio. Estos archivos se llaman archivos de plantilla

Un tema modifica el modo en que el sitio es mostrado, sin modificar el código fuente de WordPress

Los temas pueden incluir archivos de plantilla personalizados, archivos de imagen, hojas de estilo, scripts (.php o .js), así como cualquier otro archivo necesario

#### Archivos Básicos de un Tema:
* **index.php**	plantilla principal
* **style.css** hoja de estilos principal del tema
* **screenshot.png** imagen representativa del tema en el administrador de WP

#### Estructura Básica de un Tema
![Estructura Básica de un Tema en WP](http://bextlan.com/img/para-cursos/estructura-tema.png)

#### Links y Funciones Básicas de un Tema:
* [Temas](https://wordpress.org/themes/)
* [Theme Forest](http://themeforest.net/)
* [Función bloginfo()](https://codex.wordpress.org/Function_Reference/bloginfo)
* [Función get_header()](https://codex.wordpress.org/Function_Reference/get_header)
* [Función get_footer()](https://codex.wordpress.org/Function_Reference/get_footer)
* [Función get_sidebar()](https://codex.wordpress.org/Function_Reference/get_sidebar)
* [Función get_template_part()](https://codex.wordpress.org/Function_Reference/get_template_part)

#### Funciones de inclusión obligatorias:
Si queremos que nuestro tema permita el correcto funcionamiento de plugins de terceros, debemos activar las siguientes funciones de esta manera WordPress permite a los plugins imprimir información en el header o el footer

* [Función wp_head()](https://codex.wordpress.org/Plugin_API/Action_Reference/wp_head) debe colocarse antes de `</head>`
* [Función wp_footer()](https://codex.wordpress.org/Plugin_API/Action_Reference/wp_footer) debe colocarse antes de `</body>`

**[⬆ regresar al índice WordPress](#wordpress)**


## The Loop
**The Loop** es el código PHP usado por WordPress para mostrar las publicaciones

```php
if( have_posts() ):
	while( have_posts() ):
		the_post();
		//post info
	endwhile;
else:
	//no posts
endif;
```

#### Links y Funciones relacionados con The Loop
* [The Loop](https://codex.wordpress.org/The_Loop)
* [Función have_posts()](https://codex.wordpress.org/Function_Reference/have_posts)
* [Función the_post()](https://codex.wordpress.org/Function_Reference/the_post)
* [Función the_title()](https://codex.wordpress.org/Function_Reference/the_title)
* [Función the_permalink()](https://codex.wordpress.org/Function_Reference/the_permalink)
* [Función the_date()](https://codex.wordpress.org/Function_Reference/the_date)
* [Función the_time()](https://codex.wordpress.org/Function_Reference/the_time)
* [Función the_excerpt()](https://codex.wordpress.org/Function_Reference/the_excerpt)
* [Función the_category()](https://codex.wordpress.org/Function_Reference/the_category)
* [Función the_tags()](https://codex.wordpress.org/Function_Reference/the_tags)
* [Función the_author()](https://codex.wordpress.org/Function_Reference/the_author)
* [Función the_content()](https://codex.wordpress.org/Function_Reference/the_content)
* [Función rewind_posts()](https://codex.wordpress.org/Function_Reference/rewind_posts)
* [Función query_posts()](https://codex.wordpress.org/Function_Reference/query_posts)
* [Búsquedas Personalizadas en WP](http://www.anieto2k.com/2008/01/13/query_posts-personalizando-nuestros-blogs/)
* [Parámetros para Búsquedas Personalizadas](https://codex.wordpress.org/Class_Reference/WP_Query#Parameters)

**[⬆ regresar al índice WordPress](#wordpress)**


## Plantillas en WordPress
Son los archivos que nuestro tema va utilizando dependiendo del contenido solicitado, los cuales pueden ser:

* **index.php**	plantilla principal
	* **home.php**	plantilla del home del sitio
	* **archive.php** plantilla de categorías y etiquetas
		* **category.php** plantilla de categorías
		* **tag.php** plantilla de etiquetas
	* **singular.php** plantilla de entradas y páginas
		* **single.php** plantilla de entradas
		* **page.php** plantilla de páginas estáticas
	* **404.php** plantilla para error 404
	* **search.php** plantilla para búsquedas
	* **comments.php** plantillas para los comentarios
	* **author.php** plantillas para mostrar la página de autor
* Templates personalizados:
	* Podemos tener templates personalizados para: 
		* Categorías
		* Etiquetas
		* Páginas estáticas
	* Podemos crear templates personalizados por:
		* slug
		* id

![Estructura de carpetas de un Tema en WP](http://bextlan.com/img/para-cursos/plantillas-secciones-separadas.png)

#### Links y Funciones relacionados con Plantillas
* [Estructura de Archivos de un tema en WP](http://blog.eamexicano.com/wordpress/wordpress-tema/)
* [Jerarquía de Plantillas en WP](https://developer.wordpress.org/themes/basics/template-hierarchy/)
* [Plantillas de Categorías](https://codex.wordpress.org/Category_Templates)
* [Plantillas de Etiquetas](https://codex.wordpress.org/Tag_Templates)
* [Plantillas de Páginas](https://codex.wordpress.org/Pages#Page_Templates)
* [Plantilla de Página 404](https://codex.wordpress.org/Creating_an_Error_404_Page)
* [Función get_the_author_id()](http://codex.wordpress.org/get_the_author_id)
* [Función get_the_author_meta()](http://codex.wordpress.org/get_the_author_meta)
* [Función get_the_author_posts_url()](http://codex.wordpress.org/get_the_author_posts_url)
* [Función get_the_author_posts()](http://codex.wordpress.org/get_the_author_posts)
* [Función get_avatar()](http://codex.wordpress.org/get_avatar)
* [Gravatar](http://es.gravatar.com/)
* [Función comments_template()](https://codex.wordpress.org/Function_Reference/comments_template)
* [Función comment_form()](http://codex.wordpress.org/comment_form)
* [Función wp_list_comments()](http://codex.wordpress.org/wp_list_comments)
* [Función get_search_form()](https://codex.wordpress.org/Function_Reference/get_search_form)
* [Función get_search_query()](https://codex.wordpress.org/Template_Tags/get_search_query)

**[⬆ regresar al índice WordPress](#wordpress)**


## Hooks en WordPress
El archivo **functions.php**  es como una biblioteca personal de funciones, es una manera fácil de agregar o modificar el comportamiento por defecto de WordPress. Se comporta exactamente igual que un plugin, añadiendo características y funcionalidad a un tema, y se puede utilizar tanto para definir nuevas funciones PHP como para modificar las que ya incorpora WordPress, se dividen en:
* Filtros
* Acciones

#### Links y Funciones relacionados con Hooks
* [Glosario de WP](https://codex.wordpress.org/Glossary)
* [API de Plugin de WP](http://codex.wordpress.org/Plugin_API)
* [API de Hooks de WP](http://codex.wordpress.org/Plugin_API/Hooks)
* [Filtros de WP](http://codex.wordpress.org/Plugin_API/Filter_Reference)
* [Acciones de WP](http://codex.wordpress.org/Plugin_API/Action_Reference)
* [Función add_action()](https://codex.wordpress.org/Function_Reference/add_action)
* [Función add_filter()](https://codex.wordpress.org/Function_Reference/add_filter)
* [Función add_theme_support()](https://codex.wordpress.org/Function_Reference/add_theme_support)
* [Función the_post_thumbnail()](https://codex.wordpress.org/Function_Reference/the_post_thumbnail)
* [Función get_the_post_thumbnail()](https://codex.wordpress.org/Function_Reference/get_the_post_thumbnail)
* [Función register_nav_menus()](https://codex.wordpress.org/Function_Reference/register_nav_menus)
* [Función wp_nav_menu()](https://codex.wordpress.org/Function_Reference/wp_nav_menu)

**[⬆ regresar al índice WordPress](#wordpress)**

## [Plugins](https://wordpress.org/plugins/) en WordPress
* [Jetpack](https://wordpress.org/plugins/jetpack/)
* [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/)
* [WP Super Cache](https://wordpress.org/plugins/wp-super-cache/)
* [Contact Form 7](https://wordpress.org/plugins/contact-form-7/)
* [Comments Evolved for WordPress](https://wordpress.org/plugins/gplus-comments/)
* [WP PageNavi](https://wordpress.org/plugins/wp-pagenavi/)
* [Infinite Scroll](http://www.infinite-scroll.com/)
* [Max Mega Menu](https://wordpress.org/plugins/megamenu/)
* [Meta Box](https://metabox.io/)
* [Insert PHP](https://wordpress.org/plugins/insert-php/)
* [WP No Category Base](https://wordpress.org/plugins/wp-no-category-base/)
* [WP No Tag Base](https://wordpress.org/plugins/wp-no-tag-base/)

**[⬆ regresar al índice WordPress](#wordpress)**


## [Widgets](https://codex.wordpress.org/Widgets_API) en WordPress
* [Función register_sidebar()](https://codex.wordpress.org/Function_Reference/register_sidebar)	
* [Función dynamic_sidebar()](https://codex.wordpress.org/Function_Reference/dynamic_sidebar)

**[⬆ regresar al índice WordPress](#wordpress)**


## Importación / Exportación de WordPress
Esto sirve para ir del localhost al servidor en internet o viceversa

1. Respaldar todo WordPress (wp-admin,wp-includes,wp-content,archivos sueltos)
2. Cargar/Descargar el respaldo (FTP, SSH, Git)
3. Exportar en formato .sql la BD desde el phpMyAdmin
    * Considera que a veces phpMyAdmin no nos agrega la instrucción CREATE DATABASE y USE
4. Abrir el archivo .sql y reemplazar todas las rutas locales a las del servidor en internet o viceversa con ayuda del comando buscar y reemplazar de tu editor de código favorito
5. Modificar las rutas de las siguientes lineas del archivo .htaccess:
    * **RewriteBase**
    * **RewriteRule**

```htaccess
# BEGIN WordPress
<IfModule mod_rewrite.c>
    RewriteEngine On
    RewriteBase /perros/
    RewriteRule ^index\.php$ - [L]
    RewriteCond %{REQUEST_FILENAME} !-f
    RewriteCond %{REQUEST_FILENAME} !-d
    RewriteRule ./perros/index.php [L]
</IfModule>
# END WordPress
```

6. Modificar BD,USER,PWD y HOST MySQL en el archivo wp-config.php
7. Importar la BD en el destino y cargar el nuevo contenido

**Nota:**
* Si las estructuras de carpeta se respetan en el servidor y en el localhost, cuando haya nuevos cambios, sólo hay que hacer los pasos 2,3, 4 y 7. los demás sólo la primera vez.
* Para seguir con el curso usaremos el tema y la base de datos del sitio WordPress que podrán encontrar en el siguiente [repositorio](https://github.com/jonmircha/perros-inicial)

**[⬆ regresar al índice WordPress](#wordpress)**