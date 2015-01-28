1. Ladda ner jQuery

Ladda ner jQuery HÄR och inkludera det i <head> på din webbsida.


2. Ladda ner MegaSlider från GitHub

Ladda hem MegaSlider från GitHub HÄR. Inkludera filen megaslider.js samt megaslider-style.css i <head>. Så här till exempelt:

<head>
<script src='megaslider.js'>
<link rel='stylesheet' type='text/css' href='megaslider-style.css'/>
</head>

OBS! MegaSlider måste inkluderas efter jQuery.


3. HTML-kod

För att MegaSlider skall fungera och se ut som det är tänkt krävs följande HTML-kod:

<div id="slide-wrapper">

<!-- Slide images -->
<div id ="slideimages">
<div id="slideimg1" class="slideimg"></div>
<div id="slideimg2" class="slideimg"></div>
</div>

<!-- slide-text -->
<div id="slide-text">
<h1 id="firstline"></h1>
<p><a href="#" id="secondline"></a></p>
</div>

<!-- Slideshow controls -->
<div id ="controls-outer">
<div id ="controls">
<div id="back" class="btn"></div>
<div id="control" class="btn"></div>
<div id="next" class="btn"></div>
</div>
</div>

</div>


4. Ange bilder och texter

Ange bilder och texter som du vill ha med i din slideshow genom att lägga in och redigera denna kod:

<script>
var photos = [{
"title" : "Title 1",
"image" : "http://lorempixel.com/g/1920/1920/nightlife/5/",
"url" : "http://www.exempel.se/",
"firstline" : "Lorem ipsum",
"secondline" : "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
}, {
"title" : "Title 2",
"image" : "http://lorempixel.com/g/1920/1920/nightlife/2/",
"url" : "http://www.exempel.se/",
"firstline" : "Lorem ipsum",
"secondline" : "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
}];
var slideshowSpeed = 9000;
</script>


(OBS! denna kod skall läggas in innan raden där du inkluderar filen megaslider.js)
title = bildens titel
image = sökvägen till bilden
url = sökvägen dit du vill länka texten för secondline
firstline = Rubriken till texten som syns samtidigt som bilden secondline = Texten som syns samtidigt som bilden. (Denna text blir även en länk till den adress du anger för url.
slideshowSpeed = Här anger du hur lång tid varje bild ska visas. Vill du ha fler än två bilder kopierar du bara koden mellan { och } och klistrar in den innan ];.


5. Om du vill ha bakgrundsmusik?

<!-- Background music -->
<audio autoplay loop id="music">
<source src="sound/phoney.mp3">
Your browser does not support HTML5 audio.
</audio>

<!-- Control for background music -->
<div id="sound">
<img id="sound-control" src="img/ljud_pa.png" alt=""/>
</div>
</div>