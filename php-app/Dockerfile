# Imagen oficial PHP
FROM php:8.1-cli

# Carpeta de trabajo
WORKDIR /var/www/html

# Copiar app desde el host
COPY . /var/www/html

# Exponer puerto 80
EXPOSE 80

# Ejecutar servidor embebido
CMD ["php", "-S", "0.0.0.0:80", "-t", "/var/www/html"]
