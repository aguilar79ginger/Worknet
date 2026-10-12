# WorkNet

Plataforma de reclutamiento y gestión de empleo web desarrollada con WordPress, PHP, MySQL y XAMPP.

## Descripción del Proyecto
WorkNet es una solución diseñada para conectar a aspirantes con ofertas de empleo de manera eficiente, integrando perfiles de usuario personalizados, visualización de plazas disponibles y control de postulaciones.

## Requisitos Previos
* Tener instalado [XAMPP](https://www.apachefriends.org/es/index.html) (con los servicios de Apache y MySQL activos).
* Una instalación previa o limpia de WordPress en tu entorno local.

## Contenido del Repositorio
* **`twentytwentyfive.rar`**: Archivo comprimido que contiene el tema personalizado y adaptado para la interfaz visual de WorkNet.
* **`base-de-datos.sql`**: Respaldo completo de la base de datos MySQL (con los registros de usuarios, configuraciones y estructura de tablas).
* **`README.md`**: Guía de documentación e instalación del proyecto.

## Instrucciones de Instalación Local

1. **Clonar o descargar** este repositorio dentro de tu carpeta `htdocs` de XAMPP (por ejemplo: `htdocs/wordpress/`).
2. **Configurar el tema:** Extrae el contenido del archivo comprimido `twentytwentyfive.rar` dentro de la ruta `wp-content/themes/` de tu instalación de WordPress.
3. **Importar la Base de Datos:**
   * Abre phpMyAdmin en tu navegador (`http://localhost/phpmyadmin/`).
   * Crea una nueva base de datos (por ejemplo, con el nombre `wordpress`).
   * Selecciona tu base de datos, ve a la pestaña **Importar**, selecciona el archivo `base-de-datos.sql` de este repositorio y haz clic en **Continuar**.
4. **Configurar la conexión (`wp-config.php`):**
   Abre el archivo `wp-config.php` en la raíz de tu instalación de WordPress y verifica que los datos de conexión coincidan con tu servidor local:
   ```php
   define( 'DB_NAME', 'wordpress' );
   define( 'DB_USER', 'root' );
   define( 'DB_PASSWORD', '' );
   define( 'DB_HOST', 'localhost' );
