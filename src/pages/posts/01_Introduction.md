---
layout: ../../layouts/post.astro
title: "Introduksjon"
description: "Introduksjon"
author: "gurop"
excerpt: Hva er egentlig en nettside, og hvordan lager man en?  
image:
  src:
  alt:
tags: ["nivå1"]
---


Så, kva er eigentleg ei nettside?

Ei nettside er alt frå <font color="#EA580C">It's learning</font> der du sjekker lekser, til om du opnar
<font color="#EA580C">TikTok</font> i nettlesaren eller handlar ei ny t-skjorte i nettbutikken til <font color="#EA580C">HM</font>.

Det finst utruleg mange måtar å lage nettsider på, med mange program som gjer det enklare for utviklarane å bygge dei.

Men, i botnen er alle nettsider ei samling med HTML, og gjerne CSS og javascript-filer.

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

```html
<p class="fet-skrift" id="first-paragraph">Dette er eit avsnitt</p>
```


<p class="codepen" data-height="300" data-default-tab="html" data-slug-hash="OJYgJGM" data-pen-title="HTMLCSS" data-user="gurop" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/gurop/pen/OJYgJGM">
  HTMLCSS</a> by AnoymousCat (<a href="https://codepen.io/gurop">@gurop</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

## Kva er JavaScript?

Javascript er det som får nettsida til å oppføre seg på ein spesiell måte. Når du trykker på ein knapp, er det javascript
som bestemmer kva som skal skje. 

Om du for ekesmpel har fylt ut eit skjema, for å opprette ein konto på ei nettside, og trykker "send inn", kan utviklaren,
ved hjelp av javascript, samle inn all dataen du har skrive, sjekke at den ser rett ut (at e-post adresser har ein @ i seg,
at telefonnummer kun er tall), og sende den til backenden slik at dataen kan lagrast og brukaren din vert oppretta. 

Me går nærmare inn på javascript seinare. 

[Gå til neste del: Setup](02_Setup)