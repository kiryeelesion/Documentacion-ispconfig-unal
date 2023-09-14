---
title: Hacer backup del sitio web mediante ftp
author: Rodrigo Castro Díaz
date: 2023-03-08
updated: 2023-03-08
tags:
  - Tecnología
  - ispconfig
---

# Hacer backup del sitio web mediante FTP

A veces es necesario realizar un backup de todos los archivos de nuestro sitio web, y podemos realizar este backup a través de nuestro usuario FTP

## Requisitos
Para poder realizarlo requerimos del usuario y contraseña del usuario de FTP, que generalmente es entregado cuando se crea el sitio web. También necesitaremos el programa [FileZilla](https://filezilla-project.org/index.php "Home FileZilla") que funciona como cliente FTP. 

## Instalando cliente FTP
### Descargando cliente FTP
Podemos descargar FileZilla desde [aquí](https://filezilla-project.org/download.php?type=client "Descarga de FileZilla"), descargamos el archivo correspondiente al sistema operativo donde lo usaremos, para esta guía usaremos Windows como sistema operativo.

![Descarga de FileZilla](assets/01_descarga_filezilla.gif "Descarga de FileZilla")

### Instalando FileZilla
Una vez descargado el archivo, procedemos a ejecutar el programa, y seguir las instrucciones de instalación. 

![Instalando FileZilla](assets/02_instalar_filezilla.gif "Instalando FileZilla")

En caso de que ya lo tengamos instalado nos preguntara si deseamos actualizarlo, y es buena práctica mantenerlo actualizado.

## Realizar backup de los archivos del sitio web

Una vez abrimos FileZilla, ingresaremos los datos de conexión a nuestro sitio web, dirección IP del servidor donde se encuentra alojada nuestra web, usuario y contraseña del acceso a FTP y por último puerto de conexión.

![Establecer Conexión FTP](assets/03_Ingresar_credenciales.gif "Establecer Conexión FTP")

Si se realiza la conexión veremos como en la pantalla de estado nos muestra *Directorio "/" listado correctamente*, así como en el lado derecho en *sitio remoto* veremos la lista de carpetas de nuestro sitio.

![Servidor conectado](assets/04_servidor_conectado.png "Servidor conectado")

Ahora al lado izquierdo en *Sitio local* navegaremos y ubicaremos una carpeta para descargar todos nuestros archivos del sitio web. Como ejemplo, elegiré la carpeta de descargas.

![Ubicando la ruta de descarga](assets/05_ubicando_ruta_de_descarga.gif "Ubicando la ruta de descarga")

Ahora que ya tenemos la carpeta para descargar el contenido, nos dirigimos a *Sitio remoto*, seleccionamos las carpetas y procedemos a descargar todo el contenido, si el sitio es muy grande podría ser recomendable hacerlo carpeta por carpeta.

![Descargando archivos](assets/06_descargando_archivos.gif "Descargando archivos")

Una vez terminé de descargar ya tendremos todos los archivos del sitio web en nuestro equipo. Así es como podremos hacer backups.