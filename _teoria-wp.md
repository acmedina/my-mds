# WordPress

![WordPress](http://bextlan.com/img/para-cursos/wordpress.jpg)


## Índice

1. [Enlaces importantes sobre WP](#enlaces-importantes-sobre-wordpress)
1. [Taxonomía de WP](#taxonomía-de-wordpress)
1. [Cuenta en WordPress.com](#cuenta-en-wordpresscom)
1. [Instalación de WP](#instalación-de-wordpress)
1. [Importación / Exportación de WP](#importación--exportación-de-wordpress)
1. [Temas en WP](#temas-en-wordpress)
1. [The Loop](#the-loop)
1. [Plantillas en WP](#plantillas-en-wordpress)
1. [Hooks en WP](#hooks-en-wordpress)
1. [Plugins en WordPress](#plugins-en-wordpress)
1. [Widgets en WordPress](#widgets-en-wordpress)


## Enlaces importantes sobre WordPress

* [Slides](http://bextlan.com/slides/wordpress/)
* [WordPress.org](http://wordpress.org)
* [WordPress.com](http://wordpress.com)
* [WordPress.org en Español](http://es.wordpress.org)
* [WordPress.com en Español](http://es.wordpress.com)
* [WordPress.org en Español de México](https://es-mx.wordpress.org/)
* [Empezando con WordPress](https://codex.wordpress.org/es:Getting_Started_with_WordPress)
* [Codex WordPress](http://codex.wordpress.org/)
* [Developers WordPress](https://developer.wordpress.org/)
* [Embeds (Objetos Incrustados)](https://codex.wordpress.org/Embeds)
* [Roles y Capacidades en WordPress](https://codex.wordpress.org/Roles_and_Capabilities)
* [Buenas prácticas de código PHP en WordPress](https://make.wordpress.org/core/handbook/coding-standards/php/)
* [Recuperar passwords de usuarios en WordPress](http://www.wpbeginner.com/beginners-guide/how-to-reset-a-wordpress-password-from-phpmyadmin/)
* [Herramienta para resetear passwords de usuarios en WordPress](http://pajhome.org.uk/crypt/md5/)
* [Curso de WordPress en Bextlán](https://www.youtube.com/playlist?list=PLvq-jIkSeTUZDOcKsQz79wnYlTvmAdLkj)

**[⬆ regresar al índice](#Índice)**


## Taxonomía de WordPress

Es la forma en como WP estructura el contenido de nuestro sitio y lo hace a través de:

* Categorías **(Clasifican el contenido)**
* Etiquetas **(Palabras clave, para búsquedas internas)**
* Entradas **(Contenido dinámico)**
* Páginas **(Contenido estático)**

### Categorías

Son la tabla de contenidos del sitio web. Son utilizadas para agrupar los contenidos y mantener una clasificación. Deben ser la base de la organización ya que conservan un orden jerárquico, y podemos generar subcategorías.

### Etiquetas

Se utilizan como microdatos que describen detalles específicos del contenido. Sirven como keywords para el SEO de nuestras publicaciones.

### Entradas

Es el contenido final de nuestro sitio, pueden tener asociadas más de una categoría, si no le especificamos una, se guardaran como parte de la categoría que trae WP por defecto "Sin Categoría". Podemos agregarles tantas etiquetas como sean necesarias.

### Páginas

Son contenidos que difícilmente van a cambiar, por ejemplo la sección de contacto o acerca, no se pueden asociar a categorías ni a etiquetas.

**[⬆ regresar al índice](#Índice)**


## Cuenta en WordPress.com

![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-1.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-2.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-3.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-4.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-5.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-6.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-7.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-8.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-9.png)
![Creando cuenta en WordPress.com](http://bextlan.com/img/para-cursos/cuenta-wp-10.png)

**[⬆ regresar al índice](#Índice)**


## Instalación de WordPress

1. Descargar [WordPress](https://es-mx.wordpress.org/)
1. Descomprimir WordPress en la carpeta **xampp/htdocs/**
1. Es recomendable renombrar la carpeta wordpress por un nombre relacionado con el proyecto a desarrollar
1. Crear una  base de datos en MySQL para el nuevo proyecto en WordPress, lo puedes hacer desde [phpMyAdmin](http://localhost/phpmyadmin)
1. Buscar el archivo **wp-config-sample.php** y renombrarlo como **wp-config.php**
1. Abrir el archivo **wp-config.php** y editar los siguientes datos:
	```php
		define('DB_NAME', 'database_name_here');
		define('DB_USER', 'username_here');
		define('DB_PASSWORD', 'password_here');
		define('DB_HOST', 'localhost');
		define('DB_CHARSET', 'utf8');
		define('DB_COLLATE', '');

		define('AUTH_KEY',         'put your unique phrase here');
		define('SECURE_AUTH_KEY',  'put your unique phrase here');
		define('LOGGED_IN_KEY',    'put your unique phrase here');
		define('NONCE_KEY',        'put your unique phrase here');
		define('AUTH_SALT',        'put your unique phrase here');
		define('SECURE_AUTH_SALT', 'put your unique phrase here');
		define('LOGGED_IN_SALT',   'put your unique phrase here');
		define('NONCE_SALT',       'put your unique phrase here');

		$table_prefix  = 'wp_';
	```
1. Ejecutar la carpeta del sitio en el navegador **( http://localhost/carpeta-sitio-wp )**
1. Llenar la información de la instalación
	![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion1.png)
	![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion2.png)
	![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion3.png)
	![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion4.png)
	![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion5.png)
	![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion6.png)
1. Una vez instalado:
	* Para ver WP como usuario administrador:
		* **http://localhost/ruta-del-sitio/wp-login.php** o
		* **http://localhost/ruta-del-sitio/wp-admin**
		![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion7.png)
	* Para ver WP como usuario visitante:
		* **http://localhost/ruta-del-sitio**
		![Instalación de WordPress](http://bextlan.com/img/para-cursos/wp-instalacion8.png)

**[⬆ regresar al índice](#Índice)**


## Importación / Exportación de WordPress

Esto sirve para ir del localhost al servidor en internet o viceversa

1. Respaldar todo el proyecto WordPress ( wp-admin, wp-includes, wp-content, archivos sueltos )
1. Cargar o Descargar el respaldo vía FTP, SSH, Git, etc
1. Exportar en formato **.sql** la BD desde el phpMyAdmin
	* Considera que a veces phpMyAdmin no nos agrega la instrucción `CREATE DATABASE` y `USE`
1. Abrir el archivo **.sql** y reemplazar todas las rutas locales a las del servidor en internet o viceversa, con ayuda del comando buscar y reemplazar de tu editor de código favorito
1. Modificar las rutas de las siguientes lineas del archivo **.htaccess**:
	* **RewriteBase**
	* **RewriteRule**
	```htaccess
		# BEGIN WordPress
		<IfModule mod_rewrite.c>
			RewriteEngine On
			RewriteBase /carpeta-sitio-wp/
			RewriteRule ^index\.php$ - [L]
			RewriteCond %{REQUEST_FILENAME} !-f
			RewriteCond %{REQUEST_FILENAME} !-d
			RewriteRule ./carpeta-sitio-wp/index.php [L]
		</IfModule>
		# END WordPress
	```
1. Modificar **DB_NAME**, **DB_USER**, **DB_PASSWORD** y **DB_HOST** en el archivo **wp-config.php**
```php
	define('DB_NAME', 'database_name_here');
	define('DB_USER', 'username_here');
	define('DB_PASSWORD', 'password_here');
	define('DB_HOST', 'localhost');
```
1. Importar la BD en el destino y cargar el nuevo contenido

**Nota:**
* Si las estructuras de carpeta se respetan en el servidor y en el localhost, cuando haya nuevos cambios, sólo hay que hacer los pasos 2,3, 4 y 7. los demás sólo la primera vez.

**[⬆ regresar al índice](#Índice)**


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

**[⬆ regresar al índice](#Índice)**


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
* [Función get_the_title()](https://codex.wordpress.org/Function_Reference/get_the_title)
* [Función get_the_permalink()](https://codex.wordpress.org/Function_Reference/get_the_permalink)
* [Función get_the_date()](https://codex.wordpress.org/Function_Reference/get_the_date)
* [Función get_the_time()](https://codex.wordpress.org/Function_Reference/get_the_time)
* [Función get_the_excerpt()](https://codex.wordpress.org/Function_Reference/get_the_excerpt)
* [Función get_the_category_list()](https://codex.wordpress.org/Function_Reference/get_the_category_list)
* [Función get_the_tag_list()](https://codex.wordpress.org/Function_Reference/get_the_tag_list)
* [Función get_the_author()](https://codex.wordpress.org/Function_Reference/get_the_author)
* [Función get_the_content()](https://codex.wordpress.org/Function_Reference/get_the_content)

**[⬆ regresar al índice](#Índice)**


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

**[⬆ regresar al índice](#Índice)**


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

**[⬆ regresar al índice](#Índice)**

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

**[⬆ regresar al índice](#Índice)**


## [Widgets](https://codex.wordpress.org/Widgets_API) en WordPress
* [Función register_sidebar()](https://codex.wordpress.org/Function_Reference/register_sidebar)	
* [Función dynamic_sidebar()](https://codex.wordpress.org/Function_Reference/dynamic_sidebar)

**[⬆ regresar al índice](#Índice)**