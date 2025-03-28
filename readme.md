# Práctica despliegue

## Ejercico 1:
La arquitectura deseada para la puesta en producción es la siguiente:
  - Utilizar node como servidor de aplicación utilizando PM2 o supervisor como gestor de procesos node para que siempre esté en ejecución. La aplicación node deberá reiniciarse automáticamente al arrancar el servidor (en el startup).
  - Utilizar nginx como proxy inverso que se encargue de recibir las peticiones HTTP y derivárselas a node.
  - Los archivos estáticos de la aplicación (imágenes, css, etc.) deberán ser servidos por nginx (no por node). Para poder diferenciar quién sirve estos estáticos, se deberá añadir una cabecera HTTP cuando se sirvan estáticos cuyo valor sea: X-Owner (la X- indica que es una cabecera personalizada) y el valor de la cabecera deberá ser el nombre de la cuenta de usuario en github o bitbucket del alumno. Si la solución de la práctica por parte del alumno no tuviera archivos estáticos, deberá proporcionar el acceso a un archivo estático que se sirva a través de nginx (por ejemplo a través de la URL <dominio>/public/logo.jpg). En este caso, el alumno deberá indicar la URL del archivo estático en el archivo README.md del repositorio.

### Solucion:

http://ec2-184-72-210-248.compute-1.amazonaws.com/

## Ejecicio 2:
  - Si se accede al servidor web indicando la dirección IP del servidor en lugar del nombre de dominio, se deberá carga la práctica realizada en el módulo de React o React Avanzado.

### Solucion:

http://184.72.210.248/login