# Tetris (Tateti) - README
![Aplicación](https://utfs.io/f/9425cc44-3632-496c-9c5f-538f0c91efe3-1zo3d.jpg)

## Descripción

Este es un proyecto de Tetris (Tateti) que combina un frontend desarrollado con Angular, HTML y CSS, y un backend implementado con NestJS y Socket.IO. El juego permite a los usuarios jugar Tetris en tiempo real con funcionalidades multijugador a través de una conexión en tiempo real proporcionada por Socket.IO.

## Tecnologías Utilizadas

- **Frontend**: 
  - **Angular**: Framework para construir aplicaciones web dinámicas.
  - **HTML/CSS**: Tecnologías para estructurar y estilizar el contenido del juego.

- **Backend**:
  - **NestJS**: Framework para construir aplicaciones del lado del servidor con Node.js, proporcionando una arquitectura escalable y modular.
  - **Socket.IO**: Biblioteca para permitir la comunicación en tiempo real entre el cliente y el servidor.

## Estructura del Proyecto

- **Frontend**: 
  - Carpeta de Angular que contiene el código del cliente.
  - Archivos HTML y CSS para la interfaz de usuario.

- **Backend**:
  - Carpeta de NestJS que contiene el código del servidor.
  - Configuración de Socket.IO para la comunicación en tiempo real.

- **docker-compose.yaml**:
  - Configuración de Docker Compose para ejecutar el frontend y el backend en contenedores separados.

## Instalación

### Requisitos Previos

Asegúrate de tener instalados los siguientes componentes:
- [Node.js](https://nodejs.org/)
- [Docker](https://www.docker.com/get-started)


### Configuración con Docker

Para desplegar con  Docker, puedes iniciar los contenedores usando Docker Compose:

1. Asegúrate de estar en la raíz del proyecto, donde se encuentra el archivo `docker-compose.yaml`.

2. Ejecuta el siguiente comando para construir y ejecutar los contenedores:

    ```bash
    docker-compose up --build
    ```

3. La web  disponible en `http://localhost:8080` y el backend en el mismo puerto debido a que es un balanceador de carga y reverse proxy todas las peticiones se redirigiran al puerto 8080.
![Contenedores de la aplicación](https://utfs.io/f/70f3ad2b-6568-4161-a04f-ce24e9d19966-2cw.jpg)

## Uso

1. Abre tu navegador y accede a `http://localhost:8080` para ver la aplicación frontend.
2. Juega al Tetris en tiempo real con otros jugadores  gracias a la comunicación en tiempo real proporcionada por Socket.IO. Si no hay jugadores puedes abrir otra ventana

## Contribución

Si deseas contribuir a este proyecto, por favor sigue estos pasos:
1. Haz un fork del repositorio.
2. Crea una rama para tu nueva funcionalidad o corrección de errores.
3. Realiza los cambios y haz un commit.
4. Envía un pull request describiendo tus cambios.

## Licencia

Este proyecto está licenciado bajo la [MIT License](LICENSE).

## Contacto

Si tienes alguna pregunta o necesitas ayuda, no dudes en contactarme a través de [tu email](mailto:fabrisio021@gmail.com).