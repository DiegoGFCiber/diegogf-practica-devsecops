# Práctica 2: DevSecOps - Puesta en Producción Segura

## Objetivo
Crear imágenes de Docker seguras partiendo de PHP y Ubuntu+Apache.

## Estructura del proyecto
- `php-app/`: Imagen PHP copiando app local.
- `ubuntu-apache-php/`: Imagen Ubuntu que instala Apache, PHP y descarga app.

## Pasos Realizados

### Paso 1
Creación de imagen PHP copiando una aplicación local sencilla (`index.php`).

### Paso 2
Creación de imagen Ubuntu que instala Apache, PHP, descarga app PHP desde GitHub y la sirve en el puerto 80.

### Paso 3
Creación y ejecución de contenedores. Pruebas realizadas desde navegador y `curl`.

### Paso 4
Ejecución de 20 contenedores simultáneos en puertos 8001-8020.
