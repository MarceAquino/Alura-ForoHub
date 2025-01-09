# **APIREST_FOROHUB** - Foro Digital de Discusión

*¡Bienvenido al proyecto ForoHub! Un sistema API RESTful para gestionar un foro de discusión interactivo, fácil de usar y seguro.*

## 🚀 **Acerca de este Proyecto**

**APIREST_FOROHUB** es un sistema de API RESTful desarrollado utilizando **Spring Boot** que permite gestionar usuarios, autenticación, y tópicos dentro de un foro de discusión. Esta plataforma permite que los usuarios se registren, inicien sesión de manera segura, creen y gestionen temas de discusión. ¡Es ideal para desarrolladores que quieren tener un foro interactivo con un backend robusto y eficiente!

🔑 **Características principales**:
- **Autenticación segura** mediante JWT.
- **Gestión completa de usuarios**, donde puedes registrar, editar y eliminar usuarios.
- **Creación y gestión de tópicos** para discusiones en el foro.
- **API RESTful** totalmente operativa.
- **Base de datos MySQL** para el almacenamiento de datos.

¡Este proyecto tiene todo lo que necesitas para empezar a crear tu propio foro digital!

## 🛠️ **Tecnologías Utilizadas**

- **Java 17** – El corazón del backend.
- **Spring Boot 2.x** – Framework para simplificar el desarrollo de aplicaciones web.
- **Spring Security** – Autenticación y autorización robusta.
- **JWT (JSON Web Tokens)** – Autenticación segura para los usuarios.
- **JPA (Java Persistence API)** – Para manejar la base de datos de manera eficiente.
- **MySQL** – Sistema de base de datos relacional.
- **Lombok** – Reducción de boilerplate code.

## 📥 **Instalación y Configuración**

Para comenzar a utilizar **APIREST_FOROHUB**, sigue estos pasos:

### 1. **Clona el repositorio**

Primero, debes clonar el proyecto a tu máquina local:

```bash
git clone https://github.com/Marcelo/APIREST_FOROHUB.git
2. Configura la base de datos
Este proyecto usa MySQL para almacenar los datos del foro. Asegúrate de tener MySQL instalado y corriendo en tu máquina.

Crea una base de datos llamada forohub_db.
Modifica el archivo src/main/resources/application.properties con tus credenciales de MySQL.
properties
Copiar código
spring.datasource.url=jdbc:mysql://localhost:3306/forohub_db
spring.datasource.username=root
spring.datasource.password=tu_password
api.security.secret=tu_clave_secreta
3. Ejecuta el proyecto
Ahora puedes ejecutar el proyecto usando Maven o tu IDE favorito:

Si usas Maven, ejecuta el siguiente comando:
bash
Copiar código
./mvnw spring-boot:run
O si usas tu IDE, simplemente ejecuta la clase ForoHubApplication.java.
📄 Endpoints de la API
La API cuenta con varios endpoints esenciales para interactuar con el foro. Aquí están los detalles de los endpoints:

Autenticación

POST /api/auth/login – Inicia sesión y devuelve un token JWT.
Usuarios

GET /api/users – Obtiene todos los usuarios registrados.
POST /api/users – Registra un nuevo usuario.
GET /api/users/{id} – Obtiene información de un usuario específico.
PUT /api/users/{id} – Actualiza un usuario.
DELETE /api/users/{id} – Elimina un usuario.
Tópicos

GET /api/topics – Obtiene todos los tópicos de discusión.
POST /api/topics – Crea un nuevo tópico de discusión.
GET /api/topics/{id} – Obtiene un tópico por ID.
PUT /api/topics/{id} – Actualiza un tópico.
DELETE /api/topics/{id} – Elimina un tópico.
🧑‍💻 Estructura del Proyecto
Este es un vistazo a la estructura de directorios y archivos dentro del proyecto:

plaintext
Copiar código
src/
 └── main/
     └── java/
         └── com/
             └── forohub/
                 ├── controller/         # Controladores de la API
                 ├── model/              # Modelos de datos (Usuarios, Tópicos, etc.)
                 ├── repository/         # Repositorios de la base de datos
                 ├── security/           # Configuraciones de seguridad
                 └── ForoHubApplication.java  # Clase principal de la aplicación
     └── resources/
         └── application.properties   # Configuraciones de la aplicación
         └── static/                   # Archivos estáticos (si es necesario)
         └── templates/                 # Plantillas de vistas (si es necesario)

🤝 Cómo Contribuir
¡Nos encantaría recibir tus contribuciones! Si quieres aportar al proyecto, sigue estos pasos:

Haz un fork del repositorio.
Crea una nueva rama (git checkout -b feature-nueva-funcionalidad).
Haz tus cambios y realiza un commit (git commit -am 'Agrega nueva funcionalidad').
Haz push a la rama (git push origin feature-nueva-funcionalidad).
Abre un pull request en GitHub.

📧 Contacto
Si tienes alguna pregunta o comentario, ¡no dudes en contactarme! Puedes enviarme un correo a marceloaquino1676@gmail.com.

¡Gracias por tu interés en ALURA_FOROHUB! 🎉
Espero que este proyecto sea de utilidad para ti y te inspire a seguir desarrollando aplicaciones increíbles. ¡Nos vemos en el foro! 🚀
