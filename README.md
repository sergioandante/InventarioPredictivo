# 💊 Sistema de Gestión de Inventarios para Farmacias

Bienvenido al repositorio del **Sistema de Inventarios de Farmacias**, desarrollado en Django. Esta aplicación está orientada a facilitar la administración, control y monitoreo del inventario de productos farmacéuticos en uno o varios locales.

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
- 📝 *(Futuro)* Historial de movimientos, exportación de reportes e integración con ventas/compras.

---

## 🛠️ Instalación y Configuración

### 1. Requisitos Previos

- Python 3.11 o superior
- PostgreSQL
- Git (opcional)
- Navegador web

### 2. Clona el repositorio


git clone https://github.com/usuario/InventarioPredictivo.git
cd InventarioPredictivo

## 🛠️ Instalación Paso a Paso

### 3. Crea y activa un entorno virtual

```bash
python -m venv venv
