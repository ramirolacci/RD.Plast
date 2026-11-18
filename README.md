<div align="center">

  <img src="public/logo.png" alt="RD Plast Logo" width="120" />

  # RD Plast — Control & Gestión Industrial

  **Sistema Integral de Gestión de Clientes, Pedidos y Fichas Técnicas de Producción**

  ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
  ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
  ![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)
  ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

</div>

---

## ✨ Características Principales

* 📊 **Panel de Control en Tiempo Real**: Tarjetas dinámicas (KPIs) con métricas automáticas de pedidos en proceso, finalizados y entregados según las fechas programadas.
* 📋 **Fichas Técnicas de Producción**: Control exhaustivo para sectores de **Extrusión**, **Confección** e **Impresión** (Material cliente, Tratado, Fuelle, Microperforado, Medidas, Kilos, Metros, Cilindro, Colores, etc.).
* 🖨️ **Exportación e Impresión en PDF de Alta Calidad**: Generación de documentos formato A4 horizontal listos para imprenta/planta, individuales o masivos con línea de corte incorporada.
* 🔍 **Filtro y Búsqueda Inteligente**: Búsqueda instantánea multi-campo por Cliente, ID, Producto, Fechas y Estado.
* 🔒 **Seguridad y Perfiles de Usuario**: Control de acceso autenticado y roles de usuario (Administrador / Operario).
* 🎨 **Interfaz Ultra-Moderna**: Diseño en modo oscuro optimizado para alta visibilidad y dinamismo operativo.

---

## 📌 Vista Principal del Dashboard

<p align="center">
  <img src="docs/screenshots/03_dashboard_grid.png" alt="Dashboard Principal" width="100%" style="border-radius: 8px; box-shadow: 0 4px 20px rgba(0,0,0,0.3);" />
</p>

---

## 🖼️ Galería de Capturas del Sistema

### 📱 Módulos del Sistema

<table>
  <tr>
    <td width="50%" align="center">
      <b>Inicio de Sesión y Autenticación</b>
      <br/><br/>
      <img src="docs/screenshots/02_login_screen.png" alt="Inicio de Sesión" width="100%" />
    </td>
    <td width="50%" align="center">
      <b>Carga y Edición de Ficha Técnica</b>
      <br/><br/>
      <img src="docs/screenshots/04_client_form_modal.png" alt="Formulario Ficha Técnica" width="100%" />
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <b>Vista Previa de Impresión Individual</b>
      <br/><br/>
      <img src="docs/screenshots/05_pdf_print_single.png" alt="Impresión Ficha Individual" width="100%" />
    </td>
    <td width="50%" align="center">
      <b>Generación Masiva de PDF (A4)</b>
      <br/><br/>
      <img src="docs/screenshots/01_pdf_preview_multiple.png" alt="Exportación Masiva PDF" width="100%" />
    </td>
  </tr>
</table>

---

## 🛠️ Tecnologías Utilizadas

- **Frontend**: React 19, TypeScript, Vite.
- **Estilos**: Vanilla CSS moderno con variables, Glassmorphism y CSS Grid/Flexbox.
- **Base de Datos y Auth**: Supabase.
- **Librerías de Utilidad**: `html2pdf.js`, `gsap`, `react-router-dom`.

---

## 🚀 Instalación y Puesta en Marcha

### Prerrequisitos

Asegúrate de contar con las siguientes herramientas instaladas:
* [Node.js](https://nodejs.org/) (versión 18 o superior recomendada)
* [pnpm](https://pnpm.io/) (recomendado) o [npm](https://www.npmjs.com/)

---

### Pasos de Instalación

1. **Clonar el repositorio:**
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd RD.Plast
   ```

2. **Instalar dependencias:**
   ```bash
   pnpm install
   # o utilizando npm:
   # npm install
   ```

3. **Configurar las variables de entorno:**
   Copia el archivo `.env.example` y renómbralo a `.env`:
   ```bash
   cp .env.example .env
   ```
   Luego edita `.env` con las credenciales de tu proyecto de Supabase:
   ```env
   VITE_SUPABASE_URL=https://tu-proyecto.supabase.co
   VITE_SUPABASE_ANON_KEY=tu_supabase_anon_key
   ```

4. **Base de datos (Supabase):**
   Si estás configurando un nuevo proyecto de Supabase, puedes ejecutar las sentencias SQL provistas en [supabase_assets_schema.sql](file:///c:/Code/RD.Plast/supabase_assets_schema.sql) dentro del SQL Editor de Supabase para generar el esquema de tablas y políticas necesarias.

5. **Iniciar el servidor de desarrollo:**
   ```bash
   pnpm dev
   # o con npm:
   # npm run dev
   ```
   La aplicación se iniciará por defecto en `http://localhost:5173`.

---

### 📦 Scripts Disponibles

* `pnpm dev`: Inicia el servidor de desarrollo con Vite.
* `pnpm build`: Compila TypeScript y genera el bundle optimizado para producción en `dist/`.
* `pnpm preview`: Previsualiza localmente el build de producción.
* `pnpm lint`: Ejecuta el linter (Oxlint) para análisis de código.

---

<div align="center">
  <p><i>Desarrollado para RD Plast — Fábrica de Bolsas</i></p>
</div>
