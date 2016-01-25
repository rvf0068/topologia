---
layout: page
title: Inicio
date: 2016-01-25 
comments: true
published: true
categories: 
---

# Temario

1.  Espacios topológicos
    -   Definición de espacio topológico
    -   Base de una topología
    -   Ejemplos: topología del orden, topología de subespacio, producto.
    -   Funciones continuas
    -   Productos arbitrarios
    -   Metrizabilidad
    -   Topología cociente

2.  Conexidad y compacidad
    -   Conexidad
    -   Conexidad local
    -   Compacidad
    -   Compacidad local
    -   Conceptos relacionados: compacidad por puntos límite

3.  Axiomas de numerabilidad y separación
    -   Axiomas de numerabilidad
    -   Axiomas de separación
    -   Metrizabilidad, lema de Urysohn

# Exámenes

La calificación se obtendrá como el promedio de tres exámenes.

-   25 de febrero
-   7 de abril
-   2 de junio

# Presentaciones en pdf

-   25 de enero. [Topological spaces](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-01-25-topological-spaces.pdf?raw=true)

# Clases recientes

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </span>
    </li>
  {% endfor %}
</ul>
