# OPC API Service

Este proyecto es un servicio desarrollado en **Node.js** que conecta datos de un servidor OPC y los expone a través de una API REST. Además, permite configurar valores del servidor OPC de manera dinámica mediante los endpoints de la API.

---

## 🚀 Características

- **Conexión con servidor OPC:** Lectura y escritura de datos en tiempo real desde un servidor OPC.
- **API REST:** Endpoints para obtener y configurar datos del servidor OPC.
- **Configurabilidad:** Permite la modificación de valores en el servidor OPC mediante solicitudes HTTP.
- **Documentación Swagger:** Incluye documentación interactiva para facilitar el uso de la API.

---

## 📋 Requisitos

- **Node.js** v14 o superior.
- **npm** v6 o superior.
- Servidor OPC accesible.

---

## 🛠️ Instalación

1. Clona el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>

2. Accede al directorio del proyecto:
   ```bash
   cd api_opc_service-dev
3. Instala las dependencias:
   ```bash
   npm install

---

## ⚙️ Configuración

Configura las siguientes variables de entorno antes de iniciar el servicio:

- `PORT`: Puerto en el que el servicio estará disponible (por defecto: `4000`).
- `OPC_SERVER_URI`: URI del servidor OPC al que se conectará la aplicación.
- `MONGODB_URI`: URI de la base de datos MongoDB (si aplica).

Ejemplo de archivo `.env`:

```env
PORT=4000
OPC_SERVER_URI=opc.tcp://localhost:4840
MONGODB_URI=mongodb://localhost:27017/opc_service

---

## ▶️ Uso

1. Inicia el servicio:  
   ```bash
   npm start
2. Accede a la documentación de la API (Swagger):
  ```bash
  http://localhost:4000/doc/

---

## Estructura del Proyecto
```
├── src
│   ├── controllers
│   ├── libs
│   ├── middlewares
│   ├── models
│   ├── routes
├── app.js
├── config.js
├── database.js
├── index.js
```

---

## 📝 Licencia
Este proyecto se distribuye bajo la Licencia MIT.
