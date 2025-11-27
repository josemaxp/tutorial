# BirdPedy Web

Landing page oficial de **BirdPedy**, la app de birding/pajareo para el avistamiento y registro de aves en España.

Esta web está construida con **Astro** y **Tailwind CSS (v4)** y está pensada como una landing ligera, rápida y optimizada para SEO, orientada a llevar tráfico hacia la app de Android en Google Play.

---

## ✨ Características principales

- **Landing multidioma**: contenido en **español** e **inglés**, con interruptor ES/EN.
- **Diseño responsive** con layout claro:
  - Hero con call‑to‑action principal.
  - Sección de características.
  - Novedades destacadas (rareza, integración con iNaturalist y eBird).
  - Sección “Cómo funciona”.
  - Galería de capturas (ES/EN).
  - Sección de Instagram.
  - Preguntas frecuentes (FAQ) y CTA final.
- **SEO técnico**:
  - Meta tags básicas (`title`, `description`, Open Graph).
  - `JSON-LD` de tipo `FAQPage` (FAQ enriquecido).
  - `JSON-LD` de tipo `MobileApplication` (app para Android).
- **Estilo visual**:
  - Tema claro con fondo blanco.
  - Color principal verde `#6F986B` (color de BirdPedy).
  - Tipografía y espaciados pensados para lectura cómoda.
- **Sin frameworks de UI pesados**: solo Astro, Tailwind y un poco de JS vanilla para el cambio de idioma.

---

## 🛠 Stack técnico

- [Astro](https://astro.build/)
- [Tailwind CSS v4](https://tailwindcss.com/)
- HTML/JS/CSS estándar
- Sin backend (web estática)

---

## 📁 Estructura básica del proyecto

```bash
/
├─ public/
│  ├─ birdpedy-screenshot-1.png   # mockup del móvil en el hero
│  ├─ screens-es-1.png ... 6.png  # capturas en español
│  ├─ screens-en-1.png ... 6.png  # capturas en inglés
│  ├─ ig-1.jpg, ig-2.jpg, ig-3.jpg# imágenes para la sección de Instagram
│  └─ (opcional) birdpedy-logo.svg, og-image.jpg, etc.
├─ src/
│  ├─ layouts/
│  │  └─ Layout.astro             # layout principal (header, footer, SEO)
│  ├─ pages/
│  │  └─ index.astro              # landing principal
│  └─ styles/
│     └─ global.css               # Tailwind + estilos globales
├─ astro.config.mjs
├─ tailwind.config.mjs
├─ package.json
└─ README.md