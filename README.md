# 📝 Notes API

**Notes API** es un backend simple hecho con Node.js y PostgreSQL que permite a los usuarios registrar una cuenta y gestionar sus notas personales. Ideal para practicar desarrollo de APIs, autenticación y estructura modular de proyectos backend.

## 🚀 Funcionalidades

- Registro e inicio de sesión con autenticación JWT
- Crear, leer, actualizar y eliminar notas
- Rutas protegidas por token
- Estructura limpia y escalable

## ⚙️ Instalación

### 1. Clona el repositorio

```bash
git clone https://github.com/MicaelBurgos/notes-api.git
cd notes-api
2. Instala las dependencias
bash
Copiar
Editar
npm install
3. Crea un archivo .env con las variables necesarias
env
Copiar
Editar
PORT=3000
DATABASE_URL=postgres://usuario:contraseña@localhost:5432/notesdb
JWT_SECRET=clave_super_secreta
4. Ejecuta las migraciones de la base de datos
bash
Copiar
Editar
npx sequelize-cli db:create
npx sequelize-cli db:migrate
5. Inicia el servidor en desarrollo
bash
Copiar
Editar
npm run dev
La API estará corriendo en: http://localhost:3000

🛠 Tecnologías utilizadas
Node.js

Express.js

PostgreSQL

Sequelize

JWT

dotenv

📬 Endpoints
Método	Ruta	Descripción
POST	/auth/register	Crea un nuevo usuario
POST	/auth/login	Inicia sesión y devuelve un token
GET	/api/notes	Lista todas las notas del usuario
POST	/api/notes	Crea una nueva nota
PUT	/api/notes/:id	Actualiza una nota existente
DELETE	/api/notes/:id	Elimina una nota

⚠️ Las rutas bajo /api/notes requieren autenticación con token JWT:
Authorization: Bearer <tu_token>

📂 Estructura del proyecto
bash
Copiar
Editar
notes-api/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── app.js
├── .env
├── package.json
└── README.md
📌 Información adicional
Este proyecto está pensado para usarse como base para apps más grandes.

Puedes integrarlo fácilmente con un frontend hecho en React, Vue o Angular.

Próximamente: versión con Swagger + Docker.

✍️ Autor
Micael Burgos
📧 micael@example.com
🔗 GitHub | LinkedIn

📄 Licencia
Este proyecto está licenciado bajo la MIT License.

yaml
Copiar
Editar
