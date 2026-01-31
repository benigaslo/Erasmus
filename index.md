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
    background-color: #000000ff !important; 
  }

  body {
    background-image: linear-gradient(rgba(0,0,0,0.1), rgba(0,0,0,0.1)), url('https://www.consilium.europa.eu/media/54319/erasmus.png') !important;
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
    color: #ff0000ff !important;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
  }

  /* Ocultar elementos de navegación si quieres estilo 'Presentación' */
  .side-bar, .site-footer {
    display: none !important;
  }
  
  /* Ajustar el margen que deja la barra lateral al ocultarla */
  /*.main-content-wrap {
    margin-left: 0 !important;
    padding: 2rem !important;
  }*/
  /* ------------------------------------------------------ */
  /* 1. Eliminamos los límites de ancho y márgenes del tema */
  .main-content-wrap {
    margin-left: 0 !important;
    max-width: 100% !important;
    padding: 0 !important; /* Quitamos paddings excesivos */
  }

  .main-content {
    max-width: 100% !important; /* Permite que el contenido use todo el ancho */
    padding: 2rem !important;    /* Un pequeño respiro para que no toque los bordes */
    margin: 0 auto !important;   /* Centra el bloque */
  }

  /* 2. Aseguramos que los sliders no se desborden y se vean centrados */
 .slider-horizontal {
    width: 100%;
    max-width: 1000px; /* O el ancho máximo que prefieras para tus fotos */
    margin: 40px auto !important; /* Centra el slider horizontalmente */
  }
  /* ------------------------------------------------------ */

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
    border: 3px solid #ff0000ff;
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
    border: 3px solid #ff0000ff;
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
    border: 2px solid #ff0000ff;
    color: #ff0000ff;
    font-size: 24px;
    font-weight: bold;
    padding: 15px 20px;
    cursor: pointer;
    border-radius: 10px;
    transition: all 0.3s ease;
    flex-shrink: 0; /* Evita que el botón se aplaste */
  }

  .boton-lateral:hover {
    background: #ff0000ff;
    color: #000;
    box-shadow: 0 0 15px #ff0000ff;
  }

  /* Ocultar en móviles si el espacio es muy pequeño */
  @media (max-width: 600px) {
    .slider-horizontal { gap: 5px; }
    .boton-lateral { padding: 10px; font-size: 18px; }
    .visor-fotos { width: 100%; }
  }

</style>

# ERASMUS+VET 25-26
## 🌍 LA PUGLIA (TURI + BARI + MONOPOLI + ALBEROBELLO + MATERA)

---

# **DÍA 1**: 
## Llegada al instituto ISS Pertini Anelli Pinto
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel').scrollBy({left: -document.getElementById('carrusel').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel">
    <img src="./images/DIA 1/IMG_20260113_091924.jpg" alt="Llegada">
    <img src="./images/DIA 1/IMG_20260113_092303.jpg" alt="Instituto">
    <img src="./images/DIA 1/IMG_20260113_093736.jpg" alt="Clase 1">
    <img src="./images/DIA 1/IMG_20260113_112640.jpg" alt="Clase 2">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel').scrollBy({left: document.getElementById('carrusel').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

## Visita a las Grutas de la Castellana
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel2').scrollBy({left: -document.getElementById('carrusel2').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel2">
    <img src="./images/DIA 1/IMG_20260113_162437.jpg" alt="Grutas 1">
    <img src="./images/DIA 1/IMG_20260113_162741.jpg" alt="Grutas 2">
    <img src="./images/DIA 1/IMG_20260113_164003.jpg" alt="Grutas 3">
    <img src="./images/DIA 1/IMG_20260113_170420.jpg" alt="Grutas 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel2').scrollBy({left: document.getElementById('carrusel2').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

---

# **DÍA 2**: 
## Visita al instituto ISS Pertini Anelli Pinto
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel3').scrollBy({left: -document.getElementById('carrusel3').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel3">
    <img src="./images/DIA 2/IMG_20260114_114941.jpg" alt="Instituto 1">
    <img src="./images/DIA 2/IMG_20260114_121732.jpg" alt="Instituto 2">
    <img src="./images/DIA 2/IMG_20260114_123308.jpg" alt="Instituto 3">
    <img src="./images/DIA 2/IMG_20260114_123312.jpg" alt="Instituto 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel3').scrollBy({left: document.getElementById('carrusel3').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

