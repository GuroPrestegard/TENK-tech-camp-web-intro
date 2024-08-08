## 🚀 Getting started

All commands are run from the root of the project, from a terminal:

| Command                | Action                                           |
| :--------------------- | :----------------------------------------------- |
| `npm install`          | Installs dependencies                            |
| `npm run dev`          | Starts local dev server at `localhost:3000`      |
| `npm run build`        | Build your production site to `./dist/`          |
| `npm run preview`      | Preview your build locally, before deploying     |
| `npm run astro ...`    | Run CLI commands like `astro add`, `astro check` |
| `npm run astro --help` | Get help using the Astro CLI                     |



## CSS - fasit

### oppg 2
```css 
img {
  border-radius: 50%;
} 
```
### oppg 3 
```css 
img {
  filter: grayscale(100%);
}
```
### oppg 4
```css 
img {
  rotate: 180deg;
}
```
### oppg 5 
```css 
img {
  transition: transform .7s ease-in-out;
}
```
### oppg 6 
```css
.container {
    gap: 2rem;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
```

### oppg 7
```css
.container{
  flex-direction: row-reverse;
  flex-direction: column-reverse
}
```

### oppg 8

```css
.child {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

### oppg 9 
f.eks 
```html
<section>
	<div id="heading">
		<p>🌸</p>
		<h1>Mi flotte nettside</h1>
		<p>🌸</p>
	</div>
	<p>Litt tekst</p>
	<div id="picture-container">
		<img  src="https://vetericyn.com/Vetericyn/wp-content/uploads/2024/04/Benefits-of-Chondroitin-for-Dogs-350x350.jpg" alt="ein hund" width="350" height="350">
		<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Lucy_the_Dog_at_The_Green%2C_Town_Square_Las_Vegas.jpg/1600px-Lucy_the_Dog_at_The_Green%2C_Town_Square_Las_Vegas.jpg?20200314225253" alt="golden retriver" width="350" height="350"/>
	</div>
</section>
```

```css
section {
    display:flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
}
#picture-container {
    display: flex;
    gap: 2rem;
}
#heading {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
}
```

## JavaScript fasit

### Oppgave 1
```js
var alder = 87
var navn = "Harald"
console.log(alder)
console.log(navn)

var navn = "Karina"
var alder = 87-41
console.log(alder)
console.log(navn)
```


### Oppgave 2

```js

function hello() {
	console.log("Hello world!")
}


function hello(navn) {
	console.log("Hei, " + navn)
}
```


### Oppgave 3
```js
function hello(navn, alder) {
	if (alder > 26) {
		console.log(navn, " du er eldre en meg")
	}
	else {
		console.log(navn, "er bare ", alder, " år gammel")
	}
}

```


### Oppgave 4

```js
var cTof = document.getElementById("ctof")
var fToc = document.getElementById("ftoc")
cTof.addEventListener("click", konverter_temperatur())
fToc.addEventListener("click", konverter_temperatur())

// i funksjonen
console.log("En knapp ble trykket på")
```


### Oppgave 5
```js
cTof.addEventListener("click",function() {konverter_temperatur("C")})
fToc.addEventListener("click", function()
{konverter_temperatur("F")})

// I funksjonen
if enhet == "C" {
	console.log("Konverter fra C til F")
}
else {
	console.log("Konverterer fra F to C")
}
```

### Oppgave 6
```js
document.getElementById('input-field')
```


### Oppgave 7

```js
input_verdi = document.getElementById('input-field')

console.log("Inputfeltet har verdien ", input_verdi)
```


### Oppgave 8
```js
if enhet == "C" {
	resultat = 1.8 * input_verdi + 32
	motsatt = "F"
}
else {
	result = (enhet - 32) / 1.8
	mosatt = "C"
}
```


### Oppgave 9
```js
output_verdi = input_verdi + " \u00b0" + enhet + " er det samme som " + resultat + " \u00b0" + motsatt
```


### Oppgave 10
```js
document.querySelector('output').innerHTML = output_verdi
```

### Oppgave 11

```js
_ °C er det samme som 32 °F
_ °F er det samme som -17.77777777777778 °C
abc °F er det samme som NaN °C
100 °F er det samme som 37.77777777777778 °C
```

### Oppgave 12
```js
//HTML
<input type="string" id=input-field>
->
<input type="number" id=input-field>

if (input_verdi) {
	//calculate output_verdi
}
else {
	output_verdi = "Feilmelding: Input må være et tall"
}

```

### Oppagve 13

```js
// Før vi lager en formatert string så runder vi av resultat variabelen

resultat = resultat.toFixed(2)
```
