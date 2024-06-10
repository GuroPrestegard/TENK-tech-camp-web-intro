---
layout: ../../layouts/post.astro
title: "Deploy"
description: "Deploy"
author: "gurop"
excerpt: Deploy 
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

![alt text](/src/assets/images/createrepo.png "Create repos")

## Legg til koden din 
- Etter at du har laga eit repository, klikk "creating a new file"-linken
![alt text](/src/assets/images/createFile.png "Create file")
- Gi fila navnet index.html
- Skriv inn HTML-koden din (eller bruk eksempelet under)
- Klikk på "Commit changes..."
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
- Klikk "Commit changes" når du får ein popup (du treng ikkje endre noko)

## Sett opp deployment
- Gå til Settings
- Frå menyen til venstre, klikk "Pages"
- Under branch, velger du main, og klikker save

## Sjekk ut di nye nettside! 🚀
- Øverst skal det no stå: Your site is live at...
- Klikk på lenka, eller "visit site"
- Du kan òg gå tilbake til "code"-tabben, og klikke på linken under "deployments" ute til høgre. 