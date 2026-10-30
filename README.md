<h1 align="center">Gestión de Inventario con Filament</h1>

<p align="center">
  Dashboard para controlar productos, entradas, salidas, proveedores y clientes con reportes y gráficas.<br/>
  <sub>Dashboard to manage products, stock in/out, suppliers and customers with reports and charts.</sub>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-Web-38BDF8?style=flat" alt="Web"/>
  <img src="https://img.shields.io/badge/type-Backend-FF2D20?style=flat" alt="Backend"/>
  <img src="https://img.shields.io/badge/year-2025-495057?style=flat" alt="2025"/>
</p>

<p align="center">
  <a href="#español">Español</a> · <a href="#english">English</a>
</p>

<p align="center">
  <img src="https://drey.is-a.dev/img/projects/project5/project5-2.png" alt="Dashboard" width="90%"/>
</p>

## Tech stack

<p align="center">
  <img src="https://img.shields.io/badge/PHP-8.2-777BB4?style=flat&logo=php&logoColor=white" alt="PHP 8.2"/>
  <img src="https://img.shields.io/badge/Laravel-12-FF2D20?style=flat&logo=laravel&logoColor=white" alt="Laravel 12"/>
  <img src="https://img.shields.io/badge/Filament-3-FDAE4B?style=flat" alt="Filament 3"/>
  <img src="https://img.shields.io/badge/Livewire-Components-4E56A6?style=flat&logo=livewire&logoColor=white" alt="Livewire"/>
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=flat&logo=mysql&logoColor=white" alt="MySQL"/>
  <br/>
  <img src="https://img.shields.io/badge/Tailwind%20CSS-4-06B6D4?style=flat&logo=tailwindcss&logoColor=white" alt="Tailwind CSS 4"/>
  <img src="https://img.shields.io/badge/Vite-7-646CFF?style=flat&logo=vite&logoColor=white" alt="Vite 7"/>
  <img src="https://img.shields.io/badge/Chart.js-Charts-FF6384?style=flat&logo=chartdotjs&logoColor=white" alt="Chart.js"/>
  <img src="https://img.shields.io/badge/Laravel%20Excel-Exports-21A366?style=flat" alt="Laravel Excel"/>
  <img src="https://img.shields.io/badge/DomPDF-PDF-CC0000?style=flat" alt="DomPDF"/>
</p>

## Screenshots

<table>
  <tr>
    <td width="50%" align="center">
      <img src="https://drey.is-a.dev/img/projects/project5/project5-3.png" alt="Charts"/>
      <br/><b>Gráficas · Charts</b><br/><sub>Entradas y salidas por mes y por producto</sub>
    </td>
    <td width="50%" align="center">
      <img src="https://drey.is-a.dev/img/projects/project5/project5-4.png" alt="Products"/>
      <br/><b>Productos · Products</b><br/><sub>Tabla con filtros y exportación a Excel y PDF</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <img src="https://drey.is-a.dev/img/projects/project5/project5-5.png" alt="New entry"/>
      <br/><b>Nueva entrada · New stock entry</b><br/><sub>Actualiza el stock automáticamente</sub>
    </td>
    <td width="50%" align="center">
      <img src="https://drey.is-a.dev/img/projects/project5/project5-6.png" alt="Outputs"/>
      <br/><b>Salidas · Stock out</b><br/><sub>Ventas por cliente con factura y totales</sub>
    </td>
  </tr>
</table>

---

## Español

> Aplicación de inventario construida con Laravel y el panel administrativo de Filament. Registra entradas y salidas, mantiene el stock al día y muestra métricas en un dashboard.

### Funcionalidades

| Área | Descripción |
|---|---|
| **Dashboard** | Estadísticas y gráficas por categoría: entradas, productos (stock, valor, bajo stock) y proveedores. |
| **Entradas** | Registro de compras que suma stock automáticamente; al editar o eliminar se ajusta o revierte. |
| **Salidas** | Registro de ventas por cliente con número de factura. |
| **Catálogo** | Gestión de productos, categorías, proveedores y clientes. |
| **Tablas** | Búsqueda, filtros avanzados y acciones por fila. |
| **Reportes** | Exportación a Excel (Laravel Excel) y PDF (DomPDF). |

### Cómo ejecutarlo

Requisitos: **PHP 8.2+**, Composer, Node.js 18+ y MySQL.

```bash
composer install
cp .env.example .env        # configura DB_* y APP_URL
php artisan key:generate
php artisan migrate
npm install && npm run dev
php artisan serve
```

Entra al panel en `/dashboard`.

> [!TIP]
> Para ver Filament en español agrega al `.env`: `APP_LOCALE=es`, `APP_FALLBACK_LOCALE=es` y `APP_FAKER_LOCALE=es_ES`.

### Estructura

```
app/Filament/Resources   CRUD de Filament (entradas, salidas, productos, proveedores, categorías, clientes)
app/Filament/Widgets     Estadísticas y gráficas del dashboard
app/Exports              Exportaciones a Excel
app/Models               Modelos Eloquent
resources/views          Vistas Blade (incluye las de PDF)
```

---

## English

> Inventory app built with Laravel and the Filament admin panel. It records stock entries and outputs, keeps stock up to date and shows metrics on a dashboard.

### Features

| Area | Description |
|---|---|
| **Dashboard** | Stats and charts by category: entries, products (stock, value, low stock) and suppliers. |
| **Entries** | Purchase records that add stock automatically; editing or deleting adjusts or reverts it. |
| **Outputs** | Sales records per customer with invoice number. |
| **Catalog** | Management of products, categories, suppliers and customers. |
| **Tables** | Search, advanced filters and row actions. |
| **Reports** | Export to Excel (Laravel Excel) and PDF (DomPDF). |

### Getting started

Requirements: **PHP 8.2+**, Composer, Node.js 18+ and MySQL.

```bash
composer install
cp .env.example .env        # set DB_* and APP_URL
php artisan key:generate
php artisan migrate
npm install && npm run dev
php artisan serve
```

Open the panel at `/dashboard`.

> [!TIP]
> To show Filament in Spanish, add to `.env`: `APP_LOCALE=es`, `APP_FALLBACK_LOCALE=es` and `APP_FAKER_LOCALE=es_ES`.

---

## Autor · Author

Desarrollado por **Andrey Mantilla Leon** · Ingeniería de Sistemas. Portafolio: [drey.is-a.dev](https://drey.is-a.dev)
