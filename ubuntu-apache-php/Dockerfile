# Imagen base Ubuntu
FROM ubuntu:22.04

# Evitar interacción al instalar paquetes
ENV DEBIAN_FRONTEND=noninteractive

# Actualizar e instalar Apache, PHP, Git
RUN apt-get update && apt-get install -y apache2 php libapache2-mod-php git curl

# Por si acasos limpiamos posibles restos en /var/www/html
RUN rm -rf /var/www/html

# Descargar app PHP sencilla
RUN git clone https://github.com/heroku/php-getting-started.git /var/www/html

# Dar permisos correctos
RUN chown -R www-data:www-data /var/www/html

# Exponer puerto 80
EXPOSE 80

# Ejecutar Apache en primer plano
CMD ["apachectl", "-D", "FOREGROUND"]
