---
layout: post
title: "The Summits"
description: ""
date: 2021-06-15
categories: 'summit'
inreview: true
tags: [summit, hiking, adventure]
permalink: /thesummits
comments: true
share: true
hidden: true
---

Hobby hiking dan menulislah yang menghasilkan tulisan ini. Sejak 2019, setiap hiking ke suatu tempat, agar tidak menjadi sebuah kenangan semata, satu-persatu perjalan tersebut ditulis dihalaman ini. Beberapa foto juga dilampirkan, agar dunia bisa tahu bahwa gunung-gunung di Indonesia begitu Indah. Setiap perjalanan akan diusahakan dilengkapi dengan file trek GPS yang bisa dipergunakan untuk panduan para pendaki ketika pendakian.

Tidak ada tekanan, tidak ada paksaan, tergantung ajakan kemana kesitulah kaki melangkah. Tidak ada target harus menyelesaikan atau mendaki kemana, biarlah semua berjalan perlahan-lahan.

<div>
{% if site.posts.size == 0 %}
  <h2>No post found</h2>
{% else %}
  {% for post in site.posts %}
    {% if post.summit == true and post.hidden == false %}
    <div class="wow  fadeIn animated" data-wow-delay=".15s" style="visibility: visible; animation-delay: 0.15s; animation-name: fadeIn;">
      {% if post.link %}
        <a href="{{ post.link }}" class="project card text-themed">
      {% else %}
        <a href="{{ post.url | prepend: site.baseurl }}" class="project card text-themed">
      {% endif %}
        <img id="the-fabulous-img" class="card-img-top" src="{{ post.picture }}" alt="{{ post.title }}"><div class="card-body">
          <div class="list-post-date">
            <time>{{ post.hikingdate }}</time>
          </div>
          {% if post.nfi == true %}
          <div id="the-fabulous-name" class="card-title">{{ post.title }} ~ Not Finished/Incomplete</div>
          {% else %}
          <div id="the-fabulous-name" class="card-title">{{ post.title }}</div>
          {% endif %}
          <p id="the-fabulous-desc" class="card-text">{{ post.description }}</p>
          <p id="the-fabulous-tools" class="card-text">
            <span class="badge badge-pill text-primary border border-primary ml-1">Lokasi: {{ post.location }}, {{ post.province }}</span>
            <span class="badge badge-pill text-primary border border-primary ml-1">Ketinggian: {{ post.mdpl }} mdpl</span>
          </p>
        </div>
      </a>
    </div>
    {% else %}
      {% continue %}
    {% endif %}
    <br/>
  {% endfor %}
</div>
{% endif %}

<!-- <table class="table">
  <thead class=".thead-light">
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nama</th>
      <th scope="col">Tinggi (mdpl)</th>
      <th scope="col">Lokasi</th>
      <th scope="col">Summits</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">14</th>
      <td>Gunung Rinjani</td>
      <td>3727</td>
      <td>Nusa Tenggara Barat, Lombok Timur</td>
      <td>Mei 2021</td>
    </tr>
    <tr>
      <th scope="row">13</th>
      <td>Gunung Agung (NFI)</td>
      <td>3031</td>
      <td>Bali, Karangasem</td>
      <td>April 2021</td>
    </tr>  
    <tr>
      <th scope="row">12</th>
      <td>Aling-Aling Waterfall</td>
      <td>~1000</td>
      <td>Bali, Singaraja</td>
      <td>April 2021</td>
    </tr>
    <tr>
      <th scope="row">11</th>
      <td>Gunung Gede</td>
      <td>2958</td>
      <td>Jawa Barat, Bogor</td>
      <td>Maret 2021</td>
    </tr>
    <tr>
      <th scope="row">10</th>
      <td>Gunung Dempo (NFI)</td>
      <td>3173</td>
      <td>Sumatera Selatan, Pagar Alam</td>
      <td>Februari 2021</td>
    </tr>
    <tr>
      <th scope="row">9</th>
      <td>Gunung Patuha</td>
      <td>2433</td>
      <td>Jawa Barat, Bandung Kabupaten</td>
      <td>Februari 2021</td>
    </tr>
    <tr>
      <th scope="row">8</th>
      <td>Gunung Sumbing</td>
      <td>3371</td>
      <td>Jawa Tengah, Wonosobo</td>
      <td>Januari 2021</td>
    </tr>
    <tr>
      <th scope="row">7</th>
      <td>Gunung Slamet</td>
      <td>3428</td>
      <td>Jawa Tengah, Purbalingga</td>
      <td>Desember 2020</td>
    </tr>
    <tr>
      <th scope="row">6</th>
      <td>Gunung Prau</td>
      <td>2565</td>
      <td>Jawa Tengah, Wonosobo</td>
      <td>Desember 2020</td>
    </tr>
    <tr>
      <th scope="row">5</th>
      <td>Gunung Papandayan</td>
      <td>2666</td>
      <td>Jawa Barat, Garut</td>
      <td>Desember 2020</td>
    </tr>
    <tr>
      <th scope="row">4</th>
      <td>Gunung Ciremai</td>
      <td>3078</td>
      <td>Jawa Barat, Majalengka</td>
      <td>November 2020</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Sesar Lembang</td>
      <td>~1900</td>
      <td>Jawa Barat, Lembang</td>
      <td>November 2020</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Curug Siliwangi 4</td>
      <td>~1290</td>
      <td>Jawa Barat, Bandung Selatan</td>
      <td>November 2020</td>
    </tr>
    <tr>
      <th scope="row">1</th>
      <td>Sesar Lembang (NFI)</td>
      <td>~1900</td>
      <td>Jawa Barat, Lembang</td>
      <td>October 2020</td>
    </tr>
    </tbody>
</table> -->