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
- [Oppgave 3](#oppgave-3)
- [Oppgave 4](#oppgave-4)
- [Oppgave 5](#oppgave-5)
- [Oppgave 6](#oppgave-6)


## Kva er HTML?

<font color="#EA580C">HTML</font> er ein måte å strukturere tekst og anna innhald på. Litt som når du skriv ein tekst og
deler den opp med avsnitt for å markere at det er forskjell i innhaldet i teksten, gjer ein det same i HTML. Dette gjer
ein med <font color="#EA580C">tags</font>.

### Tekst

Dette er ein <font color="#EA580C">paragraph</font>-tag. Paragraph betyr avsnitt.

Kvar tag må opnast og sluttast. Til dømes, ein paragraph tag `p` blir opna med `<p>`
og blir slutta med `</p>`. Teksten mellom dei to tags er ein del av avsnittet.

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

### Tabeller

Tabeller er ofte nyttige for å "strukturere" og presentere innholdet, spesielt om man har data som kan representeres med rader og kolonner.

De er litt mer finurlige, men defineres slik:

```html
<!-- table-taggen definerer at her starter tabellen vår -->
<table>
  <!-- thead-taggen forteller oss at dette skal være headeren på tabellen -->
  <thead>
    <!-- tr-taggen forteller at dette skal være en rad i tabellen -->
    <tr>
      <!-- th-taggen representerer en kolonne i tabellen -->
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>

  <!-- tbody-taggen forteller oss at dette skal være selve innholdet i tabellen -->
  <tbody>
    <!-- første rad -->
    <tr>
      <!-- td-taggen representerer en enkel celle i tabellen -->
      <!-- merk at det bør være like mange td-elementer som vi hadde th-tagger i headeren -->
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <!-- andre rad -->
    <tr>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <!-- osv osv -->
  </tbody>
</table>
```

Et eksempel med litt innhold:

```html
<table border="1">
  <thead>
    <tr>
      <th>Navn</th>
      <th>Latinsk navn</th>
      <th>Vekt (g)</th>
      <th>Kroppstemperatur (°C)</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>Hund</td>
      <td>Canis</td>
      <td>1.500-100.000</td>
      <td>39</td>
    </tr>
    <tr>
      <td>Sommerfugl</td>
      <td>Rhopalocera</td>
      <td>0,04-0,3</td>
      <td>20-50</td>
    </tr>
  </tbody>
</table>
```

Dette blir fort veldig avansert, så det er viktig at man bruker indentering, for å gjøre det så lett-leselig som mulig.

Merk denne `border="1"`-greia vi la til - dette er en attributt, som vi skal snakke litt nærmere om seinere i workshopen,
vi legger den til her for å gjøre tabellen vår litt mer synlig.

---

<article class="oppgave">
    <h4 id="oppgave-2">Oppgave 2</h4>
    <p><em>Legg til en enkel tabell på nettsiden din</em></p>
    <ul>
      <li>Vær obs på strukturen! Det er et samspill mellom <code class="language-plaintext highlighter-rouge">&lt;table&gt;</code>, <code class="language-plaintext highlighter-rouge">&lt;thead&gt;</code>, <code class="language-plaintext highlighter-rouge">&lt;tbody&gt;</code>, <code class="language-plaintext highlighter-rouge">&lt;tr&gt;</code>, <code class="language-plaintext highlighter-rouge">&lt;th&gt;</code>, og <code class="language-plaintext highlighter-rouge">&lt;td&gt;</code> - så det kan lett gå i surr, og det er viktig at man lukker de riktig.</li>
    </ul>
</article>

---

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
    <h4 id="oppgave-3">Oppgave 3</h4>
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
    <h4 id="oppgave-4">Oppgave 4</h4>
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
    <h4 id="oppgave-5">Oppgave 5</h4>
    <p><em>Legg til noen lenker til forskjellige nettsider inne på siden din</em></p>
    <ul>
      <li>Merk at på CodePen får man ofte ikke åpne disse sidene, med mindre man åpner de i en ny fane</li>
    </ul>
</article>

---

<br/>

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
    <h4 id="oppgave-6">Oppgave 6</h4>
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
- Man kan bruke attributter på elementene for å gi de litt mer avansert funksjonalitet

### Videre

Det finnes veldig mye mer man kan gjøre i ren HTML, og veldig mange andre elementer og attributter vi ikke har snakket om.

Her er liste over alle de forskjellige elementene som er definert i HTML-standarden:
[HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

Det finnes veldig mye der ute som man kan utforske, og en moderne nettside kan være veldig avansert!

Tykkjer du det er vanskeleg å hugsa dei riktige tags? Dei fleste taggar har eit logisk namn.
Til dømes står `ul` for uordna liste, medan `ol` er ein ordna (nummerert) liste.
Kvart element i lista er eit listeelement (list item; `li`).


[Gå til neste del: CSS](/TENK-tech-camp-web-intro/posts/04_CSS)