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

## Kva er JavaScript?

Javascript er det som får nettsida til å oppføre seg på ein spesiell måte. Når du trykker på ein knapp, er det javascript
som bestemmer kva som skal skje.

Om du for ekesmpel har fylt ut eit skjema, for å opprette ein konto på ei nettside, og trykker "send inn", kan utviklaren,
ved hjelp av javascript, samle inn all dataen du har skrive, sjekke at den ser rett ut (at e-post adresser har ein @ i seg,
at telefonnummer kun er tall), og sende den til backenden slik at dataen kan lagrast og brukaren din vert oppretta.

Me går nærmare inn på javascript seinare. 




### Del 1 - Javascript grunnlegende konspemter
Her skal jeg forkalere
- variabler
Erklære en variabel, endre en variabel, bruke en variabel

- if og else
- boolean
- lister
- for
og sånne ting


---

<article class="oppgave">
    <h4 id="oppgave-1">Oppgave 1</h4>
    <p><em>Erklær to variabler en for navn og en for alder</em></p>
    <ul>
      <li>Navn kan være en tekst tekststreng: "Harald"</li>
      <li>Alder kan være et tall: 87</li>
      <li>Test hva som skjer om du gir samme variabel to forskjellige verdier</li>
    </ul>
</article>

---

<article class="oppgave">
    <h4 id="oppgave-2">Oppgave 2</h4>
    <p><em>Bruk console.log() for å printe verdier i 'Console'</em></p>
    <ul>
      <li>For å vise 'Console' trykk på `Console` knappen nede i venstre hjørne på codePen </li>
      <li>Du kan printe en vilkårlig tekststreng som "Hello World!"</li>
      <li>En kan også bruke variablene vi har definert over</li>
      <li>"Mitt navn er " + navn</li>
      <li>Test hva som skjer om du gir samme variabel to forskjellige verdier</li>
      <li>Du kan også oppdatere en variabel, etter å ha definert alder, prøv feks alder = alder-5</li>
    </ul>
</article>

---

<article class="oppgave">
    <h4 id="oppgave-3">Oppgave 3</h4>
    <p><em>Lag en funksjon som tar inn navn og alder som paramter. Inne i funksjonen kan du ha en if else som sjekker om personen er over X år. Vis to forskjellige meldiger basert på om personen er gammel nok eller ikke</em></p>
    <ul>
      <li>For å definere en funsjon skriver man `function fuknsjonsNavn(paramter1, parameter2)`</li>
      <li>Man kan så kalle på funskjonen med å skrive funksjonsNavn(argument1, arguemnt2)
      <li>Parameter beskriver hva funskjonen skal ta inn, mens argument er den faktiske dataen vi sender inn til funksjonen</li>
    </ul>
</article>

 ---

### Del 2 - Temperatur kalkulator

Her er en enkel aplikasjon for å kovertere mellom farenheit og celscius.
Her bruker vi java script de grunnleggende koseptene som if og else, og de å definere variabler og bruke de, samt å lage en funksjon og gi den argumenter.
Nye ting som vi skal se på her er hvordan man kan bestemme hva som skjer når man trykker på en knapp.
Hvordan lese hvilken verdi som er lagret i et inputfelt.
Og legge oppdatere innholdet i et html element.

Her bruker man evenListerner for å følge med på  om en knapp blir trykket på.
Så bruker vi id en et element for å hente verdien som en lagret i et tekst felt
Så brukes en funksjon vi har lagd til å regner ut den nye farenheit/celsuius verdien
Tilslutt henter vi ut et output element, hvor vi legger til resulttatstrenger vår og oppdateren den slik at resultatet dukker opp på siden


La oss sette i gang.

Vi ønsker først at noe skal skje når vi trykker på knappene.
Start med å lage en funksjon som skal bli kalt på når vi trykker på knappen. For nå så kan alt denne funksjonen gjør er å enten consol.logge eller lage en alert på at knappen ble trykket på.

Dette er jo to forskjellige knapper så vi ønsker at de skal ha forskjellig oppførsel.
La oss oppdatere funksjonene slik at de har et paramtert sdom er enhet. I hver av knappene legg til argumentet "C" om vi skal gjøre om til celsceisu og F om vi skal gjøre om til Farenheit.

Oppdater consol.log / alert meldingen og sjekk at knappenen har forskjellig oppførsel med å også printe hva de får som argument.


