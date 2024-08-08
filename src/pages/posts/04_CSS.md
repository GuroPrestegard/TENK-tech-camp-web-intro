---
layout: ../../layouts/post.astro
title: "CSS"
description: "CSS"
author: "gurop"
excerpt: CSS er korleis innhaldet på nettsida skal sjå ut. Om ein tekst er oransje, fet eller kursiv, eller om bakgrunnen på nettsida er kvit eller svart, alt det kan styrast av CSS. 
image:
  src:
  alt:
tags: ["nivå3"]
---

### Innhald

- [Oppgave 1](#oppgave-1)
- [Oppgave 1.5](#oppgave-1.5)
- [Oppgave 2](#oppgave-2)
- [Oppgave 3](#oppgave-3)
- [Oppgave 4](#oppgave-4)
- [Oppgave 5](#oppgave-5)
- [Oppgave 6](#oppgave-6)
- [Oppgave 7](#oppgave-7)
- [Oppgave 8](#oppgave-8)
- [Oppgave 9](#oppgave-9)

## Kva er CSS?
Mens HTML vert brukt for å gruppere innhold i tags, litt som om at du puttar alt innhaldet ditt i boksar som du skriv kva dei
inneheld utanpå, så er CSS korleis innhaldet skal sjå ut.

Om ein tekst er <font color="#EA580C">oransje</font>, **fet** eller _kursiv_, eller om bakgrunnen på nettsida er kvit
eller svart, alt det kan styrast av CSS.

Man kaller ofte CSS for styling, og man setter styling for dei forskjellige HTML-elementa man har tilgjengelig.
```css
p {
  color: pink;
}
```

I eksempelet over seier me at alle tags av typen p skal ha fargen rosa. 
p (paragraf, som me såg i HTML-biten) er typen element du vil treffe, og så er alt du skriv inni krøllparantesene {} den stylingen elementet får.
For å skrive krøllparanteser på mac, brukar du option+shift+8 og option+shift+9.
For å skrive krøllparanteser på windows, brukar du altgr+7 og altgr+0.

Man kan sette styling på tags, slik som over, men og på klasser og id-er man har gitt til tags.

#### Klasser
Klasser settes på html-tags ved å skrive ```class="et-superbra-klassenavn"``` som vist over. Her kan du f.eks lagre styling som 
du har lyst til å bruke på fleire elementer. Du skriver css som treffer klasser-er med ``.``, f.eks ``.et-superbra-klassenavn``. 

Html:
```html
<p class="et-superbra-klassenavn">Dette er eit avsnitt</p>
```

Css:
```css
.et-superbra-klassenavn {
    color: orange
}
```

#### ID-er
Id-er settes på html-tags ved å skrive ``id="et-superbra-id-navn"``. Ein ID høyrer kun til **eitt** element, og kan brukes til 
å style det spesifikke elementet. Du skriver css som treffer Id-er med ``#``, f.eks ``#et-superbra-id-navn``.

html:
```html
<p id="et-superbra-id-navn">Dette er eit avsnitt</p>
```

css: 
```css
#et-superbra-id-navn {
   font-weight: bold 
}
```

NB! navn på klasser og Id-er kan ikkje ha mellomrom i seg. Bruk ``-`` i staden for. 


<p class="codepen" data-height="300" data-default-tab="html" data-slug-hash="OJYgJGM" data-pen-title="HTMLCSS" data-user="gurop" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/gurop/pen/OJYgJGM">
  HTMLCSS</a> by AnoymousCat (<a href="https://codepen.io/gurop">@gurop</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


---

<article class="oppgave">
    <h4 id="oppgave-1">Oppgave 1</h4>
    <p><em>Legg til litt styling på teksten på nettsiden din</em></p>
    <ul>
      <li>F.eks legg til farge på teksten</li>
      <li>Gjer tekst "fet"</li>
      <li>Lag bakgrunnsfarge</li>
      <li>Klarar du å lage ei ramme rundt teksten?</li>
    </ul>
</article>

---

<p class="codepen" data-height="300" data-default-tab="css,result" data-slug-hash="gOJGXgK" data-pen-title="Untitled" data-editable="true" data-user="gurop" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/gurop/pen/gOJGXgK">
  Untitled</a> by AnoymousCat (<a href="https://codepen.io/gurop">@gurop</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

---

<article class="oppgave">
    <h4 id="oppgave-1.5">Oppgave 1.5</h4>
    <p><em>Leik deg litt med dei forskjellige elementa i kodeeksempelet over</em></p>
</article>

---

### Bilder
Her ser du eit bilete av ein hund, som eigentleg er firkanta. Men, ved hjelp av CSS har det blitt rundt. Dette fungerar 
best med bileter som er heilt kvadratiske. 
<div>
<img class="rounded" src="https://vetericyn.com/Vetericyn/wp-content/uploads/2024/04/Benefits-of-Chondroitin-for-Dogs-350x350.jpg" alt="ein hund" width="350" height="350">
</div>

html:
```html
<img src="https://vetericyn.com/Vetericyn/wp-content/uploads/2024/04/Benefits-of-Chondroitin-for-Dogs-350x350.jpg" alt="ein hund" width="350" height="350">
```
<article class="oppgave">
    <h4 id="oppgave-2">Oppgave 2</h4>
    <p><em>Lag ei side med eit bilde</em></p>
    <ul>
      <li>Gi biletet runde kantar ved å bruke "border-radius". Verdien vert satt i prosent </li>
    </ul>
</article>

---

Her har me tatt bildet frå i stad, og gjort det svart-kvitt. 
<div>
<img class="rounded filter"  src="https://vetericyn.com/Vetericyn/wp-content/uploads/2024/04/Benefits-of-Chondroitin-for-Dogs-350x350.jpg" alt="ein hund" width="350" height="350">
</div>

<article class="oppgave">
    <h4 id="oppgave-3">Oppgave 3</h4>
    <p><em>Lag ei side med eit bilde</em></p>
    <ul>
      <li>Gjer biletet svart-kvitt ved å bruke "filter". </li>
      <li>Se dokumentasjonen på filter <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/filter">her</a>.</li>
    </ul>
</article>


---

Her har me tatt bildet frå i stad, og gjort det opp-ned.
<div>
<img class="rounded filter updown"  src="https://vetericyn.com/Vetericyn/wp-content/uploads/2024/04/Benefits-of-Chondroitin-for-Dogs-350x350.jpg" alt="ein hund" width="350" height="350">
</div>

<article class="oppgave">
    <h4 id="oppgave-4">Oppgave 4</h4>
    <p><em>Lag ei side med eit bilde</em></p>
    <ul>
      <li>Gjer biletet opp-ned ved å bruke "rotate"</li>
      <li>Se dokumentasjonen på rotate <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/rotate">her</a>.</li>
    </ul>
</article>

---

Her har me tatt bildet frå i stad, og skrive CSS som gjer at det snurra rundt når du held musa over det. For å style når
nokon held musa over noko, brukar me :hover. For eksempel om nokon held musa over ein p-tag, kan me bruke

Css:
```css
p:hover {
color: blue;
}
```
<div>
<img class="rounded filter rotate"  src="https://vetericyn.com/Vetericyn/wp-content/uploads/2024/04/Benefits-of-Chondroitin-for-Dogs-350x350.jpg" alt="ein hund" width="350" height="350">
</div>

<article class="oppgave">
    <h4 id="oppgave-5">Oppgave 5 (Vanskelig! det er lov å hoppe over)</h4>
    <p><em>Lag ei side med eit bilde</em></p>
    <ul>
      <li>Få biletet til å snurre når du bevegar musa over!</li>
      <li>(Det treng ikkje å vera likt som her, så lenge det er bevegelse av eit slag)</li>
      <li>Du må gjerne google, eller spørre om hjelp!</li>
      <li>Bruk <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/transition">transition</a>, <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/transform">transform</a> og selectoren <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/:hover">:hover</a></li>
    </ul>
</article>

---

Du kan fortsette til neste delen, eller jobbe med ekstra oppgavene under hvis du
liker å jobbe mer med CSS.

[Gå til neste del: Avansert HTML](/TENK-tech-camp-web-intro/posts/05_HTML_plus)

---

## Ekstra oppgaver

### Plassering & FlexBox

Om du vil lese meir om Flexbox, ta ein kikk <a href="https://css-tricks.com/snippets/css/a-guide-to-flexbox/">her</a>. 

Noko av det som vert mest brukt innan CSS, er korleis ein plasserar elementa sine på sida. Flexbox er ein av dei enklaste
måtane å gjere det på, og hjelper deg å plassere ting i relasjon til kvarandre.

Konseptet med Flexbox er at du har ein container (behaldar), og inni den har du children (barn/underelementer). Containeren
er ansvarleg for å plassere sine children/underelementer, men children har også mulighet til å plassere seg sjølv. 

For å markere eit html-element med at du vil bruke Flexbox, skriv me CSS-en slik: 

CSS:
```css
.container {
    display: flex;
}
```
Eit HTML-utgangspunkt for å jobbe med Flexbox kan sjå ut som eksempelet i Codepen under. Der har du ein container, og tre underelementer (children).
Alle elementa har fått ein klasse, i tillegg har kvart av underelementa fått sin eigen id, slik at dei kan få forskjellige fargar. 

<p class="codepen" data-height="300" data-default-tab="css,result" data-slug-hash="LYozWrq" data-pen-title="Untitled" data-editable="true" data-user="gurop" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/gurop/pen/LYozWrq">
  Untitled</a> by AnoymousCat (<a href="https://codepen.io/gurop">@gurop</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

---

CSS:
```css title="Forskjellige verdiar man kan bruke på flexbox-properties"
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right;
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start;
  flex-direction: row | row-reverse | column | column-reverse;
  gap: 1rem; /*oppgis i rem, px, eller lignande.*/
}
```

<article class="oppgave">
    <h4 id="oppgave-6">Oppgave 6</h4>
    <p><em>Bli kjent med Flexbox. Skriv din eigen HTML- og CSS-kode, eller bruk den i eksempelet. </em></p>
    <ul>
      <li>Endre mellomrommet (gap) mellom boksane</li>
      <li>Bruk justify-content på container-elementet til å senterere boksene </li>
      <li>Bruk flex-direction på container-elementet for å endre boksene til å sorteres nedover </li>
      <li>Bruk align-items på container-elementet til å sentrere boksene </li>
    </ul>
</article>


Grunnen til at du må  sentrere to gonger i oppgåva over, er at justify-content og align-items fungerer på kvar sin akse. 
justify-content sentrerer bortover, medan align-items senterere nedover. Leik deg gjerne litt med dei forskjellige verdiane
du kan gi til justify-content og align-items. 


<article class="oppgave">
    <h4 id="oppgave-7">Oppgave 7</h4>
    <p><em>Reverser rekkefølga på child-elementa, slik at det blir Child 3, Child 2, Child 1. </em></p>
    <ul>
      <li>Prøv både for kolonner og rader.</li>
    </ul>
</article>

---

<article class="oppgave">
    <h4 id="oppgave-8">Oppgave 8</h4>
    <p><em> Sentrer teksten inni child-elementa. Hugs at children også kan bli containers. </em></p>
    <ul>
      <li>Sentrer på samme måte som du har gjort for .container-elementet</li>
    </ul>
</article>

---

<article class="oppgave">
    <h4 id="oppgave-9">Oppgave 9</h4>
    <p><em>Lag ei nettside med overskrift, bilder og forskjellige element. Prøv å plasser elementa på forskjellige måtar på sida ved å bruke teknikkane du har lært.  </em></p>
</article>

[Gå til neste del: Avansert HTML](/TENK-tech-camp-web-intro/posts/05_HTML_plus)
