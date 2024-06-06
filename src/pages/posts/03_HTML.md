---
layout: ../../layouts/post.astro
title: "HTML"
description: "HTML"
author: "gurop"
excerpt: HTML
image:
  src:
  alt:
tags: [ "nivå2" ]
---

### Innhald

- [Kva er HTML](#kva-er-html)
- [Elementer](#elementer)
- [Tags](#tags)
- [Oppgave 1](#oppgave-1)
- [Oppgave 2](#oppgave-2)
- [Oppgave 3](#oppgave-3)
- [Oppgave 4](#oppgave-4)

## Kva er HTML?

<font color="#EA580C">HTML</font> er ein måte å strukturere tekst og anna innhald på. Litt som når du skriv ein tekst og
deler den opp med avsnitt for å markere at det er forskjell i innhaldet i teksten, gjer ein det same i HTML. Dette gjer
ein med <font color="#EA580C">tags</font>.

Dette er ein <font color="#EA580C">paragraph</font>-tag. Paragraph betyr avsnitt.

```html
<p>Dette er eit avsnitt</p> 
```

Dette er ein <font color="#EA580C">header</font>-tag. Header betyr overskrift. h1 er veldig stor tekst, mens h2 er litt
mindre,
og h3 blir litt mindre enn det att, og så vidare.

```html
<h1>Dette er ei overskrift</h1>
<h2>Dette er ei underoverskrift</h2> 
```

Grunnen til at ein er nøydd til å strukturere innhaldet på nettsida slik at alt ligg i tags er at nettlesaren din, f.eks
<font color="#EA580C">chrome</font>, <font color="#EA580C">safari</font> eller <font color="#EA580C">firefox</font> skal
kunne skjøne kva sida innehalder og korleis det skal vises.

<article class="oppgave">
    <h4 id="oppgave-1">Oppgave 1</h4>
    <p><em>Lag en enkel side, med de html-elementene over.</em></p>
    <ul>
      <li>Hva skjer når du endrer på måten ting er nøstet på?</li>
      <li>Det er veldig viktig at man er eksakt, og skriver taggene nøyaktig slik de er definert. Husk også å lukke de!</li>
      <li><code class="language-plaintext highlighter-rouge">&lt;div&gt;</code>-taggen er en generisk tag for å samle innhold, og kan være nyttig for å dele opp innholdet på en fornuftig måte.</li>
    </ul>
</article>

---

## Lister

Det fins 142 element ein kan legga til nettsida sin, og nokon har meir avansert funksjonalitet enn å berre endre på
korleis teksten ser ut. Disse elementene består gjerne av flere forskjellige typer elementer, som man bruker samtidig.
Vi kan legge til lister, med en kombinasjon av `<ul>`- og `<li>`-taggene:

```html
<ul>
  <li>Gandalf</li>
  <li>Frodo</li>
  <li>Aragorn</li>
  <li>Gimli</li>
</ul>
```

Vi kan også ha nummererte lister, dersom rekkefølgen er viktig, med `<ol>`- og `<li>`-taggene:

```html
<ol>
  <li>Liverpool</li>
  <li>Manchester City</li>
  <li>Arsenal</li>
  <li>Aston Villa</li>
</ol>
```


---

<article class="oppgave">
    <h4 id="oppgave-2">Oppgave 2</h4>
    <p><em>Lag ei liste med innhald</em></p>
    <ul>
        <li>Klarar du å laga underelementer på elementa i listene? </li>
    </ul>


</article>

---

<article class="oppgave">
    <h4 id="oppgave-3">Oppgave 3</h4>
</article>

---

<article class="oppgave">
    <h4 id="oppgave-4">Oppgave 4</h4>
</article>






[Gå til neste del: CSS](04_CSS)