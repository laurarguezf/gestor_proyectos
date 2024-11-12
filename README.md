# ProjectHub

ProjectHub es una aplicación web que permite gestionar y visualizar proyectos individuales con detalles específicos. Está diseñado con una arquitectura de servidor y cliente, utilizando tecnologías de back-end para manejar la conexión con la base de datos y renderizar vistas dinámicas.

## Características ⭐

- **Visualización de Proyectos**: Cada proyecto tiene una página de detalles que incluye información como el nombre, descripción, tecnologías utilizadas, enlaces a la demo y el repositorio, así como información sobre el autor.
- **Base de Datos Relacional**: Los proyectos y sus autores se gestionan en una base de datos, permitiendo una relación entre proyectos y autores.
- **Renderizado Dinámico**: Utiliza `EJS` para renderizar dinámicamente las páginas del proyecto, lo que facilita el uso de variables y datos obtenidos de la base de datos en las vistas.
- **Estilos Responsivos**: La aplicación utiliza Sass y responsive design para garantizar una visualización óptima en distintos dispositivos.

## Tecnologías Utilizadas 🛠️

- **Frontend**: 🌐HTML5, 🎨Sass, ⚛️React, EJS (para el renderizado de vistas en el servidor)
- **Backend**: 🟩Node.js, 🚂Express.js
- **Base de Datos**: 🗃️MySQL (para almacenar la información de proyectos y autores)

## Instalación y Ejecución 🚀

1. **Clona el repositorio**:
    ```bash
    git clone https://github.com/tu-usuario/nombre-del-repositorio.git
    ```
2. **Instala las dependencias**:
    ```bash
    npm install
    ```
3. **Importa las tablas necesarias**:
   - En la carpeta `bd`, encontrarás el archivo `projectHub.dump.sql`. Importa este archivo en tu base de datos MySQL.

4. **Configura variables de entorno .env en el directorio raíz del proyecto y añade las siguientes variables** :
   - Variables como la URL de la base de datos pueden ser configuradas en un archivo `.env`.

    ```bash
    DB_HOST=            # Host de la base de datos (e.g., localhost)
    DB_USER=            # Usuario de la base de datos (e.g., root)
    DB_PASSWORD=        # Contraseña del usuario
    DB_NAME=            # Nombre de la base de datos
    ```
5. **Inicia el servidor**:
    ```bash
    npm start
    ```
   El servidor debería iniciarse en `http://localhost:3000`.

## Uso 👨‍💻

- Navega a `http://localhost:3000/projects` para ver la lista de proyectos.
- Selecciona un proyecto para ver sus detalles en una página específica.

## Endpoints Principales 📚

- **GET /projects**: Muestra la lista de todos los proyectos.
- **GET /projects/:id**: Muestra los detalles de un proyecto específico.
- **POST /projects**: Crea un nuevo proyecto