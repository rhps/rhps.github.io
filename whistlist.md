---
layout: default
title: Book Whislist
permalink: /whislist/
---

<h3>Book Whislist</h3>
Ada banyak buku yang menarik untuk dibaca, berikut adalah buku yang masuk kedalam daftar bacaan saya,
<br />
<br />

<table class="table">
  <thead>
    <tr>
      <th scope="col">Judul</th>
      <th scope="col">Rate by me</th>
    </tr>
  </thead>
  <tbody>
    {% for book in site.data.newbook %}
        {% if "" == book.Title %}
        {% else %}
            <tr>
                <td><a href="{{ book.Link }}" class="c-shelf__link">{{ book.Title }}</a></td>
                <td>
                <div style="font-size: 0.5rem">
                {% assign star = book.Rate %}
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
                </td>
            </tr>
        {% endif %}
    {% endfor %}
  </tbody>
</table>