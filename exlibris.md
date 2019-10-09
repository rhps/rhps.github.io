---
layout: default
title: Ex Libris
permalink: /exlibris/
---
<h3>Ex Libris</h3>
Rekomendasi dan ulasan dari beberapa buku yang pernah dibaca.
<ul class="c-shelf">
  {% for book in site.data.books %}
    <li class="c-shelf__volume book-item">
      <a href="{{ book.Post }}" class="c-shelf__link">
        <figure class="c-cover book-figure">
            <img src="{{ book.Image }}?w=250&amp;h=400&amp;fit=crop&amp;q=50&amp;auto=format" alt="{{ book.Title}}"/>
        </figure>
        <div style="font-size: 0.5rem">
          {% assign star = book.Rating %}
          {% case star %}
            {% when 1 %}
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
            {% when 2 %}
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>              
            {% when 3 %}
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
            {% when 4 %}
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star fa-xs"></i>
            {% when 5 %}
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
              <i class="fa fa-star checked fa-xs"></i>
            {% else %}
              ...unrated...
          {% endcase %}
        </div>
        <h2 class="c-shelf__volume__title">{{ book.Title }} - {{ book.Writer }}</h2>
      </a>
    </li>
  {% endfor %}
</ul>