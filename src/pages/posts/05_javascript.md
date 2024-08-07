---
layout: ../../layouts/post.astro
title: "JavaScript"
description: "JavaScript"
author: "gurop"
excerpt: JavaScript 
image:
  src:
  alt:
tags: ["nivå4"]
---


### Innhald

- [Oppgave 1](#oppgave-1)
- [Oppgave 2](#oppgave-2)
- [Oppgave 3](#oppgave-3)
- [Oppgave 4](#oppgave-4)
- [Oppgave 5](#oppgave-5)
- [Oppgave 6](#oppgave-6)
- [Oppgave 7](#oppgave-7)
- [Oppgave 8](#oppgave-8)
- [Oppgave 9](#oppgave-9)
- [Oppgave 10](#oppgave-10)
- [Oppgave 11](#oppgave-11)
- [Oppgave 12](#oppgave-12)

## Kva er JavaScript?

Javascript er det som får nettsida til å oppføre seg på ein spesiell måte. Når du trykker på ein knapp, er det JavaScript
som bestemmer kva som skal skje.

Ta eksempelet for eksempel at du har fylt ut eit skjema for å opprette ein konto på ei nettside. Når du trykker "send inn", kan utviklaren
ved hjelp av javascript samle inn all dataen du har skrive. Utviklaren kan òg sjekke at teksten er rett (at e-post adresser har ein @ i seg,
at telefonnummer kun er tall), og deretter sende den til databasen slik at dataen kan lagrast og brukaren din vert oppretta.

### Del 1 - Javascript grunnleggende konsepter

#### Variabler
Variabler er som bokser der vi kan lagre informasjon vi ønsker å bruke senere. Tenk på dem som navngitte beholdere som kan inneholde tall, tekst eller andre typer data.

```js
// tekststrenger
var rund_ting_1 = "klokke"
var rund_ting_2 = "cd"

// tall
var radius = 5
var pi = 3.1415

// utrykk
var omkrets = 2 * pi * radius

// oppdatere variabler
var antall_runde_ting = 2
antall_runde_ting = antall_runde_ting * 3

// boolske verdier true/false
var har_kanter  = false
```

#### if så else, og boolske verdier

Boolske verdier er enkle data som bare kan være enten true (sann) eller false (usann).
If-else-setninger lar oss ta beslutninger i koden vår. De sjekker om en betingelse (en påstand) er sann eller usann, og utfører handlinger basert på dette.

```js
var klokkeslett = 15

if (klokkeslett < 18){
  console.log("God dag")
} else {
  console.log("God kveld")
}


// om det første utrykket er sant vil den printe God morgen.
// om klokkeslettet er ikke er mindre enn 10 går den til neste steg
// da sjekker den om klokkeslettet er mindre enn 18, om det er sant
// så printer den God dag
// men om det ikke er sant, går den ned til else og printer God Kveld
if (klokkeslett < 10){
  console.log("God morgen")
} else if (klokkeslett < 18) {
  console.log("God dag")
} else {
  console.log("God kveld")
}
```

#### Funksjoner

Funksjoner er som oppskrifter. De forteller datamaskinen hva den skal gjøre, steg for steg. Vi kan lage en funksjon for å utføre en bestemt oppgave, og deretter bruke den hvor som helst i koden vår.

```js
function omkrets(radius) {
  var pi = 3.1415
  return pi * radius * 2
}

omkrets(5)
```

---

<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="mdZPyvq" data-pen-title="Temperatur kalkulator" data-editable="true" data-user="Elinborg" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/Elinborg/pen/mdZPyvq">
  Temperatur kalkulator</a> by Karina Elinborg (<a href="https://codepen.io/Elinborg">@Elinborg</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

---

<article class="oppgave">
    <h4 id="oppgave-1">Oppgave 1</h4>
    <p><em>Sette variabler og printe dem i konsollen</em></p>
    <ul>
      <li>Vi skal starte med å finne konsollen, den kan du åpne med å trykke på `Console` knappen nede i venstre hjørne i CodePen</li>
      <li>I JS vinduet skal vi sette noen variabler: <em>navn</em> og <em>alder</em></li>
      <li>Navn kan være en tekst tekststreng: "Harald"</li>
      <li>Alder kan være et tall: 87</li>
      <li>For å se hvilken verdi som ligger i en variabel kan vi bruke console.log(navn) eller console.log(alder)</li>
      <li>Test hva som skjer om du gir samme variabel to forskjellige verdier</li>
      <li>Du kan også oppdatere en variabel, etter å ha definert alder, prøv feks <em>alder = alder-5</em></li>
    </ul>
</article>

---

<article class="oppgave">
    <h4 id="oppgave-2">Oppgave 2</h4>
    <p><em>Lag to funksjon som printer noe i konsollen</em></p>
    <ul>
      <li>For å definere en funksjon skriver man <em>function funksjonsNavn(parameter1, parameter2)</em>, en funksjon trenger ikke å ha parameter da har man bare en tom ()</li>
      <li>Du kaller på funksjonen med å skrive <em>funksjonsNavn(argument1, argument2)</em></li>
      <li>Parameter beskriver hva funksjonen skal ta inn, mens argument er den faktiske dataen vi sender inn til funksjonen</li>
      <li>Lag en funksjon hello(), som printer feks <em>Hello World!</em> til konsollen</li>
      <li>Lag en annen funksjon som tar inn navn og alder som argumenter, og bruk disse i <em>console.log()</em> meldingen</li>
      <li>Feks. <em>console.log("Hei, " + navn)</em></li>
    </ul>
</article>

---

<article class="oppgave">
    <h4 id="oppgave-3">Oppgave 3</h4>
    <p><em>Logikksjekk inne i funksjonen med parameter</em></p>
    <ul>
      <li>Lag en if else som sjekker om personen er over 18 år.</li>
      <li>Vis to forskjellige meldinger basert på om personen er gammel nok eller ikke</li>
    </ul>
</article>

 ---

### Del 2 - Temperatur kalkulator

Her skal vi lage en enkel applikasjon for å konvertere mellom fahrenheit og celsius.
Her bruker vi de  grunnleggende JavaScript konseptene som if og else, og definerer variabler, samt å lage en funksjon og gi den argumenter som vi utforsket i oppgave 1-3.
Nye ting som vi skal se på her er hvordan man kan bestemme hva som skjer når man trykker på en knapp.
Hvordan lese hvilken verdi som er lagret i et input-felt.
Og oppdatere innholdet i et html element.

Her er planen for hvordan vi skal bygge opp kalkulatoren vår, vi skal gå igjennom det steg for steg i oppgavene under
Her bruker man evenListener for å følge med på  om en knapp blir trykket på.
Så bruker vi id en et element for å hente verdien som en lagret i et tekst feltet
Så brukes en funksjon vi har lagd til å regner ut den nye fahrenheit/celsius verdien
Tilslutt henter vi ut et output element, hvor vi legger til resultatstrenger vår og oppdatere den slik at resultatet dukker opp på siden

---

La oss sette i gang.

Vi ønsker først at noe skal skje når vi trykker på knappene. Her skal vi bruke funksjonen konverter_temperatur. For å sjekke at funksjonen blir brukt kan du console.log noe inne i funksjonen.

<article class="oppgave">
    <h4 id="oppgave-4">Oppgave 4</h4>
    <p><em>Regisetre knappetrykk</em></p>
    <ul>
      <li>Her skal vi bruke <em>addEventListener()</em> på knapp-elementene, for å registrere når man trykker på knappene.</li>
      <li>Først må vi finne knapp-elementene. Vi viser et eksempel for celsius til fahrenheit knappen.</li>
      <li>var cToFElement = document.getElementById("ctof")</li>
      <li>Neste steget er å registrere en event listener, som aktiverer en funksjon på click eventen.</li>
      <li>cToFElement.addEventListener("click", konverter_temperatur())</li>
      <li>Sjekk at trykket blir registrert og aktiverer funksjonen.</li>
      <li>Gjør det samme for knappen som konverterer fra fahrenheit til celsius.</li>
    </ul>
</article>

---


Vi har to knapper og vi ønsker at de skal ha forskjellig oppførsel.
La oss oppdatere funksjonen slik at den har et parameter: enhet.
I hver av knappene legg til argumentet "C" om verdien vi tar i mot er celsius og F om verdien vi tar inn er Farenheit.
Siden funksjonen nå tar inn et parameter må vi endre litt på <em>addEventListener(function(){myFunction(parameter1, parameter2)})</em>

<article class="oppgave">
    <h4 id="oppgave-5">Oppgave 5</h4>
    <p><em>Oppdater funksjon til å ta inn argument, oppdater eventListener</em></p>
    <ul>
      <li>La funksjonen ha et parameter som er enhet</li>
      <li>Vi må også oppdatere addEventListener() som vi har på knappene</li>
      <li>addEventListener(function(){myFunction(parameter1)})</li>
      <li>Legg til argumentet "C" og "F"</li>
      <li>Oppdater console.log / alert meldingen og sjekk at knappene har forskjellig oppførsel med å også printe hva de får som argument.</li>
    </ul>
</article>

 ---

I html vinduet er det et inputfelt, dette har id="input-field", vi har lyst til å hente verdien som er lagret i dette inputfeltet.
Vi kan starte med å prøve ting ut i konsollen.
Med å bruke document.getElementById('input-field') henter vi ut et html element med denne iden.
Siden vi ønsker å finne verdien lagret i dette elementet kan vi bruke .value
Dette gir oss document.getElementById('input-field').value

<article class="oppgave">
    <h4 id="oppgave-6">Oppgave 6</h4>
    <p><em>Bruk konsollen til å se hvilken verdi som er lagret i input feltet</em></p>
    <ul>
      <li>Skriv document.getElementById('input-field'), bytt ut "input-field" er id'en på inputfeltet</li>
      <li>Prøv å ha forskjellige verdier i inputfeltet, hva skjer om feltet er tomt, om det har tekst, tall eller desimaltall i seg</li>
    </ul>
</article>

 ---



Neste steg er å hente ut denne informasjonen i scriptet vårt.
Inne i funksjonen bruk variabelen input_verdi til å lagre denne verdien
Om du ønsker å se at riktig verdi ble lagret når vi kjører funksjonen kan du console logge variabelen.

<article class="oppgave">
    <h4 id="oppgave-7">Oppgave 7</h4>
    <p><em>Oppdater funksjonen til å hente input felt verdien</em></p>
    <ul>
      <li>Bruk input_verdi variabelen til å lagre verdien som vi henter fra inputfeltet</li>
      <li>Sjekk med console.log at vi får tak i verdien når vi kaller på funksjonen med å trykke på en av knappene</li>
    </ul>
</article>

 ---

Nå har vi all informasjonen vi trenger. Vi vet om vi skal gjøre om til celsius eller farenheit, og vi vet input verdien vår. Det eneste vi trenger å gjøre nå er å regne ut den riktige konverteringen.

<article class="oppgave">
    <h4 id="oppgave-8">Oppgave 8</h4>
    <p><em>La funksjonen sjekke hvilken knapp vi trykket på / gjør 2 forskjellige ting basert på hva argument funksjonen får</em></p>
    <ul>
      <li>Bruk en if/else for å sjekke om argumentet vi fikk til funksjonen er C eller F</li>
      <li>Brukt input verdien til å regne ut en result verdi som vi lagrer i variabelen <em>resultat</em></li>
      <li>for formatering av resultat meldingen vil vi vite den motsatte enhets-verdien fra argumentet vi fikk. Så om enhet='C' skal motsatt='F'</li>
      <li>Lagre denne verdien i en variabel, motsatt</li>
    </ul>
</article>


For å regne ut fra celsius til farenheit er funksjonen:
`1.8 * C + 32` hvor `C` er temperaturen i celsius
om man skal fra farenheit blir formelen
`(F -32) / 1.8`

 ---

Nå har vi hva original temperaturen vår var <em>input_verdi</em>, og hvilken enhet den hadde <em>enhet</em>, vi har også funnet den konverterte temperaturen <em>resultat</em> og den motsatte enheten <em>motsatt</em>.
Vi kan nå lage en tekststreng som vi skal la være vår <em>output_verdi</em>

<article class="oppgave">
    <h4 id="oppgave-9">Oppgave 9</h4>
    <p><em>Formater resultatet i en resultat streng og lagre denne verdien i en variabel</em></p>
    <ul>
      <li>output_verdi = input_verdi + " \u00b0" + enhet + " er det samme som " + resultat + " \u00b0" + motsatt</li>
      <li>\u00b0 er ascii koden for grad symbolet, man kan også kopiere denne verdien °</li>
      <li>Print output_verdi i konsollen med console.log() for å sjekket at det ser riktig ut</li>
    </ul>
</article>

---


Nå har vi lyst til å legge til denne output-verdien inn i htmlen slik at den dukker opp på siden.
I htmlen kan man se at vi har et element som heter output, dette er hva vi skal bruke

Her skal vi bruke `querySelector` som er en annen måte å hente ut et html element. Den er litt mer generell enn `getElementById`. Denne kan vi spørre etter type html element og den gir oss den første instansen av dette elementet. Man kan også hente ut elementer basert på andre kriterier men her bruker vi element type, som er output

`document.querySelector('output').innerHTML = output_verdi`

Her kan vi også bruk andre elementer som kan holde på text som en div, og enten hente den slik som vi gjorde med input felted og getElementById eller querySelector etter div eller klasse.

<article class="oppgave">
    <h4 id="oppgave-10">Oppgave 10</h4>
    <p><em>Adder resultatet til HTML output elementet</em></p>
    <ul>
      <li>I slutten av funksjonen så legger du en linje for å addere resultat strenger til HTML elementet output</li>
      <li>document.querySelector('output').innerHTML = output_verdi</li>
    </ul>
</article>

 ---

Nå som alle disse tingene er satt opp har man en fungerende kalkulator

... eller er den helt uten feil??

---
<article class="oppgave">
    <h4 id="oppgave-11">Oppgave 11</h4>
    <p><em>Test at ting fungerer som den skal</em></p>
    <ul>
      <li>Test hva som skjer om man gir tekst som input og ikke et tall</li>
      <li>Test hva som skjer om input feltet er tomt</li>
      <li>Test hva som skjer om du prøver å konverter 100F til C</li>
    </ul>
</article>

 ---


---
<article class="oppgave">
    <h4 id="oppgave-12">Oppgave 12</h4>
    <p><em>La oss fikse litt bugs: Input check</em></p>
    <ul>
      <li>De to første tingene vi testet over faller under samme kategori.</li>
      <li>Vi kan endre input elementet til i forvente "number" med å erstatte "string" til number</li>
      <li>Test hva som skjer om man nå gir ikke tall til input feltet da får vi en tom streng</li>
      <li>Nå trenger vi bare å håndtere en tom streng</li>
      <li>En tom streng har egenskapen at den er boolske verdien false</li>
      <li>Vi kan dermed sjekke om input_verdi er true eller false</li>
      <li>Om den er false kan vi droppe å regne ut noe, og bare oppdatere output elementer vårt med en feilmelding</li>
    </ul>
</article>

 ---
<article class="oppgave">
    <h4 id="oppgave-13">Oppgave 13</h4>
    <p><em>La oss fikse litt bugs: Desimaltall formatering</em></p>
    <ul>
      <li>Man kan bruke funksjonen toFixed(n) til å bestemme at et tall bare skal ha max n desimaler</li>
      <li>Etter vi har regnet ut den nye temperaturen, endre variabelen slik at den bare har 2 desimaler</li>
    </ul>
</article>

 ---


### Del 3 - Todo list

Her har vi en litt mer avansert applikasjon enn den over. I tillegg til alle de nye konseptene vi lærte over brukes det her også hvordan å lage ny html elementer og legge de til med javascript.
Her er det også noen nye konsepter som lister og for-løkker.


<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="VwJYVbK" data-pen-title="To Do List" data-editable="true" data-user="Elinborg" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/Elinborg/pen/VwJYVbK">
  To Do List</a> by Karina Elinborg (<a href="https://codepen.io/Elinborg">@Elinborg</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

[Gå til neste del: Deploy](/TENK-tech-camp-web-intro/posts/06_deploy)