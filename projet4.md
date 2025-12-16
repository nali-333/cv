# Conception  - testprojet4.html (Design  & Scroll)

## Objectifs
* Moderniser l'interface graphique 
* Détecter le défilement de la page (Scroll Event).
* Créer une barre de navigation réactive qui change d'aspect au défilement.

## Outils
* VS Code
* Gemini (Génération de CSS et Logique JS)
* Navigateur

## Sources
* [MDN Web Docs - L'événement Scroll](https://developer.mozilla.org/fr/docs/Web/API/Document/scroll_event)
* [CSS Gradient](https://cssgradient.io/)

## Réalisation

**1. Recherche du style graphique (Prompt Gemini)**
Je voulais un design très spécifique rappelant l'univers . Au lieu de chercher les codes couleurs hexadécimaux un par un, j'ai demandé à l'IA de me générer une base CSS.

> Prompt Gemini : "Je veux refaire le design de ma page. Donne-moi un code CSS pour un fond sombre avec des dégradés violets et oranges, inspiré du style de ça (screen). Ajoute aussi du style pour des cartes avec des coins arrondis."

**2. Intégration du Scroll en JavaScript (Prompt Gemini)**
Je souhaitais que l'interface réagisse quand l'utilisateur descend dans la page (par exemple, changer la transparence du header). Ne connaissant pas la syntaxe exacte, j'ai sollicité une explication.

> Prompt Gemini : "Comment faire en JavaScript pour détecter quand l'utilisateur scrolle vers le bas ? Je veux ajouter une classe 'sticky' à ma barre de navigation quand on dépasse 50 pixels de hauteur."

**3. Mise en place de la logique **
J'ai récupéré le code fourni : `window.addEventListener('scroll', ...)` et la condition `if (window.scrollY > 50)`. J'ai inséré ce bloc dans mon fichier script existant pour combiner cette nouvelle fonctionnalité avec mes animations précédentes.
