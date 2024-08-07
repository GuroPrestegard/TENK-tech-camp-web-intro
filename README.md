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