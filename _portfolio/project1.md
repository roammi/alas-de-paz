---
title: Programa Apoyo Escolar
subtitle: Educación Inicial y nivelación escolar
image: assets/img/portfolio/educacion1.png

caption:
  title:  Apoyo escolar educación inicial
  subtitle: Nivelación académica 
  thumbnail: assets/img/portfolio/educacion3.png
---

{:.list-inline}
- Apoyo escolar especializado
- Volando alto

---
Nuestro objetivo es que los niños desde la etapa inicial, sean desarrollados con una educación integral, que les permita contar con cimientos sólidos para una vida exitosa.
---

title: Apoyo personalizado
subtitle: Continuo y lúdico
image: assets/img/portfolio/educacion4.png

---

{:.list-inline}
- Apoyo escolar
- Centro de Excelencia académica
- Año: 2025
---
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Carrusel Automático</title>
  <!-- Enlace al CSS -->
  <link rel="stylesheet" href="css/style.css">
</head>
<body>

  <!-- Carrusel -->
  <div class="carousel">
    <div class="slides">
      <img: src="assets/img/portfolio/educacion1.png">
      <img: src="assets/img/portfolio/educacion3.png">
      <img: src="assets/img/portfolio/educacion4.png">
      <img: src="assets/img/portfolio/educacion5.png">
    </div>
  </div>

  <!-- Enlace al JS -->
  <script src="js/script.js"></script>
</body>
</html>
/* Estilos básicos */
* {box-sizing: border-box;}
body {font-family: Arial, sans-serif; margin: 0; padding: 0;}

/* Contenedor principal */
.carousel {
  position: relative;
  max-width: 800px;
  margin: 40px auto;
  overflow: hidden;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
}

/* Contenedor de las diapositivas */
.slides {
  display: flex;
  width: 100%;
  transition: transform 1s ease-in-out;
}

/* Cada imagen */
.slides img {
  width: 100%;
  flex-shrink: 0;
}
const slides = document.querySelector('.slides');
const totalSlides = document.querySelectorAll('.slides img').length;
let index = 0;

function showNextSlide() {
  index++;
  if (index >= totalSlides) index = 0;
  slides.style.transform = `translateX(${-index * 100}%)`;
}

setInterval(showNextSlide, 3000); // cambia cada 3 segundos
