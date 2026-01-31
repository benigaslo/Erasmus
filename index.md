---
layout: default
title: Presentación Erasmus
nav_order: 1
---

<style>
  /* 1. Transparencia Total en todas las capas del tema */
  /* Forzamos que los contenedores principales no tengan color de fondo */
  .main-content-wrap, 
  .main-content, 
  .site-header, 
  .side-bar,
  .main-header,
  .site-footer,
  .navigation-list,
  .nav-list-item {
    background: transparent !important;
    background-color: transparent !important;
  }

  /* 2. Configuración del Fondo en la capa más profunda */
  html, body {
    margin: 0;
    padding: 0;
    min-height: 100vh;
    /* Color oscuro de respaldo por si la imagen tarda en cargar */
    background-color: #000 !important; 
  }

  body {
    background-image: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1516321318423-f06f85e504b3?q=80&w=2070') !important;
    background-size: cover !important;
    background-position: center !important;
    background-attachment: fixed !important; /* Mantiene el fondo quieto al hacer scroll */
    background-repeat: no-repeat !important;
  }

  /* 3. Estilos de Texto para alta visibilidad */
  .main-content h1, .main-content h2, .main-content h3, 
  .main-content p, .main-content li, .main-content label {
    color: #ffffff !important;
  }

  /* Color especial para el título principal */
  .main-content h1 {
    color: #00fbff !important;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
  }

  /* Ocultar elementos de navegación si quieres estilo 'Presentación' */
  .side-bar, .site-footer {
    display: none !important;
  }
  
  /* Ajustar el margen que deja la barra lateral al ocultarla */
  .main-content-wrap {
    margin-left: 0 !important;
    padding: 2rem !important;
  }

/* --- Estilos del Slider --- */
  .slider-wrapper {
    position: relative;
    max-width: 900px;
    margin: 40px auto;
  }

  .slider {
    display: flex;
    overflow-x: auto;
    scroll-behavior: smooth;
    scroll-snap-type: x mandatory;
    gap: 20px;
    padding: 20px;
    /* Ocultar barra de scroll en navegadores */
    scrollbar-width: none; 
  }
  .slider::-webkit-scrollbar { display: none; }

  .slider img {
    flex: 0 0 100%; /* Cada imagen ocupa el 100% del contenedor */
    scroll-snap-align: center;
    width: 100%;
    height: auto;
    border: 3px solid #00fbff;
    border-radius: 15px;
    box-shadow: 0 10px 30px rgba(0, 251, 255, 0.3);
    object-fit: cover;
  }

  /* --- Botones de Navegación --- */
  .nav-btn {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background: rgba(0, 251, 255, 0.2);
    border: 2px solid #00fbff;
    color: white;
    padding: 15px;
    cursor: pointer;
    font-size: 24px;
    border-radius: 50%;
    backdrop-filter: blur(5px);
    transition: 0.3s;
    z-index: 10;
  }

  .nav-btn:hover { background: #00fbff; color: #000; }
  .prev { left: -60px; }
  .next { right: -60px; }

  /* Ajuste para móviles */
  @media (max-width: 768px) {
    .prev { left: 10px; }
    .next { right: 10px; }
    .nav-btn { padding: 10px; font-size: 18px; }
  }

</style>

# PRESENTACIÓN ERASMUS-VET 25-26
## 🌍 TURI (ISS PERTINI ANELLI)

---

### DÍA 1: Llegada al instituto ISS Pertini Anelli Pinto
<div class="mosaico-horizontal">
  <img src="./images/IMG_20260113_091924.jpg" alt="Llegada">
  <img src="./images/IMG_20260113_092303.jpg" alt="Instituto">
</div>

---

### Clase de informática - Prof. Vito Montanaro
<div class="slider-wrapper">
  <button class="nav-btn prev" onclick="moveSlider(-1, 'slider1')">❮</button>
  
  <div class="slider" id="slider1">
    <img src="./images/IMG_20260113_091924.jpg" alt="Llegada">
    <img src="./images/IMG_20260113_092303.jpg" alt="Instituto">
    <img src="./images/IMG_20260113_093736.jpg" alt="Clase 1">
    <img src="./images/IMG_20260113_112640.jpg" alt="Clase 2">
  </div>

  <button class="nav-btn next" onclick="moveSlider(1, 'slider1')">❯</button>
</div>

---

<div style="text-align: center; margin-top: 100px; padding-bottom: 50px;">
  <h1>¡Gracias por su atención!</h1>
  <p>Erasmus+ 2025-2026</p>
</div>