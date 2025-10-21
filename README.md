# amity<!doctype html>

<html 
lang="en">

<head>

<meta 
charset="utf-8" />

<meta 
name="viewport" 
content="width=device-width, initial-scale=1" />

<title>Products & Services — Price List</title>

<meta 
name="description" 
content="Guitar services price list with details." />

<style>

/* --- Reset (light) --- */

*, 
*::before, 
*::after { 
box-sizing: border-box; }

html, 
body { height: 
100%; }

body { 
margin: 0; 
font-family: system-ui, 
-apple-system, "Segoe UI", Roboto,
Helvetica, 
Arial, "Apple Color Emoji", 
"Segoe UI Emoji"; line-height:
1.5; }



/* --- Layout / Theme --- */

:root{

--bg: #111;

--card: #181818;

--muted: #b8b8b8;

--text: #f5f5f5;

--accent: #ffffff;

--ring: 2px solid #6b6b6b;

--radius: 16px;

}

body{

background: var(--bg);

color: var(--text);

display: grid;

place-items: start center;

padding: 48px 16px 96px;

}

.wrap{

width: 100%;

max-width: 880px;

}



/* --- Header --- */

.brand{

display: grid;

place-items: center;

gap: 12px;

margin-bottom: 24px;

text-align: center;

}

.brand img{

width: 180px;

height: auto;

display: block;

filter: drop-shadow(0 10px 24px rgba(0,0,0,.45));

}

