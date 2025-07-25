# 💊 Sistema de Gestión de Inventarios para Farmacias

Bienvenido al repositorio del **Sistema de Inventarios de Farmacias**, desarrollado en Django. Esta aplicación está diseñada para facilitar la administración, control y monitoreo del inventario de productos farmacéuticos en uno o varios locales.

---

## 🚀 Descripción General

Este proyecto es una aplicación web que permite a cada farmacia:

- Visualizar y gestionar su inventario (productos, categorías, stock, fechas de vencimiento, etc.).
- Clasificar los estados de stock como crítico, bajo, medio o alto.
- Controlar el valor económico de los productos.
- Prevenir faltantes, sobrestock y pérdidas por caducidad.

---

## 📦 Funcionalidades Principales

- 📋 Visualización del inventario paginado por farmacia.
- 🔍 Consulta detallada de cada producto: categoría, precio, stock, vencimiento, etc.
- ⚠️ Alertas y reportes de productos con stock bajo o próximos a vencer.
- 📊 Resumen estadístico del inventario: totales, críticos, bajo stock, valor total.
- 👥 Gestión de usuarios (empleados, administradores) con permisos diferenciados.
- 📝 *(Futuro)* Historial de movimientos y auditoría de inventario.

---

## 🛠️ Instalación Paso a Paso

Sigue estos pasos para configurar el proyecto en tu entorno local:

1. **Clona el repositorio**
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd <NOMBRE_DEL_REPOSITORIO>
   ```

2. **Crea y activa un entorno virtual**
   ```bash
   python -m venv venv
   ```
   - En Windows:
     ```bash
     venv\Scripts\activate
     ```
   - En Mac/Linux:
     ```bash
     source venv/bin/activate
     ```

3. **Instala las dependencias**
   ```bash
   pip install -r requirements.txt
   ```

   <details>
   <summary>📦 Dependencias principales</summary>

   - Django==5.0.4
   - psycopg2-binary==2.9.9
   - python-decouple==3.8
   - pandas==2.2.2
   - SQLAlchemy==2.0.30

   </details>

4. **Configura las variables de entorno**
   Crea un archivo `.env` en la raíz del proyecto con el siguiente contenido:
   ```env
   DEBUG=True
   SECRET_KEY=tu_clave_secreta
   DB_NAME=nombre_de_tu_base
   DB_USER=tu_usuario_postgres
   DB_PASSWORD=tu_password_postgres
   DB_HOST=localhost
   DB_PORT=5432
   ```
   Asegúrate de que los valores coincidan con tu configuración local de PostgreSQL.

5. **Aplica las migraciones y crea un superusuario**
   ```bash
   python manage.py migrate
   python manage.py createsuperuser
   ```

6. **Ejecuta el servidor de desarrollo**
   ```bash
   python manage.py runserver
   ```
   Accede a la aplicación en: [http://localhost:8000](http://localhost:8000)

---

## 📁 Estructura Básica del Proyecto

| Carpeta/Archivo       | Descripción                                      |
|-----------------------|--------------------------------------------------|
| `farmacia_app/`       | Lógica principal del sistema: modelos, vistas, etc. |
| `manage.py`           | Comando principal de Django                      |
| `requirements.txt`    | Dependencias del proyecto                        |
| `.env`                | Variables de entorno sensibles                   |
| `BasedeDatos/`        | Archivos o respaldos relacionados con la base    |

---

## ✨ Uso Básico

1. Inicia sesión con el usuario creado o solicita acceso al administrador.
2. Usa el menú para seleccionar la farmacia y visualizar el inventario:
   - Productos, stock actual, vencimiento, estado de stock.
3. Filtra productos por nombre, clase, etc.
4. Consulta reportes de productos en estado crítico o próximos a vencer.
5. *(Solo Admin)* Agrega productos, ajusta stock o consulta el resumen general.

---

## 🧩 Manual Técnico y de Usuario

Para más detalles técnicos y guías de uso, consulta la carpeta `/docs/` (si existe) o solicita el manual integrado al equipo desarrollador.

---

## 📝 Notas Adicionales

- Asegúrate de tener PostgreSQL instalado y configurado correctamente antes de ejecutar las migraciones.
- Si tienes problemas con las dependencias, verifica que estás utilizando una versión compatible de Python (recomendado: Python 3.8+).
- Para personalizar los estilos de la aplicación, revisa los archivos CSS en la carpeta correspondiente (si aplica).

---

¡Gracias por usar el **Sistema de Gestión de Inventarios para Farmacias**! Si tienes dudas o sugerencias, contacta al equipo desarrollador. 🚀
