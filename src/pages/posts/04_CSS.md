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

Man kan sette styling på tags, slik som over, men og på klasser og id-er man har gitt til tags.

#### Klasser
Klasser settes på html-tags ved å skrive ```class="et-superbra-klassenavn"``` som vist over. Her kan du f.eks lagre styling som 
du har lyst til å bruke på fleire elementer. Du skriver css som treffer klasser-er med ``.``, f.eks ``.et-superbra-klassenavn``. 
```html
<p class="et-superbra-klassenavn">Dette er eit avsnitt</p>
```
```css
.et-superbra-klassenavn {
    color: orange
}
```

#### ID-er
Id-er settes på html-tags ved å skrive ``id="et-superbra-id-navn"``. Ein ID høyrer kun til **eitt** element, og kan brukes til 
å style det spesifikke elementet. Du skriver css som treffer Id-er med ``#``, f.eks ``#et-superbra-id-navn``.
```html
<p id="et-superbra-id-navn">Dette er eit avsnitt</p>
```
```css
.et-superbra-id-navn {
   font-weight: bold 
}
```

NB! navn på klasser og Id-er kan ikkje ha mellomrom i seg. bruk ``-`` i staden for. 


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



[Gå til neste del: javaScript](05_javascript)