.brand .fallback{

width: 200px;

height: 80px;

border-radius: 12px;

background: linear-gradient(180deg, #222, #161616);

display: grid;

place-items: center;

color: var(--muted);

font-weight: 600;

letter-spacing: .6px;

text-transform: uppercase;

}

h1{

font-size: clamp(22px, 3.2vw, 34px);

margin: 0;

line-height: 1.15;

letter-spacing: .2px;

}

p.lede{

margin: 0;

color: var(--muted);

font-size: clamp(14px, 2.2vw, 16px);

}



.cta{

display: inline-block;

margin-top: 8px;

padding: 8px 14px;

background: #2a7ae2;

color: #fff;

text-decoration: none;

border-radius: 10px;

font-weight: 600;

box-shadow: 0 6px 18px rgba(42,122,226,.15);

}

.cta:hover{ filter: brightness(.98); }



/* --- Accordion --- */

.accordion{

margin-top: 28px;

background: var(--card);

border-radius: var(--radius);

overflow: hidden;

border: 1px solid #222;

box-shadow: 0 10px 30px rgba(0,0,0,.35);

}

.item + .item{ border-top: 1px solid #222; }



.trigger{

appearance: none;

width: 100%;

background: transparent;

color: inherit;

border: 0;

text-align: left;

padding: 18px 20px;

display: grid;

grid-template-columns: 1fr auto;

gap: 12px;

align-items: center;

font-size: 16px;

line-height: 1.3;

cursor: pointer;

}

.trigger:hover{ background: #1b1b1b; }

.trigger:focus-visible{

outline: none;

box-shadow: 0 0 0 3px rgba(255,255,255,.15) inset;

}

.title{

display: flex; gap: 10px; align-items: baseline; flex-wrap: wrap;

}

.price{

color: var(--accent);

font-weight: 600;

white-space: nowrap;

}

.chev{

transition: transform .2s ease;

font-size: 18px;

opacity: .9;

}

.trigger[aria-expanded="true"] .chev{ transform: rotate(90deg); }



.panel{

max-height: 0;

overflow: hidden;

transition: max-height .25s ease;

background: #151515;

border-top: 1px solid #202020;

}

.panel-inner{

padding: 16px 20px 22px;

color: var(--muted);

font-size: 15px;

}

.panel-inner ul{ margin: 8px 0 0 22px; }

.note{ color: #cfcfcf; }



/* --- Section labels (categories) --- */

.cat{

display: inline-block;

font-size: 12px;

letter-spacing: .06em;

text-transform: uppercase;

color: #ddd;

background: #242424;

border: 1px solid #2b2b2b;

padding: 4px 8px;

border-radius: 999px;

margin-right: 10px;

}



/* Footer */

footer{

color: var(--muted);

font-size: 13px;

text-align: center;

margin-top: 16px;

}



/* Reduced motion preference */

@media (prefers-reduced-motion: reduce) {

.panel { transition: none !important; }

.chev { transition: none !important; }

}

</style>

</head>

<body>

<main 
class="wrap" 
id="top">

<header 
class="brand" 
aria-label="Brand">

<!-- logo.svg should exist in repo; if it fails we'll show the fallback -->

<img 
src="logo.svg" 
alt="Brand Logo" 
onerror="(function(img){const
fb=document.querySelector('.fallback').cloneNode(true);fb.removeAttribute('hidden');img.replaceWith(fb);})(this)">

<div 
class="fallback" 
hidden>Your Logo</div>

<h1>Products & Services — Price List</h1>

<p 
class="lede">Tap a line to see what's included. Keyboard: ↑/↓ to move, Enter/Space to open.</p>

<a 
class="cta" 
href="https://calendar.google.com/calendar/r/eventedit?text=Amity+Instrument+Drop-off&details=Please+describe+your+instrument+and+preferred+drop-off+times.&location=Amity&sf=true"
target="_blank"
rel="noopener noreferrer">Schedule a drop-off</a>

</header>



<section class="accordion" id="price-accordion">

<!-- Jump the Line -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p0" id="t0">

<span class="title"><span class="cat">Jump the Line</span>Flat expedited service fee</span>

<span class="price">$150<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p0" role="region" aria-labelledby="t0" aria-hidden="true">

<div class="panel-inner">

Expedited service for most clients. Complimentary for <strong>Nels Cline</strong> and <strong>Bill Frisel</strong>.

</div>

</div>

</div>



<!-- Set-ups & Fret Levels -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p1" id="t1">

<span class="title"><span class="cat">Set-ups &amp; Fret Levels</span>Standard Guitars — Setup / with Fret Level</span>

<span class="price">$90 / $200<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p1" role="region" aria-labelledby="t1" aria-hidden="true">

<div class="panel-inner">

<ul>

<li><strong>Standard Guitars:</strong> $90 (<span class="note">with Fret Level, Recrown &amp; Polish: $200</span>)</li>

<li><strong>Other Instruments &amp; Complex Guitars:</strong> $100 (<span class="note">with FL/R&amp;P: $210</span>)</li>

<li><strong>Mandolin or Archtop (bridge fit):</strong> $110 (<span class="note">with FL/R&amp;P: $220</span>)</li>

<li><strong>Rickenbacker Bass/6-String</strong> (gloss board &amp; double truss): $125 (<span class="note">with FL/R&amp;P: $235</span>)</li>

<li><strong>Rickenbacker 12-String</strong> (gloss board &amp; double truss): $150 (<span class="note">with FL/R&amp;P: $260</span>)</li>

<li><strong>Steinberger TransTrem:</strong> $200 (<span class="note">with Fret Level: $320</span>)</li>

<li><strong>Buzz Feiten Retrofit (most Electrics):</strong> $200 (<span class="note">setup included; with FL: $310</span>)</li>

<li><strong>Buzz Feiten Retrofit (most Acoustics):</strong> $450 (<span class="note">with Fret Level add: $560</span>)</li>

</ul>

</div>

</div>

</div>



<!-- Restring & Tune -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p2" id="t2">

<span class="title"><span class="cat">Restring &amp; Tune</span>6/7-String, Banjo &amp; Uke / 12-String / Classical &amp; Mandolin / Floyd Rose</span>

<span class="price">$40–$60<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p2" role="region" aria-labelledby="t2" aria-hidden="true">

<div class="panel-inner">

<ul>

<li><strong>6-String, 7-String, Banjo &amp; Ukulele:</strong> $40 (<span class="note">with other work: $30</span>)</li>

<li><strong>12-String:</strong> $60 (<span class="note">with other work: $50</span>)</li>

<li><strong>Classical, Latin Instruments &amp; Mandolins:</strong> $50 (<span class="note">with other work: $40</span>)</li>

<li><strong>Floyd Rose Trem:</strong> $50 (<span class="note">with other work: $40</span>)</li>

</ul>

</div>

</div>

</div>



<!-- Restring & Adjust -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p3" id="t3">

<span class="title"><span class="cat">Restring &amp; Adjust</span>6/7-String, Banjo &amp; Uke / 12-String / Classical &amp; Mandolin / Floyd Rose</span>

<span class="price">$60–$80<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p3" role="region" aria-labelledby="t3" aria-hidden="true">

<div class="panel-inner">

<ul>

<li><strong>6-String, 7-String, Banjo &amp; Ukulele:</strong> $60 (<span class="note">with other work: $50</span>)</li>

<li><strong>12-String:</strong> $80 (<span class="note">with other work: $70</span>)</li>

<li><strong>Classical, Latin Instruments &amp; Mandolins:</strong> $70 (<span class="note">with other work: $60</span>)</li>

<li><strong>Floyd Rose Trem:</strong> $65 (<span class="note">with other work: $55</span>)</li>

</ul>

</div>

</div>

</div>



<!-- Nuts -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p5" id="t5">

<span class="title"><span class="cat">Nuts</span>Standard / Fender Style / Gibson-Style or Acoustic / 12-String</span>

<span class="price">$70–$200<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p5" role="region" aria-labelledby="t5" aria-hidden="true">

<div class="panel-inner">

<ul>

<li><strong>Standard Nut:</strong> $70 (<span class="note">with setup: $50</span>)</li>

<li><strong>Fender Style Nut:</strong> $110 (<span class="note">with setup: $90</span>)</li>

<li><strong>Gibson Style, Acoustic, or Fender w/ Binding:</strong> $200 (<span class="note">with setup: $100</span>)</li>

<li><strong>12-String Nut:</strong> $190 (<span class="note">with setup: $65</span>)</li>

<li><strong>Materials:</strong> graphite, brass, steel, etc. may add surcharge.</li>

</ul>

</div>

</div>

</div>



<!-- Guitar Bridge Work -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p6" id="t6">

<span class="title"><span class="cat">Bridge Work</span>Acoustic bridges, saddles, reglues</span>

<span class="price">$60–$300+<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p6" role="region" aria-labelledby="t6" aria-hidden="true">

<div class="panel-inner">

<ul>

<li><strong>Acoustic Guitar Bridges:</strong> $60</li>

<li><strong>Saddle, Hand-Crafted Bone:</strong> $85</li>

<li><strong>Saddle for 12-String:</strong> $235</li>

<li><strong>Bridge Remove &amp; Re-glue (Martin-style 6-string):</strong> $300+</li>

<li><strong>Bridge Reglue on Polyurethane Top (6-string):</strong> $250</li>

<li>Additional bridge services available on request.</li>

</ul>

</div>

</div>

</div>



<!-- Guitar Electronics -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p7" id="t7">

<span class="title"><span class="cat">Electronics</span>Diagnosis, pickups, routing, rewiring</span>

<span class="price">$25–$355<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p7" role="region" aria-labelledby="t7" aria-hidden="true">

<div class="panel-inner">

<ul>

<li><strong>Minimum bench/diagnosis fee:</strong> $25</li>

<li>Pickup installs, rewinds, routing, &amp; additional electronics work range from $25–$355 depending on complexity and parts.</li>

</ul>

</div>

</div>

</div>



<!-- Fret Work & Fingerboards -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p8" id="t8">

<span class="title"><span class="cat">Fret Work</span>Level &amp; re-crown, fret-end file, inlays</span>

<span class="price">$75–$165<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p8" role="region" aria-labelledby="t8" aria-hidden="true">

<div class="panel-inner">

<ul>

<li><strong>Full Fret Level &amp; Re-Crown (basic 6-string):</strong> $165 (<span class="note">with setup: $120</span>)</li>

<li><strong>Fret-End File:</strong> $75 (<span class="note">with setup: $50</span>)</li>

<li><strong>Refret:</strong> $250 (<span class="note">w/ binding +$100</span>)</li>

<li>Additional fingerboard inlay and specialty fret services available; pricing varies.</li>

</ul>

</div>

</div>

</div>



<!-- Necks -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p9" id="t9">

<span class="title"><span class="cat">Necks</span>Mounting, truss work, heat set, resets</span>

<span class="price">Varies<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p9" role="region" aria-labelledby="t9" aria-hidden="true">

<div class="panel-inner">

Neck mounting, truss rod replacement, heat setting, and full neck resets available with detailed, instrument-specific pricing.

</div>

</div>

</div>



<!-- Cracks & Structural Repairs -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p10" id="t10">

<span class="title"><span class="cat">Structural</span>Cracks, splints, headstock repairs</span>

<span class="price">Varies<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p10" role="region" aria-labelledby="t10" aria-hidden="true">

<div class="panel-inner">

Sealing, repairing, and splinting cracks; headstock repairs and other structural work quoted after inspection.

</div>

</div>

</div>



<!-- Paint & Touch-Up -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p11" id="t11">

<span class="title"><span class="cat">Finish</span>Buffing, wet-sand, polish, touch-ups &amp; refinish</span>

<span class="price">Varies<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p11" role="region" aria-labelledby="t11" aria-hidden="true">

<div class="panel-inner">

Buffing, wet sanding, polishing, localized touch-ups, finish repairs, and full refinishes available upon evaluation.

</div>

</div>

</div>



<!-- Add-Ons (moved to bottom) -->

<div class="item">

<button class="trigger" aria-expanded="false" aria-controls="p4" id="t4">

<span class="title"><span class="cat">Add-Ons</span>Small adjustments &amp; add-ons</span>

<span class="price">$15–$75<span class="chev" aria-hidden="true">›</span></span>

</button>

<div class="panel" id="p4" role="region" aria-labelledby="t4" aria-hidden="true">

<div class="panel-inner">

Various add-ons and adjustments are available; pricing depends on scope and parts. Typical minor tweaks fall between $15 and $75.

</div>

</div>

</div>



</section>



<footer>

<p>Questions or custom work? Contact us with your instrument details for an exact quote.</p>

</footer>

</main>



<script>

// Accessible accordion: toggle, focus movement (↑/↓), Home/End, and close-others behavior.

(function(){

const 
triggers = Array.from(document.querySelectorAll('.trigger'));

const 
panels = 
new Map(triggers.map(btn
=> [btn, document.getElementById(btn.getAttribute('aria-controls'))]));



function 
collapseAll(exceptBtn){

triggers.forEach(btn
=> {

if(btn 
!== exceptBtn){

btn.setAttribute('aria-expanded','false');

const 
panel = panels.get(btn);

// animate close reliably: set explicit current height then 0

panel.style.maxHeight = panel.scrollHeight
+ 
'px';

// force reflow

panel.offsetHeight;

panel.style.maxHeight = 
'0';

panel.setAttribute('aria-hidden',
'true');

}

});

}



function 
openPanel(btn){

const 
panel = panels.get(btn);

panel.setAttribute('aria-hidden',
'false');

// set to exact height to animate

panel.style.maxHeight = panel.scrollHeight
+ 
'px';

// when transition finishes, allow natural height

const 
onEnd = (e)
=> {

if (e.target 
!== panel || e.propertyName 
!== 'max-height') 
return;

// remove explicit max-height so content can grow/shrink naturally

panel.style.maxHeight = 
'none';

panel.removeEventListener('transitionend', onEnd);

};

panel.addEventListener('transitionend', onEnd);

}



function 
closePanel(btn){

const 
panel = panels.get(btn);

panel.setAttribute('aria-hidden',
'true');

// if currently 'none', set to actual scrollHeight first to animate to 0

panel.style.maxHeight = panel.scrollHeight
+ 
'px';

// force reflow

panel.offsetHeight;

panel.style.maxHeight = 
'0';

}



function 
toggle(btn){

const 
isOpen = btn.getAttribute('aria-expanded')
=== 
'true';

if(!isOpen){
collapseAll(btn); }

const 
newVal = 
String(!isOpen);

btn.setAttribute('aria-expanded', newVal);

const 
panel = panels.get(btn);

if(!isOpen){

openPanel(btn);

}else{

closePanel(btn);

}

}



// initialize closed

triggers.forEach(btn
=> {

btn.setAttribute('aria-expanded','false');

const 
panel = panels.get(btn);

panel.setAttribute('aria-hidden',
'true');

panel.style.maxHeight = 
0;



btn.addEventListener('click', ()
=> 
toggle(btn));

btn.addEventListener('keydown', (e)
=> {

const 
idx = triggers.indexOf(btn);

switch(e.key){

case 
'ArrowDown':

e.preventDefault();

(triggers[idx + 
1] || triggers[0]).focus();

break;

case 
'ArrowUp':

e.preventDefault();

(triggers[idx - 
1] || triggers[triggers.length
- 
1]).focus();

break;

case 
'Home':

e.preventDefault();

triggers[0].focus();

break;

case 
'End':

e.preventDefault();

triggers[triggers.length 
- 1].focus();

break;

case 
'Enter':

case 
' ':

e.preventDefault();

toggle(btn);

break;

}

});

});



// Recompute max-heights on resize for open items

let resizeTimer 
= null;

window.addEventListener('resize', ()
=> {

clearTimeout(resizeTimer);

resizeTimer = 
setTimeout(() => {

triggers.forEach(btn
=> {

if(btn.getAttribute('aria-expanded')
=== 
'true'){

const 
panel = panels.get(btn);

// if we removed maxHeight (none), temporarily set to scrollHeight to avoid visual jump

panel.style.maxHeight = panel.scrollHeight
+ 
'px';

// then after a tick, clear maxHeight so content can flow (keeps open state)

setTimeout(() 
=> { panel.style.maxHeight = 
'none'; }, 250);

}

});

}, 100);

});



// Close all when clicking outside (optional UX)

document.addEventListener('click', (e)
=> {

if (!e.target.closest('.accordion')) {

collapseAll(null);

}

});

})();

</script>

</body>

</html>
