---
title: "Galería de Imágenes"
date: 2024-11-21
---

# Imágenes de Mi Pueblo

Aquí hay algunas fotos de mi pueblo. ¡Espero que las disfruten!

<div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    {{ range .Site.Data.images }}
      <div class="carousel-item {{ if eq .Params.index 0 }}active{{ end }}">
        <img src="{{ .src }}" class="d-block w-100" alt="Imagen">
      </div>
    {{ end }}
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
