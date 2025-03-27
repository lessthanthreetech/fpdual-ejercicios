# Ejercicio: Crear un contenedor Docker con Nginx

En este ejercicio aprenderás a crear un contenedor Docker que utilice Nginx para servir una página web. A continuación, se describen los pasos y requerimientos necesarios para completar la tarea.

## Requerimientos

1. **Instalación de Docker**: Asegúrate de tener Docker instalado en tu sistema. Si no lo tienes, puedes descargarlo desde [la página oficial de Docker](https://www.docker.com/).

2. **Conocimientos básicos de Docker**: Familiarízate con los conceptos básicos de Docker, como imágenes, contenedores y comandos básicos (`docker build`, `docker run`, etc.).

3. **Editor de texto**: Utiliza un editor de texto de tu preferencia para crear los archivos necesarios (por ejemplo, Visual Studio Code, Vim, Nano, etc.).

4. **Archivo HTML**: Crea un archivo `index.html` que será servido por Nginx. Este archivo debe contener una página web básica con un mensaje de bienvenida.

## Pasos a seguir

1. **Crear el archivo `Dockerfile`**:
    - En el mismo directorio, crea un archivo llamado `Dockerfile`.
    - Este archivo debe contener las instrucciones necesarias para:
      - Usar la imagen base de Nginx.
      - Copiar el archivo `index.html` al directorio adecuado dentro del contenedor.

2. **Construir la imagen Docker**:
    - Utiliza el comando `docker build` para construir la imagen Docker a partir del `Dockerfile`.
    - Asegúrate de etiquetar la imagen con un nombre descriptivo.

3. **Ejecutar el contenedor**:
    - Usa el comando `docker run` para crear y ejecutar un contenedor basado en la imagen creada.
    - Mapea el puerto 80 del contenedor al puerto 80 de tu máquina local para poder acceder a la página web desde el navegador.

4. **Probar la página web**:
    - Abre un navegador web y accede a `http://localhost` para verificar que la página se muestra correctamente.

## Resultado esperado

Al finalizar este ejercicio, deberías tener un contenedor Docker en ejecución que sirva la página web creada desde el archivo `index.html`. 

¡Ahora es tu turno! Completa los pasos y crea el `Dockerfile` necesario para arrancar el contenedor y mostrar la página.
