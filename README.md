#Einbindung von Schriftarten (Fonts) in HTML & CSS

##Beschreibung

In dieser Anleitung lernen Teilnehmende im Modul 1 (HTML & CSS), wie sie verschiedene Schriftarten (Fonts) in ihr Projekt einbinden und anwenden können. Die Fonts befinden sich im Ordner fonts/assets/fonts und können mit der CSS-Regel @font-face integriert werden.


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


Code-Beispiele

#1. Schriftarten einbinden mit @font-face

@font-face {
    font-family: "mono";
    src: url("../fonts/TT Interphases Pro Mono Trial Regular.ttf");
}
@font-face {
    font-family: "JHM";
    src: url("../fonts/JMH Typewriter-Thin.ttf");
}
@font-face {
    .....
}


#2. Schriftarten im HTML verwenden

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
    color:#ffffff;
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
    color:#04ebac;
    background-color: #5c3cdc;
    padding: 20px;
    border-radius: 10px;
}
