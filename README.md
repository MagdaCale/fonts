# Einbindung von Schriftarten (Fonts) in HTML & CSS

## Übersicht

Diese Anleitung zeigt Schritt für Schritt, wie Schriftarten in einem HTML- und CSS-Projekt eingebunden und verwendet werden können. Die bereitgestellten Fonts befinden sich im Ordner `fonts/assets/fonts` und können mit der CSS-Regel `@font-face` eingebunden werden.

---

## Verzeichnisstruktur

```plaintext
project-folder/
├── assets/
│   └── fonts/
│       ├── JMH Typewriter-Thin.ttf
│       ├── Jura-VariableFont_wght.ttf
│       ├── LEMONMILK-Regular.otf
│       ├── NectoMono-Regular.otf
│       ├── OldNewspaperTypes.ttf
│       └── TT Interphases Pro Mono Trial Regular.ttf
├── index.html
└── styles.css
```


## Schritt 1: Schriftarten einbinden

Um Schriftarten in dein Projekt einzubinden, verwende die CSS-Regel `@font-face`. Dies ermöglicht dir, benutzerdefinierte Schriftarten zu definieren, die du später in deinem HTML und CSS verwenden kannst.

### Beispiel-Code

```css
@font-face {
    font-family: "mono";
    src: url("../fonts/TT Interphases Pro Mono Trial Regular.ttf");
}
@font-face {
    font-family: "JHM";
    src: url("../fonts/JMH Typewriter-Thin.ttf");
}
@font-face {
    font-family: "lemon";
    src: url("../fonts/LEMONMILK-Regular.otf");
}
@font-face {
    font-family: "oldNewspaper";
    src: url("../fonts/OldNewspaperTypes.ttf");
}
@font-face {
    font-family: "necto";
    src: url("../fonts/NectoMono-Regular.otf");
}
@font-face {
    font-family: "jura";
    src: url("../fonts/Jura-VariableFont_wght.ttf");
}
```


## Schritt 2: Schriftarten im CSS verwenden

Nach der Definition der Schriftarten kannst du sie mithilfe der font-family-Eigenschaft verschiedenen HTML-Elementen zuweisen.

### Beispiel-Code

```css
body {
    text-align: center;
}

h1 {
    background-color: #5c3cdc;
    margin: 0 auto;
    color: #04ebac;
    width: 650px;
    border-radius: 5px;
    font-family: "mono";
    padding: 5px 0;
}

main {
    color: #5c3cdc;
    margin: 0 auto;
    width: 650px;
}

article:nth-of-type(1) p {
    font-family: "oldNewspaper"; 
    font-size: 20px;
}

article:nth-of-type(2) p {
    font-family: "lemon"; 
    font-size: 15px;
}

article:nth-of-type(3) p {
    font-family: "JHM"; 
    font-size: 25px;
    color: #ffffff;
    background-color: #04ebac;
    padding: 20px;
    border-radius: 10px;
}

article:nth-of-type(4) p {
    font-family: "necto"; 
    font-size: 18px;
}

article:nth-of-type(5) p {
    font-family: "jura";
    font-size: 12px;
    color: #04ebac;
    background-color: #5c3cdc;
    padding: 20px;
    border-radius: 10px;
}
```



