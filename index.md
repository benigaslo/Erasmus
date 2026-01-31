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
    background-image: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://www.consilium.europa.eu/media/54319/erasmus.png') !important;
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

/* La tira de imágenes */
/* Contenedor principal: usamos Flex para alinear [Botón][Imagen][Botón] */
  .slider-horizontal {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    margin: 40px 0;
    width: 100%;
  }

  /* El marco donde se ven las fotos */
  .visor-fotos {
    display: flex;
    overflow: hidden; /* Escondemos el resto de fotos */
    scroll-behavior: smooth;
    scroll-snap-type: x mandatory;
    width: 80%; /* Ajusta esto para cambiar el ancho de las fotos */
    max-width: 800px;
    border: 3px solid #00fbff;
    border-radius: 15px;
    background: rgba(0,0,0,0.4);
    box-shadow: 0 10px 30px rgba(0, 251, 255, 0.2);
  }

  .visor-fotos img {
    flex: 0 0 100%;
    scroll-snap-align: center;
    width: 100%;
    height: 450px; /* Altura fija para consistencia */
    object-fit: contain; /* Evita que la foto se corte */
    padding: 10px;
  }

  /* Estilo de los botones laterales */
  .boton-lateral {
    background: none;
    border: 2px solid #00fbff;
    color: #00fbff;
    font-size: 24px;
    font-weight: bold;
    padding: 15px 20px;
    cursor: pointer;
    border-radius: 10px;
    transition: all 0.3s ease;
    flex-shrink: 0; /* Evita que el botón se aplaste */
  }

  .boton-lateral:hover {
    background: #00fbff;
    color: #000;
    box-shadow: 0 0 15px #00fbff;
  }

  /* Ocultar en móviles si el espacio es muy pequeño */
  @media (max-width: 600px) {
    .slider-horizontal { gap: 5px; }
    .boton-lateral { padding: 10px; font-size: 18px; }
    .visor-fotos { width: 100%; }
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
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel').scrollBy({left: -document.getElementById('carrusel').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel">
    <img src="./images/IMG_20260113_091924.jpg" alt="Llegada">
    <img src="./images/IMG_20260113_092303.jpg" alt="Instituto">
    <img src="./images/IMG_20260113_093736.jpg" alt="Clase 1">
    <img src="./images/IMG_20260113_112640.jpg" alt="Clase 2">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel').scrollBy({left: document.getElementById('carrusel').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

---

<div style="text-align: center; margin-top: 100px; padding-bottom: 50px;">
  <h1>¡Gracias por su atención!</h1>
  <p>Erasmus+ 2025-2026</p>
</div>