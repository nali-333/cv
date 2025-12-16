# Conception  - testprojet3.html (Animation Library)

## Objectifs
* Découvrir et intégrer une librairie externe (Anime.js).
* Animer les éléments du DOM (titres, barres de compétences) au chargement.
* Comprendre la syntaxe des objets en JS (targets, easing, duration).

## Outils
* VS Code
* Gemini
* Librairie Anime.js (CDN)

## Sources
* [Documentation Anime.js](https://animejs.com/documentation/)

## Réalisation

**1. Importation de la librairie**
J'ai appris à relier une librairie externe en ajoutant la balise `<script src="...">` pointant vers le CDN d'Anime.js dans mon fichier HTML.

**2. Animation d'entrée (Code + Tuto)**
Au lieu d'utiliser des transitions CSS classiques, j'ai écrit un script JS utilisant `anime({...})`. J'ai ciblé les éléments (comme `.skill-fill` ou les titres) pour les faire apparaître progressivement (translation + opacité).

**3. Configuration des délais (Staggering)**
J'ai utilisé la propriété `delay: anime.stagger(100)` pour que les éléments n'apparaissent pas tous en même temps, mais en cascade, ce qui donne un effet plus professionnel.