## Visita al pueblo de Monopoli
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel4').scrollBy({left: -document.getElementById('carrusel4').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel4">
    <img src="./images/DIA 2/IMG_20260114_153445.jpg" alt="Monopoli 1">
    <img src="./images/DIA 2/IMG_20260114_154315.jpg" alt="Monopoli 2">
    <img src="./images/DIA 2/IMG_20260114_154727.jpg" alt="Monopoli 3">
    <img src="./images/DIA 2/IMG_20260114_161100.jpg" alt="Monopoli 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel4').scrollBy({left: document.getElementById('carrusel4').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

---

# **DÍA 3**: 
## Último día en el instituto ISS Pertini Anelli Pinto
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel5').scrollBy({left: -document.getElementById('carrusel5').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel5">
    <img src="./images/DIA 3/IMG_20260115_110339.jpg" alt="Instituto 1">
    <img src="./images/DIA 3/IMG_20260115_110334.jpg" alt="Instituto 2">
    <img src="./images/DIA 3/IMG_20260115_105825.jpg" alt="Instituto 3">
    <img src="./images/DIA 3/IMG_20260115_105917.jpg" alt="Instituto 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel5').scrollBy({left: document.getElementById('carrusel5').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

## Visita a la ciudad de Bari
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel6').scrollBy({left: -document.getElementById('carrusel6').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel6">
    <img src="./images/DIA 3/IMG_20260115_143824.jpg" alt="Bari 1">
    <img src="./images/DIA 3/IMG_20260115_155458.jpg" alt="Bari 2">
    <img src="./images/DIA 3/IMG_20260115_162712.jpg" alt="Bari 3">
    <img src="./images/DIA 3/IMG_20260115_172909.jpg" alt="Bari 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel6').scrollBy({left: document.getElementById('carrusel6').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

---

# **DÍA 4**: 
## Visita a Alberobello
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel7').scrollBy({left: -document.getElementById('carrusel7').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel7">
    <img src="./images/DIA 4/IMG_20260116_095251.jpg" alt="Alberobello 1">
    <img src="./images/DIA 4/IMG_20260116_102348.jpg" alt="Alberobello 2">
    <img src="./images/DIA 4/IMG_20260116_102711.jpg" alt="Alberobello 3">
    <img src="./images/DIA 4/IMG_20260116_102958.jpg" alt="Alberobello 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel7').scrollBy({left: document.getElementById('carrusel7').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

## Visita a Matera
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel8').scrollBy({left: -document.getElementById('carrusel8').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel8">
    <img src="./images/DIA 4/IMG_20260116_144629.jpg" alt="Matera 1">
    <img src="./images/DIA 4/IMG_20260116_155335.jpg" alt="Matera 2">
    <img src="./images/DIA 4/IMG_20260116_162445.jpg" alt="Matera 3">
    <img src="./images/DIA 4/IMG_20260116_163129.jpg" alt="Matera 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel8').scrollBy({left: document.getElementById('carrusel8').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

---

# DÍA 5: 
## Último día en Italia y visita por Turi
<div class="slider-horizontal">
  <button class="boton-lateral" onclick="document.getElementById('carrusel9').scrollBy({left: -document.getElementById('carrusel9').offsetWidth, behavior: 'smooth'})">❮</button>

  <div class="visor-fotos" id="carrusel9">
    <img src="./images/DIA 5/IMG_20260117_100231.jpg" alt="Turi 1">
    <img src="./images/DIA 5/IMG_20260117_100246.jpg" alt="Turi 2">
    <img src="./images/DIA 5/IMG_20260117_100800.jpg" alt="Turi 3">
    <img src="./images/DIA 5/IMG_20260117_101053.jpg" alt="Turi 4">
  </div>

  <button class="boton-lateral" onclick="document.getElementById('carrusel9').scrollBy({left: document.getElementById('carrusel9').offsetWidth, behavior: 'smooth'})">❯</button>
</div>

---

<div style="text-align: center; margin-top: 100px; padding-bottom: 50px;">
  <h1>¡Gracias por vuestra atención!</h1>
  <p>Erasmus+VET 2025-2026</p>
</div>