# Conception [Date] - testprojet2.html (Version Dynamique & Librairie)

## Objectifs
* Passer d'un code HTML statique à une génération dynamique (Algorithmique).
* Séparer les données (Data) de l'affichage (DOM).
* Intégrer une librairie externe d'animation (**Anime.js**).

## Outils
* VS Code
* Gemini (Modèle Pro)
* Documentation Anime.js

## Sources
* [Documentation officielle Anime.js](https://animejs.com/documentation/)
* [MDN Web Docs - Array.prototype.forEach()](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) (Pour comprendre comment parcourir mes données)


## Réalisation

**1. Structuration des données (Fait main)**
Après avoir lu la documentation sur les tableaux en JavaScript, j'ai décidé de ne plus écrire mes compétences "en dur" dans le HTML, mais de créer une structure de données flexible dans le script. J'ai écrit moi-même le tableau d'objets pour pouvoir modifier mes pourcentages facilement :

```javascript
const skillsData = [
    { name: "Collaboration", level: 90, color: "#bf5af2" },
    { name: "Adaptabilité", level: 85, color: "#0a84ff" },
    // ...
];