Fra koden som er utgitt så er det et input felt, dette har id="input-field", vi har lyst til å hente verdien som er lagret i dette inputfeltet.
Vi kan starte med å prøve ting ut i konsollen.
Med å bruke document.getElementById('input-field') så henter vi ut et html element med denne id om det finnes.
Siden vi ønsker å finne verdien lagret i dette elementet kan vi bruke .value funksjonen.
Dette gir oss document.getElementById('input-field').value

Neste steg er å hente ut denne informasjonen i scriptet vårt.
Inne i funksjonen lag en variabel hvor vi lagrer denne input verdien
Om du ønsker å se at riktig verdi ble lagret når vi kjører funksjonen kan du console logge variabelen.

Nå har vi vet vi om vi skal gjøre om til cesceius eller farenheit, og vi vet input verdien vår. Det eneste vi trenger å gjøre nå er å utføre riktig konvertering.

Bruk en if/else for å sjekke om argumentet vi fikk til funksjonen er C eller F
brukt input verdien vår til å regne ut en result vardi som vi lagrer i en resultat variabel.
for formatering av resultat meldigen vil vi vite den motsatte verdien fra den vi fikk inn. Så om t='C' skal motsatt='F'


For å regne ut fra celceius to farenheit er funksjonen:
1.8 * C + 32 hvor C er temperaturen i ceceuis
om man skal fra farenheit blir formelen
(F -32) / 1.8


Nå har vi hva orginal temperaturen vår var input-verdi, og hvilken enhetn den hadde t, vi har også funnet den konverterte temperaturen og den motsatte enheten.
Vi kan nå lage en formatering tekststreng som vi skal la være vår output-verdi
output-verdi = output_verdi = input_verdi + " \u00b0" + t + " er det samme som " + resultat + " \u00b0" + motsatt;
\u00b0 er ascii koden for grade symbolet, man kan også kopiere denne verdien °

Nå har vi lyst til å legge til denne veriden inn i htmlen slik at den dukker opp på siden.
I htmlen kan man se at vi har et element som heter output, vi kan så bruke


document.querySelector('output').innerHTML = output_verdi
for å oppdatere verdien som er i dette elementer.
Her kunne vi også bruk andre elementer som kan holde på text som en div, og enten hente den slik som vi gjorde med input felted og getElementById eller querySelector etter div eller klasse.

Nå når alle disse tingene er satt opp har man en fungerende kalkultor

Eller er den helt uten feil

Hva skjer om kan ikke gir den et tall
Eller hva skjer om man ikke gir den noe input
Hva skjer om du prøver å konverter 100F til C

Fikses med å sette type=number
Fikses med å sette type=number
Fikses med å sette resultat = resultat.toFixed(2)




<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="jOjEemm" data-pen-title="Temperature" data-editable="true" data-user="Elinborg" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/Elinborg/pen/jOjEemm">
  Temperature</a> by Karina Elinborg (<a href="https://codepen.io/Elinborg">@Elinborg</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


```js
function convert_temperature(t) {

  var output, given, result, opposite;
  given = document.getElementById('temp').value;


  if (t === "C") {
    result = 1.8 * (given) + 32;
    opposite = "F";
  } else {
    result = (given - 32) / 1.8;
    opposite = "C";
  }


  result = result.toFixed(2);



  if (given) {
    output = given + " \u00b0" + t + " is equal to " + result + " \u00b0" + opposite;
  } else {
    output = "Error: Input must be a valid number";
  }


  document.querySelector('output').innerHTML = output;
}
document.getElementById('ctof').addEventListener('click', function(){convert_temperature('C');})
document.getElementById('ftoc').addEventListener('click', function(){convert_temperature('F');})

```

### Del 3 - Todo list

Her har vi en litt mer avansert appliactiosn enn den over. I tilegg til alle de nye konseptene vi lærte over skal vi her også lage ny html elementer og legge de til med javascript.
Vi ser på lister og forløkker, og knapper som kaller på flere funksjoner.


<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="dyBPQwW" data-pen-title="To Do List" data-editable="true" data-user="Elinborg" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/Elinborg/pen/dyBPQwW">
  To Do List</a> by Karina Elinborg (<a href="https://codepen.io/Elinborg">@Elinborg</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

[Gå til neste del: Deploy](/TENK-tech-camp-web-intro/posts/06_deploy)