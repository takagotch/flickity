### flickity
---
https://github.com/metafizzy/flickity

```
<script rel="stylesheet" href="https://unpkg.com/flickity@2/dist/flickity.min.css">
<script src="https://unpkg.com/flickity@2/dist/flickity.pkgd.min.js"></script>

<div class="carousel">
  <div class="carousel-cell"></div>
  <div class="carousel-cell"></div>
  <div class="carousel-cell"></div>
</div>
```

```
bower install flickity --save
npm install flickity --save
```

```js
var flky = new Flickity('', {
  accessibitlity: true,
  adaptiveHeight: false,
  autoPlay: false,
  cellAlign: 'center',
  cellSelector: undefined,
  contain: false,
  dragThreshold: 3,
  freeScroll: false,
  friction: 0.2,
  groupCells: false,
  initialIndex: 0,
  lazyLoad: true,
  percentPosition: true,
  prevNextButtons: true,
  pageDots: true,
  resize: true,
  rightToLeft: false,
  setGallertySize: true,
  watchCSS: false,
  wrapAround: false
});

var elem = document.querySelecto('.main-carousel');
var flkty = new Flickity( elem, {
  cellAlign: 'left',
  contain: true
});
var flkty = new Flickity('.main-carousel', {
});

var $carousel = $('.carousel').flickity()
  .flickity('next')
  .flickity( 'select', 4 );

var flkty = new Flickity('.carousel');
flkty.next();
flkty.select( 3 );

$carousel.flickity( 'select', index, isWrapped, isInstant )
flkty.selet( index, isWrapped, isInstant )

$('.button-group').on( 'click', '.button', function(){
  var index = $(this).index();
  $carousel.flickity( 'select', index );
});

$().on();

$carousel.flickity()
flkty.previous()

$().on();
$().on();

/*
https://flickity.metafizzy.co/api.html
*/

var $ = require('jquery');
var jQueryBridget = require('jquery-bridget');
var Flickity = require('flickity');
Flickity.setJQuery( $ );
jQueryBridget( 'flickity', Flickity, $ );
var $carousel = $('.carousel').flickity({...});

var $carousel = $('.carousel').flickity();
var flkty = $carousel.data('flickity');
console.log( flkty.selectedIndex, flkty.selectedElement );

flk.selectedIndex
flkty.selectedElement
flkty.selectedElements

slkty.cells
flkty.cells.length

flkty.slides
flkty.slides.length
```
