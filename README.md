# 📡 Web API CRUD con ASP.NET y C#

Este proyecto es una **Web API RESTful** desarrollada en **ASP.NET con C#**, que se conecta a una base de datos **SQL Server**. Implementa operaciones **CRUD** (Crear, Leer, Actualizar, Eliminar) sobre una tabla de productos, utilizando **procedimientos almacenados**. La API puede ser probada fácilmente con herramientas como **Postman**.

> ✅ Proyecto desarrollado en **Visual Studio 2022**

---

## 🎯 Funcionalidades Principales

- ✅ Crear una Web API en C#
- ✅ Conectar a base de datos SQL Server
- ✅ Ejecutar procedimientos almacenados desde la API
- ✅ Implementar métodos CRUD: `GET`, `POST`, `PUT`, `DELETE`
- ✅ Probar las rutas de la API usando Postman

---

## ⚙️ Pila Tecnológica

- **C#**
- **ASP.NET Web API**
- **SQL Server**
- **HTML (para documentación de rutas)**
- **T-SQL (procedimientos almacenados)**

---

## 🧱 Estructura del Proyecto

ProyectoAPI/
│

├── App_Start/

│ └── WebApiConfig.cs → Configuración de rutas de la API

│
├── Controllers/

│ └── UsuarioController.cs → Controlador principal para operaciones CRUD

│
├── Data/

│ ├── Conexion.cs → Clase de conexión a SQL Server

│ └── UsuarioData.cs → Lógica de acceso a datos, ejecución de SP

│
├── Models/

│ └── Usuario.cs → Modelo de datos del objeto Usuario o Producto

│

└── DBPRUEBAS.sql → Script SQL de la base de datos

---

## 🗃️ Base de Datos: `DBPRUEBAS`

Contiene:

- **Tabla:** `PRODUCTO`
- **Procedimientos almacenados:**
  - `sp_lista_productos`
  - `sp_guardar_producto`
  - `sp_editar_producto`
  - `sp_eliminar_producto`
 

  🧪 Pruebas con Postman
  
Rutas disponibles (ejemplos):

GET /api/usuario → Lista todos los productos

POST /api/usuario → Inserta un nuevo producto

PUT /api/usuario → Actualiza un producto existente

DELETE /api/usuario/{id} → Elimina un producto por ID

Para probar estos métodos puedes importar un JSON a Postman o crear una colección con las rutas mencionadas.

🚀 Requisitos
Visual Studio 2022

SQL Server

Postman

Configurar cadena de conexión en Conexion.cs:

public static string rutaConexion = "Data Source=TU_SERVIDOR;Initial Catalog=DBPRUEBAS;Integrated Security=True";

🤝 Contacto
Para cualquier consulta técnica o comentario sobre este proyecto:

**Nombre: Maicolm Rivera Zamudio**

**Correo: grupoxpertos@gmail.com**

**LinkedIn: www.linkedin.com/in/maicolm-rivera-9537b6ba**


Este proyecto se ha diseñado con fines puramente demostrativos, formando parte de una evaluación técnica y como un ejemplo de la formación continua. El objetivo principal es mostrar las habilidades y capacidades adquiridas, así como demostrar la aplicación de los conocimientos en un contexto práctico. 
