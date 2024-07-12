---
layout: ../../layouts/post.astro
title: "Deploy"
description: "Deploy"
author: "gurop"
excerpt: No har me lært å lage ein nettside. Men korleis skal me få gjort det slik at andre òg får sjå den? Det gjer me ved å “deploye” nettsida. 
image:
  src:
  alt:
tags: ["nivå5"]
---

No har me lært å lage ein nettside. Men korleis skal me få gjort det slik at andre òg får sjå den? Det gjer me ved å 
"deploye" nettsida. Akkurat kva som skjer når man deployer treng me ikkje gå inn på her, men det held å sei at me laster
opp koden vår slik at den kan verte køyrt og blir synleg for andre.

Det finst mange forskjellige tenestar ein kan bruke for å gjere ei nettside tilgjengelig på nett. Ein av dei enklaste er
kanskje github pages. Denne nettsida, som alle oppgåvene står i, er hosta på github pages! 

La oss sette i gong :)

## Lag konto
Det fyrste ein må gjere, er å lage ein GitHub-konto. Til det treng du ei e-post adresse. 

- Gå til https://github.com/, og klikk "Sign up" i høgre hjørne.
- Følg instruksjonane for å oppretta brukaren. 

## Opprett ei ny mappe (repository)
- Trykk på "+"-knappen oppe i høgre hjørne
- Velg "New repository" frå nedtrekksmenyen.
- Fyll inn navn
- Velg "public" 
  - For gratis konto må repository vera public for å kunne publiserast som GitHub pages. Dette betyr at alt du legg til i dette repositoriet er tilgjengelig for alle. 
- Trykk "Create repository"

![alt text](/public/assets/images/createrepo.png "Create repos")

## Legg til koden din 
- Etter at du har laga eit repository, klikk "creating a new file"-linken
![alt text](/public/assets/images/createFile.png "Create file")
- Gi fila navnet index.html
- Skriv inn HTML-koden din (eller bruk eksempelet under)
- Klikk på "Commit changes..."
- Klikk "Commit changes" når du får ein popup (du treng ikkje endre noko)
```html
<!DOCTYPE html>
<html>
<head>
<title>Nettsida mi</title>
</head>
<body>

<h1>Velkommen til nettsida mi!✨</h1>

</body>
</html>
```

## Sett opp deployment
- Gå til Settings
- Frå menyen til venstre, klikk "Pages"
- Under branch, velger du main, og klikker save

## Sjekk ut di nye nettside! 🚀
- Øverst skal det no stå: Your site is live at...
- Klikk på lenka, eller "visit site"
- Du kan òg gå tilbake til "code"-tabben, og klikke på linken under "deployments" ute til høgre. Klikk på linken du finn der. 

## Legg til CSS 💅
Det finst to måtar å legge til CSS i ei HTML-fil. Enten, kan du bruke <code class="language-plaintext highlighter-rouge">&lt;style&gt;</code> tags, eller du kan linke til ei
css-fil som inneheld stylinga di. Me prøvar oss på ein <code class="language-plaintext highlighter-rouge">&lt;style&gt;</code>-tag her. 

- opne index.html fila i github. 
- trykk på blyanten i høgre hjørne. 
- inne i  <code class="language-plaintext highlighter-rouge">&lt;head&gt;</code>-taggen, legg du til ein <code class="language-plaintext highlighter-rouge">&lt;style&gt;</code> tag. 
- Her legg du til stylinga du vil ha. F.eks slik som i eksempelet under
- Trykk på "commit changes..."
- Klikk "Commit changes" når du får ein popup (du treng ikkje endre noko)
- Vent til sida di er ferdig med å deploye (du kan sjekke status til høgre i code-tabben)
- Sjekk resultat!

```html
<!DOCTYPE html>
<html>
<head>
  <title>Nettsida mi</title>
  <style>
    h1 {
      color: pink;
    }
  </style>
</head>
<body>

<h1>Velkommen til nettsida mi!✨</h1>

</body>
</html>
```

## Legg til ei ny side
- Opprett ei ny fil ved å trykke på pluss-tegnet til høgre når du står på "code"-tabben. Kall fila noko som passar med det innhaldet du vil vise (og slutt med .html). Eg kalla mi fil dogs.html.
- Legg til innhald på sida, f.eks ei side om hundar som i eksempelet under.
- Commit changes som me har gjort tidlegare. 
- Opne index.html, og trykk på blyanten. 
- Legg til ei lenke til den nye sida du laga. Sidan eg kalla mi fil dogs.html, blir lenka ```<a href="./dogs.html">Gå til hundar</a>```
- Commit changes som me har gjort tidlegare. 
- Vent til nettsida har deploya på nytt, og sjekk resultatet. 
- P.S pass på å referere til fila på rett måte. Dersom filene er i samme mappe, bruk ./ før filnamnet. Dersom fila er i ei mappe over, bruk ../ før filnamnet. Dersom fila er i ei mappe under, som f.eks heiter pages, bruk ./pages/ før filnamnet. 


```html title="dogs.html"
<!DOCTYPE html>
<html>
<head>
  <title>Hundar</title>
</head>
<body>

<h1>Her finn du eit bilde av ein hund</h1>
<img src="https://i.natgeofe.com/n/4f5aaece-3300-41a4-b2a8-ed2708a0a27c/domestic-dog_thumb_3x2.jpg" 
     alt="ein hund" 
     width="500" 
     height="350">

</body>
</html>
```