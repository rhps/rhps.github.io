---
layout: post
title: "Flâneur Run"
description: ""
date: 2020-10-1
categories: 'notes'
inreview: true
tags: [running, Flâneur, photo]
permalink: /flanerunv2
comments: true
share: true
hidden: true
---

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial;
}

.header {
  text-align: center;
  padding: 32px;
}

.row {
  display: -ms-flexbox; /* IE10 */
  display: flex;
  -ms-flex-wrap: wrap; /* IE10 */
  flex-wrap: wrap;
  padding: 0 4px;
}

/* Create four equal columns that sits next to each other */
.column {
  -ms-flex: 25%; /* IE10 */
  flex: 25%;
  max-width: 25%;
  padding: 0 4px;
}

.column img {
  margin-top: 8px;
  vertical-align: middle;
  width: 100%;
}

/* Responsive layout - makes a two column-layout instead of four columns */
@media screen and (max-width: 800px) {
  .column {
    -ms-flex: 50%;
    flex: 50%;
    max-width: 50%;
  }
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .column {
    -ms-flex: 100%;
    flex: 100%;
    max-width: 100%;
  }
}

/* Lightbox */

.mfp-img {
 cursor: pointer; 
}

.mfp-force-scrollbars {
  &.mfp-wrap {
      overflow-y: auto !important;
      overflow-x: auto !important;
  }
  .mfp-img {
    max-width: none;
  }
  .mfp-close {
   position: fixed;
  }
  
}

</style>

<!-- <script>

$('a').magnificPopup({
		type: 'image',
		closeBtnInside: false,
    closeOnContentClick: false,
  
    callbacks: {
      open: function() {
        var self = this;
        self.wrap.on('click.pinhandler', 'img', function() {
          self.wrap.toggleClass('mfp-force-scrollbars');
        });
      },
      beforeClose: function() {
            this.wrap.off('click.pinhandler');
        this.wrap.removeClass('mfp-force-scrollbars');
      }
    },
     
    image: {
			verticalFit: false
		}
  
	});

</script> -->

<div class="header">
  <p>as a casual wanderer, observer and reporter of street-life in the modern city</p>
  <p>captured when run on the city</p>
</div>

<!-- Photo Grid -->
<div class="row"> 
  <div class="column">
    <img src="/images/gallery/wedding.jpg" style="width:100%">
    <img src="/images/gallery/rocks.jpg" style="width:100%">
    <img src="/images/gallery/falls2.jpg" style="width:100%">
    <img src="/images/gallery/paris.jpg" style="width:100%">
    <img src="/images/gallery/nature.jpg" style="width:100%">
    <img src="/images/gallery/mist.jpg" style="width:100%">
    <img src="/images/gallery/paris.jpg" style="width:100%">
  </div>
  <div class="column">
    <img src="/images/gallery/underwater.jpg" style="width:100%">
    <img src="/images/gallery/ocean.jpg" style="width:100%">
    <img src="/images/gallery/wedding.jpg" style="width:100%">
    <img src="/images/gallery/mountainskies.jpg" style="width:100%">
    <img src="/images/gallery/rocks.jpg" style="width:100%">
    <img src="/images/gallery/underwater.jpg" style="width:100%">
  </div>  
  <div class="column">
    <img src="/images/gallery/wedding.jpg" style="width:100%">
    <img src="/images/gallery/rocks.jpg" style="width:100%">
    <img src="/images/gallery/falls2.jpg" style="width:100%">
    <img src="/images/gallery/paris.jpg" style="width:100%">
    <img src="/images/gallery/nature.jpg" style="width:100%">
    <img src="/images/gallery/mist.jpg" style="width:100%">
    <img src="/images/gallery/paris.jpg" style="width:100%">
  </div>
  <div class="column">
    <img src="/images/gallery/underwater.jpg" style="width:100%">
    <img src="/images/gallery/ocean.jpg" style="width:100%">
    <img src="/images/gallery/wedding.jpg" style="width:100%">
    <img src="/images/gallery/mountainskies.jpg" style="width:100%">
    <img src="/images/gallery/rocks.jpg" style="width:100%">
    <img src="/images/gallery/underwater.jpg" style="width:100%">
  </div>
</div>

<a href="/images/gallery/wedding.jpg" data-lightbox="image-1" data-title="1978 Yamaha XS750">
  <img width="100" src="/images/gallery/wedding.jpg"/>
</a>
<a href="/images/gallery/wedding.jpg" data-lightbox="image-1" data-title="The Round Porch">
  <img width="100" src="/images/gallery/wedding.jpg"/>
</a>

<!-- <p>After you open lightbox, you can click on main image second time to enarge it even more.</p>
<a href="http://upload.wikimedia.org/wikipedia/commons/thumb/a/a3/Christmas_flood_1717.jpg/1280px-Christmas_flood_1717.jpg" class="with-caption image-link" title="Click on image to enlarge/reduce it">
  <img src="http://upload.wikimedia.org/wikipedia/commons/thumb/a/a3/Christmas_flood_1717.jpg/1280px-Christmas_flood_1717.jpg" width="172" height="105" />  
</a>

<script async src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script async src="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/jquery.magnific-popup.min.js"></script> -->






https://dimsemenov.com/plugins/magnific-popup/
https://www.smashingmagazine.com/2013/05/truly-responsive-lightbox/
https://dimsemenov.com/plugins/magnific-popup/documentation.html#zoom_effect
https://github.com/dimsemenov/Magnific-Popup/find/master
