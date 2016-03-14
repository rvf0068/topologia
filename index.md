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
-   26 de enero. [Bases](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-01-26-bases.pdf?raw=true)
-   28 de enero. [Bases and subbases](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-01-28-bases-and-subbases.pdf?raw=true)
-   1 de febrero. [The order topology](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-01-order-topology.pdf?raw=true)
-   2 de febrero. [Subspaces](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-02-subspaces.pdf?raw=true)
-   4 de febrero. [Products](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-04-products.pdf?raw=true)
-   8 de febrero. [Closed sets](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-04-closed-sets.pdf?raw=true)
-   9 de febrero. [Closure and interior](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-09-closure-and-interior.pdf?raw=true)
-   11 de febrero. [Hausdorff spaces](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-11-hausdorff-spaces.pdf?raw=true)
-   15,16 de febrero. [Continuous functions](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-15-continuous-functions.pdf?raw=true)
-   18 de febrero. [Constructing continuous functions](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-02-18-constructing-continuous-functions.pdf?raw=true)
-   7 de marzo. [Arbitrary products](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-03-07-arbitrary-products.pdf?raw=true)
-   14 de marzo. [Metric topology](https://github.com/rvf0068/topologia/raw/gh-pages/pdfs/2016-03-14-metric-topology.pdf?raw=true)

# Textos

-   Munkres. *Topology: a first course*
-   Conway. *A Course in Point Set Topology* <http://link.springer.com/book/10.1007/978-3-319-02368-7>
-   Crossley. *Essential topology* <http://link.springer.com/book/10.1007/1-84628-194-6>
-   Manetti. *Topology* <http://link.springer.com/book/10.1007/978-3-319-16958-3>
-   Runde. *A Taste of Topology* <http://link.springer.com/book/10.1007/0-387-28387-0>

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
