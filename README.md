### flickity
---
https://github.com/metafizzy/flickity

```html
<script rel="stylesheet" href="https://unpkg.com/flickity@2/dist/flickity.min.css">
<script src="https://unpkg.com/flickity@2/dist/flickity.pkgd.min.js"></script>

<div class="carousel">
  <div class="carousel-cell"></div>
  <div class="carousel-cell"></div>
  <div class="carousel-cell"></div>
</div>
```

```sh
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

$('button-group').on('click', '.button', function(){
  var index = $().index();
  $carousel.flickity( 'select', index, false, true );
});

$carousel.flickity( 'previous', isWrapped, isInstant )
flikty.previous( isWrapped, isInstant )

$('.button--previous').on('click', function(){
  $carousel.flickity('previous');
});
$('.button--previsou-wrapped').on('click', function(){
  $carousel.flickity('previous', true );
});
  
$carousel.flickity('next', isWapped, isInstant )
flkty.next( isWrapped, isInstant )

$('.button--next').on('click', function(){
  $carousel.flickity('next');
});
$('.button--next-wrapped').on('click', function(){
  $carousel.flickity('next', true );
});

$carousel.flickity( 'selectCell', value, isWrapped, isInstant )
flkty.selectCell( value, isWrapped, isInstant )

$('.button-group').on('click', '.button', function(){
  var index = $(this).index();
  $carousel.flickity( 'selectCell', index);
});

$carousel.flickity('selectCell', '.cell2');

$carousel.flickity('resize')
flkty.resize()

$('.button--resize').on('click', function(){
  $carousel.toggleClass('is-expanded')
    .flickity('resize');
});

$('.button').on('click', function(){
  $carousel.show()
     .flickity('resize');
});

$carousel.flickity('respoition')
flikty.reposition()

$carousel.on('staticClick', function( event, pointer, cellElement, cellindex){
  if( !cellElement ){
    return;
  }
  $( cellElement ).toggleClass('is-expended');
  $carousel.flickity('reposition');
});

$carousel.flickity( 'append', elements )
flkty.prepend( elements )
$('.button').on('click', function(){
  var $cellElems = $('<div class="carousel-cell">...</div>');
  $carousel.flickity( 'prepend', $cellElems );
});

$carousel.flickity( 'append', elements )
flkty.append( elements )

$('.button').on('click', function(){
  var $cellElems = $('<div class="carousel-cell"></div>');
  $carousel.flickity( 'append', $cellElems );
});

$carousel.flickity( 'insert', elements, index )
flkty.insert( elements, index )
$('.button').on('click', function(){
  var $cellElems = $('<div class="carousel-cell"></div>');
  $carousel.flickity('insert', $cellElems, 1 );
});


/*
https://flickity.metafizzy.co/api.html
*/
Flickity.setJQuery( $ )
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

```css
.carousel { width: 50%; }
.carousel.is-expanded { width: 100%; }
.carousel.is-expanded .carousel-cell{
  height: 320px;
}
```

```js
$('.main-carousel').flickity({
  cellAlign: 'left',
  contain: true
});

var elem = document.querySelector('.main-carousel');
var flkty = new Flicktiy( elem, {
  cellAlign: 'left',
  contain: true
});

var flkty = new Flickity( '.main-carousel', {
  // option
});

$carousel.flicktity( 'prepend', elements )

flikty.prepend( elements )

$('.button').on( 'click', function() {
  var $vellElems = $('<div class="carousel-cell">...</div>');
  $carousel.flickity( 'prepend', $cellElems );
});

```
