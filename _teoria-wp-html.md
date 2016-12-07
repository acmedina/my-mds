Plantillas en WordPress: Son los archivos que nuestro tema va utilizando dependiendo del contenido solicitado
        https://developer.wordpress.org/files/2014/10/wp-template-hierarchy.jpg
        index.php   >>  template principal
            home.php    >>  template del home del sitio
            archive.php >>  template de categorías y etiquetas
                category.php    >>  template de categorías
                tag.php >>  template de etiquetas
            singular.php    >>  template de entradas y páginas
                single.php  >>  template de entradas
                page.php    >>  template de páginas estáticas
            404.php >>  template para Error 404
            search.php  >>  template para búsquedas
            comments.php    >>  template para los comentarios
            author.php  >>  template para mostrar la página de autor
            ***Templates personalizados:
                Podemos tener templates personalizados para: 
                    categorías, etiquetas y páginas estáticas
                Podemos crear templates personalizados por:
                    slug, id o comentario php
    Etiquetas Condicionales
        https://codex.wordpress.org/Conditional_Tags
    https://developer.wordpress.org/themes/basics/including-css-javascript/



    WordPress
        https://platzi.com/blog/email-marketing-wordpress/
        https://wordpress.org/plugins/w3-total-cache/
        https://wordpress.org/plugins/wp-super-cache/
        http://www.ideaweb.es/wordpress-conoce-para-que-sirve-cada-tabla-de-la-base-de-datos/
        https://platzi.com/blog/crear-plugin-wordpress/
        https://platzi.com/blog/wp-api-rest/
        http://www.desarrolloweb.com/articulos/creacion-custom-post-type-wordpress.html
            http://metabox.io/
            https://wordpress.org/plugins/types/

        Seguridad
            http://www.trazos-web.com/2010/10/05/21-formas-de-mejorar-la-seguridad-de-tu-blog-en-wordpress/
            http://ignaciosantiago.com/blog/web/seguridad-en-wordpress-como-configurar-htaccess-para-evitar-hackeos/
            http://www.cws-tech.com/es/la-seguridad-de-wordpress/
            http://ignaciosantiago.com/blog/web/seguridad-en-wordpress-como-configurar-htaccess-para-evitar-hackeos/
            http://www.danielnabil.com/blog/redireccion-usuarios-registro-wordpress/
            http://www.danielnabil.com/blog/mostrar-contenidos-wordpress-usuarios-conectados/
            http://www.danielnabil.com/blog/proteger-categoria-wordpress-usuario-contrasena/
            https://platzi.com/blog/cambiar-url-login-wordpress/
                https://wordpress.org/plugins/peters-login-redirect/
            https://platzi.com/blog/medidas-de-seguridad-para-wordpress/
            https://platzi.com/blog/facebook-login-wordpress/
            https://www.youtube.com/watch?v=3BIoIWocR1I
            https://platzi.com/blog/wp-config-wordpress/

        Plugins
            https://wordpress.org/plugins/pdf-viewer/
            https://wordpress.org/plugins/pdfjs-viewer-shortcode/
            https://wordpress.org/plugins/simple-share-buttons-adder/
            https://wordpress.org/plugins/duplicator/
            https://wordpress.org/plugins/w3-total-cache/installation/
            https://wordpress.org/plugins/ewww-image-optimizer/
            https://wordpress.org/plugins/googleanalytics/
            https://wordpress.org/plugins/multiple-featured-images/
            https://wordpress.org/plugins/wp-most-popular/
            https://wordpress.org/plugins/most-popular-tags/
            https://wordpress.org/plugins/wp-spamshield/
            https://wordpress.org/plugins/gallery-images/
            https://wordpress.org/plugins/gtmetrix-for-wordpress/
            https://wordpress.org/plugins/mailchimp-for-wp/
            https://wordpress.org/plugins/gtmetrix-for-wordpress/
            https://wordpress.org/plugins/w3-total-cache/installation/
    

    WordPress
        <img width="300" height="169" src="http://localhost/aCursos/WordPress/perros/wp-content/uploads/2015/08/unicos-300x169.jpg" class="Post-image wp-post-image" alt="??????????????" srcset="http://localhost/aCursos/WordPress/perros/wp-content/uploads/2015/08/unicos-300x169.jpg 300w, http://localhost/aCursos/WordPress/perros/wp-content/uploads/2015/08/unicos.jpg 1024w" sizes="(max-width: 300px) 100vw, 300px">

        https://css-tricks.com/snippets/wordpress/remove-width-and-height-attributes-from-inserted-images/
        <img  src="<?php the_post_thumbnail_url( 'small'); ?>"
              srcset="<?php the_post_thumbnail_url( 'medium'); ?> 300w,
              <?php the_post_thumbnail_url( 'large'); ?> 768w,
              <?php the_post_thumbnail_url( 'full'); ?> 1200w"
              sizes="(min-width:64em) 33vw,
                    (min-width:48em) 50vw,
                    100vw"
              alt="<?php the_post_thumbnail_caption(); ?>" />
              
        http://cesarhdz.com/articulos/personalizar-menus-en-wordpress-con-un-walker#personalizar-el-menu
