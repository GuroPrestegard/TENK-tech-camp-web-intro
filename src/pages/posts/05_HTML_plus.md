---
layout: ../../layouts/post.astro
title: "Avansert HTML"
description: "Avansert HTML"
author: "gurop"
excerpt: Her jobber vi med mer avanserte HTML elementer som forbereder oss til JavaScript oppgavene.  
image:
  src:
  alt:
tags: [ "nivå2" ]
---

### Innhald

- [Oppgave 1](#oppgave-1)
- [Oppgave 2](#oppgave-2)
- [Oppgave 3](#oppgave-3)

## Avansert HTML

I JavaScript delen, bygger vi et verktøy som konverterer temperaturer fra celsius
til fahrenheit og motsatt vei. Vi bruker input og knapp elementene i den oppgaven.
Derfor utforsker vi dem her før vi setter i gang med konverteringsverktøyet.

### Input

Nettsider lar oss gjerne gjøre litt mer enn å bare se på innhold, for eksempel kan man legge til en kommentar, eller logge inn.
Da finnes det litt mer avanserte elementer vi kan benytte for å la brukeren gjøre slike handlinger.

Litt senere, når vi kommer til JavaScript-delen, skal vi se på hvordan vi kan bruke disse elementene til å gi oppførsel til siden vår.

Ofte ønsker man at de som bruker nettsiden skal kunne legge inn noe tekst, for eksempel om de skal logge inn med brukernavn og passord,
eller legge til en kommentar.

`<input>`-elementet gir oss en enkel tekstboks som brukeren kan skrive i.
Merk at dette også er et sånt spesielt element, som opnast og lukkast i samme tag.

```html
<div>
  Brukernavn:
  <input />
  Passord:
  <input />
</div>
```

Dersom man ønsker at bruker skal kunne skrive litt lengre tekster med linjeskift, for eksempel en kommentar på en post, kan man
bruke `<textarea>`-elementet:

```html
<div>
  Kommentar:
  <textarea> </textarea>
  <!-- merk at denne må man lukke -->
</div>
```

Vi kan bruke `<button>`-elementet for å lage knapper på nettsiden vår:

```html
<div>
  Kommentar:
  <textarea> </textarea>
  <button>Legg til kommentar</button>
</div>
```

---

<article class="oppgave">
    <h4 id="oppgave-1">Oppgave 1</h4>
    <p><em>Legg til noen tekstfelt og knapper til nettsiden din</em></p>
    <ul>
      <li>Vi kommer seinere til å gå inn på hvordan vi kan få disse til å både se litt bedre ut, og ha faktisk oppførsel, i CSS- og JavaScript-delene</li>
    </ul>
</article>

---

### Attributter

Et veldig viktig konsept som vi må være innom, og som blir veldig relevant for CSS- og JavaScript-delene,
er dette med attributter på HTML-elementene våre.

Attributter er ekstra konfigurering og informasjon vi kan gi til elementene våre, for å spisse de litt mer.

Dette er noe man legger til inne i selve taggen, og er separat fra innholdet:

```html
<div id="div-1-id">Innhold</div>
```

Merk at man ikke trenger å legge de til i lukke-taggen, og det er viktig at man starter og slutter attributten med `"`.

`<input>`-elementet er et eksempel på en tag som kan endres ganske mye basert på hvilke attributter vi gir den.

Vi kan bruke `type="checkbox"` for å lage en checkbox der man kan velge ja / nei:

```html
<div>
  <h3>velg det viktigste for feriedestinasjonen din:</h3>
  <input type="checkbox" /> Strand <br />
  <input type="checkbox" /> Snø <br /> 
  <input type="checkbox" /> Luksus hotel <br />
  <input type="checkbox" /> Billig mat <br />
  <input type="checkbox" /> Barnevennlig <br />
</div>
```

Vi kan bruke `type="number"` for å gjøre det om til et tekstfelt man bare kan legge til tall i:

```html
<div>
  <label>Maks antall timer fra Bergen:</label> <br />
  <input type="number" />
</div>
```

Som default får `<input>`-elementet verdien `type="text"`, men man kan ha flere attributter samtidig,
for eksempel om vi ønsker å begrense hvor mange tegn brukeren skal kunne skrive inn, og også ha en placeholder tekst:

```html
<div>
  <label>Brukernavn:</label> <br />
  <input type="text" maxlength="20" placeholder="Angi brukernavn..." />

  <br />
  <!-- merk at det er lov ha attributter over flere linjer, som kan gjøre det lettere å lese: -->
  <label>Passord:</label> <br />
  <input
    type="password"
    minlength="8"
    maxlength="50"
    placeholder="Angi passord..."
  />
</div>
```

---

<article class="oppgave">
    <h4 id="oppgave-2">Oppgave 2</h4>
    <p><em>Bruk attributter for å legge til noen mer avanserte <code class="language-plaintext highlighter-rouge">&lt;input&gt;</code>-elementer på nettsiden din</em></p>
    <ul>
      <li>Det finnes mange gyldige <code class="language-plaintext highlighter-rouge">type</code>-attributter for <code class="language-plaintext highlighter-rouge">&lt;input&gt;</code> som f.eks <code class="language-plaintext highlighter-rouge">color</code>, <code class="language-plaintext highlighter-rouge">date</code>, <code class="language-plaintext highlighter-rouge">search</code>, <code class="language-plaintext highlighter-rouge">radio</code>, <code class="language-plaintext highlighter-rouge">file</code> - Eksperimenter gjerne med disse, og legg merke til hvor mye form og funksjon blir påvirket av å endre dette attributtet</li>
    </ul>
</article>

---

<br/>

Attributter er svært viktige for lenker, for eksempel, da det er der vi angir hvilken adresse lenken skal peke på.
Lenker defineres med `<a>`-taggen i HTML, og må ta en `href`-attributt.

```html
<div>
  <a href="https://www.nrk.no/">NRK.no</a>
  <br />
  <!-- Denne magiske target-attributten vil automatisk åpne lenken i en ny fane i nettleseren -->
  <a href="https://www.google.com/" target="_blank">Google</a>
</div>
```

Nettsider består gjerne også av mange forskjellige lenker, som peker på forskjellige sider inne på den samme nettsiden,
eller til sider som finnes på helt andre adresser, andre steder på nett.
I denne workshopen skal vi bare fokusere på én enkel nettside, uten lenker til andre sider av samme nettside.

---

<article class="oppgave">
    <h4 id="oppgave-3">Oppgave 3</h4>
    <p><em>Legg til noen lenker til forskjellige nettsider inne på siden din</em></p>
    <ul>
      <li>Merk at på CodePen får man ofte ikke åpne disse sidene, med mindre man åpner de i en ny fane</li>
    </ul>
</article>

[Gå til neste del: JavaScript](/TENK-tech-camp-web-intro/posts/06_javascript)
