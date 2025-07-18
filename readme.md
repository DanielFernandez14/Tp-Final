# 🧪 Trabajo Práctico Complementario: Implementación de Búsqueda por Nombre

## 🎯 Objetivo

Agregar una funcionalidad de **búsqueda por nombre** de productos a una aplicación CRUD existente con backend en **Node.js + Express + MongoDB** y frontend en **React + Vite**. Esta mejora simula una tarea cotidiana dentro de un entorno laboral real, cumpliendo buenas prácticas de arquitectura y desarrollo.

---

## 📌 Funcionalidad Agregada

- Se incorporó un **campo de búsqueda en el frontend**, ubicado en la pantalla principal.
- A medida que el usuario escribe, se consulta al **backend** para buscar productos por nombre de forma **parcial e insensible a mayúsculas**.
- Los resultados se actualizan **en tiempo real (búsqueda en vivo)** sin recargar la página.
- Se mantiene la arquitectura MVC en el backend y la modularización en el frontend.

---

## 🚀 Tecnologías utilizadas

### Backend

- Node.js
- Express
- TypeScript
- MongoDB + Mongoose
- cors

### Frontend

- React
- Vite
- Fetch API
- Context API

---

## ⚙️ Instrucciones para ejecutar el proyecto

### 🛠️ 1. Clonar el repositorio

```bash
git clone https://github.com/DanielFernandez14/Tp-Final

**Backend bash:**
cd backend
npm install (node_modules)

Crear el archivo .env:
PORT=1234
URI_DB=mongodb://localhost:27017/api-utn-products (o el que corresponda para desarrollo)
JWT_SECRET=claveSecretaUltraSegura123 (clave usada para el desarrollo)

Ejecutar:
npm run dev


**Frontend bash:**
cd frontend
npm install

Crear el archivo .env:
VITE_BACKEND_URL=http://localhost:1234

Ejecutar: 
npm run dev

La app estará disponible en: http://localhost:5173

Ejemplo de uso:

El usuario accede a la pantalla principal (/).

Escribe un término en el campo de búsqueda, por ejemplo: "lavanDina"

Automáticamente se filtran los productos que contienen ese nombre, sin importar mayúsculas/minúsculas.

Si el input se limpia, se muestran todos los productos de nuevo.
