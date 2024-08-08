---
layout: ../../layouts/post.astro
title: "HTML"
description: "HTML"
author: "gurop"
excerpt: HTML er ein måte å strukturere tekst og anna innhald på, ved å plassere dei ulike elementa på nettsida i ulike boksar.  
image:
  src:
  alt:
tags: [ "nivå2" ]
---

### Innhald

- [Oppgave 1](#oppgave-1)
- [Oppgave 2](#oppgave-2)

## Kva er HTML?

<font color="#EA580C">HTML</font> er ein måte å strukturere tekst og anna innhald på. Litt som når du skriv ein tekst og
deler den opp med avsnitt for å markere at det er forskjell i innhaldet i teksten, gjer ein det same i HTML. Dette gjer
ein med <font color="#EA580C">tags</font>.

### Tekst

Dette er ein <font color="#EA580C">paragraph</font>-tag. Paragraph betyr avsnitt.

Kvar tag må opnast og sluttast. Til dømes, ein paragraph tag `p` blir opna med `<p>`
og blir slutta med `</p>`. Teksten mellom dei to tags er ein del av avsnittet.

```html
<p>Dette er eit avsnitt du kan bruke i oppgave 1</p> 
```

Dette er ein <font color="#EA580C">header</font>-tag. Header betyr overskrift. h1 er veldig stor tekst, mens h2 er litt
mindre,
og h3 blir litt mindre enn det att, og så vidare.

```html
<h1>Dette er ei overskrift du kan bruke i oppgave 1</h1>
<h2>Dette er ei underoverskrift</h2> 
```

Grunnen til at ein er nøydd til å strukturere innhaldet på nettsida slik at alt ligg i tags er at nettlesaren din, f.eks
<font color="#EA580C">chrome</font>, <font color="#EA580C">safari</font> eller <font color="#EA580C">firefox</font> skal
kunne skjøne kva sida innehalder og korleis det skal vises.

<article class="oppgave">
    <h4 id="oppgave-1">Oppgave 1</h4>
    <p><em>Lag en enkel side, med de html-elementene over.</em></p>
    <ul>
      <li>Lim inn overskriftene og avsnittet over</li>
      <li>Hva skjer når du endrer på måten ting er organisert på? (dvs flytte på elementene)</li>
      <li>Det er veldig viktig at man er eksakt, og skriver taggene nøyaktig slik de er definert. Husk også å lukke de!</li>
      <li><code class="language-plaintext highlighter-rouge">&lt;div&gt;</code>-taggen er en generisk tag for å samle innhold, og kan være nyttig for å dele opp innholdet på en fornuftig måte.</li>
    </ul>
    <p><em>Hvis du sliter med kva du skal skrive, kan du for eksempel skrive litt om feriedestinasjoner eller forskjellige dyr.</em></p>
</article>

---

### Lister

Det fins 142 element ein kan legga til nettsida sin, og nokon har meir avansert funksjonalitet enn å berre endre på
korleis teksten ser ut. Disse elementene består gjerne av flere forskjellige typer elementer, som man bruker samtidig.
Vi kan legge til lister, med en kombinasjon av `<ul>`- og `<li>`-taggene:

```html
<ul>
  <li>Hund</li>
  <li>Sjøsnegle</li>
  <li>Sommerfugl</li>
  <li>Neshorn</li>
</ul>
```

Vi kan også ha nummererte lister, dersom rekkefølgen er viktig, med `<ol>`- og `<li>`-taggene:

```html
<ol>
  <li>Bergen</li>
  <li>Gran Canaria</li>
  <li>Lofoten</li>
  <li>London</li>
</ol>
```

---

### Bilder

Et annet element som er veldig avhengig av attributter, er `<img>`-taggen, som lar oss legge til bilder på nettsiden.

Denne taggen har en `src`-attributt, hvor vi legger stien / adressen til bildet.

```html
<div>
  Et tilfeldig bilde
  <br />
  <img src="https://picsum.photos/200" />
</div>
```

Merk at det er ikke alltid man får lov til å vise slike bilder direkte fra en annen side, da de som eier den andre nettsiden
har mulighet for å stenge for dette.
Det går an å vise til et bilde som ligger sammen med HTML-filen:

```html
<div>
  Et utvalgt bilde
  <br />
  <img src="bildet-mitt.jpg" />
</div>
```

Dette forutsetter at i samme mappe (lokalt på din maskin), så ligger det en bilde-fil (.jpg, .png, etc) ved siden av HTML-filen.

---

<article class="oppgave">
    <h4 id="oppgave-2">Oppgave 2</h4>
    <p><em>Legg til et bilde på nettsiden din</em></p>
    <ul>
      <li>Du kan finne et bilde på nett, og enten legge til adressen direkte til bildet - men det er ikke alltid man får lov</li>
      <li>Kan også laste ned et bilde lokalt, og vise til stien direkte (men forutsetter at man ikke bruker CodePen)</li>
      <li>Det finnes noen sider som lar deg hente slikte bilder gratis: <a href="https://picsum.photos">https://picsum.photos</a>, <a href="https://placekitten.com/">https://placekitten.com/</a></li>
    </ul>
</article>

---

### Oppsummering 

- HTML-sider har en struktur, som består av tagger og tekst
- Disse taggene angir hvilket type innhold og hvilken struktur siden skal ha
- Det finnes et mangfold av ulike typer elementer

### Videre

Det finnes veldig mye mer man kan gjøre i ren HTML, og veldig mange andre elementer og attributter vi ikke har snakket om.

Her er liste over alle de forskjellige elementene som er definert i HTML-standarden:
[HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

Det finnes veldig mye der ute som man kan utforske, og en moderne nettside kan være veldig avansert!

Tykkjer du det er vanskeleg å hugsa dei riktige tags? Dei fleste taggar har eit logisk namn.
Til dømes står `ul` for uordna liste, medan `ol` er ein ordna (nummerert) liste.
Kvart element i lista er eit listeelement (list item; `li`).


[Gå til neste del: CSS](/TENK-tech-camp-web-intro/posts/04_CSS)