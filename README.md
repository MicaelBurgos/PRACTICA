# FacturasApp

Aplicación backend para la **gestión de facturación**, creada con Node.js y PostgreSQL. Permite registrar clientes, productos y generar facturas con cálculos automáticos. Ideal para pequeñas empresas o como base de práctica para proyectos CRUD con autenticación.

---

## ✨ Características principales

✅ Registro y listado de clientes  
✅ Registro de productos  
✅ Generación de facturas con totales  
✅ Asociación de múltiples productos por factura  
✅ Listado de facturas por cliente  
✅ Estructura modular y limpia, fácil de extender  

---

## 🧩 Tecnologías utilizadas

- 🟩 **Node.js** + **Express** (servidor backend)
- 🐘 **PostgreSQL** con **Sequelize** (ORM)
- 🔐 **JWT** (autenticación segura)
- 🧾 **PDFKit** (opcional para generar facturas en PDF)
- 📦 **dotenv**, **nodemon**, **bcrypt**, entre otros

## ¿Cómo funciona?

1. Se cargan los datos de los clientes y productos.
2. Se seleccionan productos para armar una factura.
3. Se genera la factura con fecha, cliente y total.
4. Las facturas pueden consultarse y editarse desde el sistema.

## Requisitos

- Node.js instalado
- PostgreSQL en funcionamiento
- npm o yarn como gestor de paquetes

## Pasos para ejecutar

1. Clona el repositorio:

   `git clone https://github.com/MicaelBurgos/facturas-app.git`

2. Instala dependencias:

   `npm install`

3. Configura el archivo `.env` con tus datos de base de datos.

4. Crea la base de datos y ejecuta las migraciones.

5. Inicia el servidor:

   `npm run dev`

## Autor

Micael Burgos  
Contacto: micael@example.com  
GitHub: [MicaelBurgos](https://github.com/MicaelBurgos)

