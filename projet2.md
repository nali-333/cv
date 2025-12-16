# Conception  - testprojet2.html (Interactivité Utilisateur)

## Objectifs
* Ajouter une dimension participative au site (User Input).
* Manipuler le DOM en temps réel (récupérer la valeur du slider).
* Créer une logique conditionnelle visuelle (changement de couleur).

## Outils
* VS Code
* Gemini
* Navigateur (Inspecteur)

## Sources
* [MDN Web Docs - L'élément Input Range](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/range)

## Réalisation

**1. Création de l'interface **
J'ai ajouté la balise `<input type="range">` dans le HTML pour créer la barre de notation, en fixant les attributs `min="0"` et `max="100"`.

**2. Écoute de l'événement (JavaScript)**
J'ai utilisé `addEventListener('input', ...)` pour détecter le mouvement du curseur. Cela permet de mettre à jour le pourcentage affiché en temps réel sans recharger la page.

**3. Logique conditionnelle (Prompt Gemini)**
Pour rendre l'interface vivante, j'ai demandé à l'IA une structure `if/else` qui change la couleur de la barre selon la note (Rouge < 40%, Orange < 75%, Vert > 75%).
