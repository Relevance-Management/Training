# Bazele dezvoltarii web pentru incepatori

## 1. Ce este HTTP si cum functioneaza?

HTTP (Hypertext Transfer Protocol) este protocolul fundamental utilizat pentru transferul de date pe World Wide Web. Iata cum functioneaza:

1. Clientul (de obicei un browser web) trimite o cerere HTTP catre un server.
2. Serverul proceseaza cererea si trimite inapoi un raspuns HTTP.
3. Raspunsul contine informatii despre starea cererii si, de obicei, continutul solicitat (pagina web, imagine, etc.).

Exemplu simplu:
1. Utilizatorul tasteaza www.exemplu.ro in browser.
2. Browserul trimite o cerere GET HTTP catre serverul exemplu.ro.
3. Serverul raspunde cu codul de stare 200 (OK) si continutul paginii web.

## 2. HTML - Structura unei pagini web

HTML (Hypertext Markup Language) este folosit pentru a structura continutul unei pagini web.

Exemplu de structura HTML de baza:

```html
<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <title>Prima mea pagina web</title>
</head>
<body>
    <h1>Bine ati venit pe site-ul meu!</h1>
    <p>Acesta este un paragraf de text.</p>
</body>
</html>
```

## 3. CSS - Stilizarea paginilor web

CSS (Cascading Style Sheets) este folosit pentru a controla aspectul si formatul elementelor HTML.

Exemplu de CSS de baza:

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
}

h1 {
    color: #333;
    text-align: center;
}

p {
    color: #666;
    line-height: 1.6;
}
```

## 4. JavaScript - Adaugarea interactivitatii

JavaScript permite adaugarea de functionalitati interactive pe paginile web.

Exemplu simplu de JavaScript:

```javascript
function salutare() {
    let nume = prompt("Cum te numesti?");
    alert("Salut, " + nume + "! Bine ai venit pe site-ul meu.");
}
```

## 5. Proiect demonstrativ: Pagina personala simpla

Vom crea o pagina web personala simpla care combina HTML, CSS si JavaScript.

### index.html
```html
<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <title>Pagina mea personala</title>
    <link rel="stylesheet" href="stil.css">
</head>
<body>
    <header>
        <h1>Bine ati venit pe pagina mea!</h1>
    </header>
    <main>
        <section>
            <h2>Despre mine</h2>
            <p>Sunt un dezvoltator web incepator, pasionat de tehnologie si invatare continua.</p>
        </section>
        <section>
            <h2>Proiecte</h2>
            <ul>
                <li>Pagina personala</li>
                <li>Calculator simplu</li>
                <li>Lista de sarcini</li>
            </ul>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Numele Meu</p>
        <button onclick="salutare()">Spune Salut!</button>
    </footer>
    <script src="script.js"></script>
</body>
</html>
```

### stil.css
```css
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header, main, footer {
    padding: 20px;
    max-width: 800px;
    margin: 0 auto;
}

header {
    background-color: #333;
    color: #fff;
    text-align: center;
}

h1, h2 {
    margin-bottom: 20px;
}

ul {
    list-style-type: square;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    position: fixed;
    bottom: 0;
    width: 100%;
}

button {
    background-color: #4CAF50;
    border: none;
    color: white;
    padding: 10px 20px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
}
```

### script.js
```javascript
function salutare() {
    let nume = prompt("Cum te numesti?");
    if (nume) {
        alert("Salut, " + nume + "! Multumesc ca ai vizitat pagina mea.");
    } else {
        alert("Salut! Multumesc ca ai vizitat pagina mea.");
    }
}
```

Acest proiect demonstrativ combina elementele de baza ale HTML, CSS si JavaScript pentru a crea o pagina web personala simpla, dar functionala. Incurajeaza cursantii sa experimenteze cu codul, sa modifice stilurile si sa adauge noi functionalitati pentru a-si imbunatati intelegerea si abilitatile.
