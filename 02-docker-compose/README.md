# Ejercicio: Creación de un fichero `docker-compose.yaml`

Este ejercicio consiste en crear un fichero `docker-compose.yaml` que permita orquestar los diferentes servicios necesarios para una aplicación. El objetivo es configurar y levantar los siguientes servicios:

1. **Backend**: La aplicación principal que ya cuenta con su propio `Dockerfile` creado.
2. **Base de datos (DB)**: Un servicio de base de datos que será utilizado por el backend.
3. **Nginx**: Un servidor web que actuará como proxy inverso para servir la aplicación.

## Requerimientos

1. **Backend**:
    - Utilizar la imagen generada a partir del `Dockerfile` existente.
    - Configurar las variables de entorno necesarias para que el backend se conecte a la base de datos.
    - Exponer el puerto correspondiente para que el backend sea accesible internamente.

2. **Base de datos**:
    - Utilizar una imagen oficial de base de datos (por ejemplo `mysql`).
    - Configurar las credenciales de acceso (usuario, contraseña y nombre de la base de datos) mediante variables de entorno.
    - Mapear un volumen para persistir los datos.

3. **Nginx**:
    - Utilizar una imagen oficial de `nginx`.
    - Configurar un archivo de configuración personalizado para que actúe como proxy inverso hacia el backend.
    - Exponer el puerto 80 para que la aplicación sea accesible desde el navegador.

## Instrucciones

1. Crear un fichero `docker-compose.yaml` en el directorio actual.
2. Definir los servicios mencionados anteriormente con sus respectivas configuraciones.
3. Verificar que todos los servicios se inicien correctamente ejecutando `docker-compose up`.
4. Comprobar que la aplicación es accesible desde el navegador a través de `http://localhost`.

¡Buena suerte con el ejercicio!