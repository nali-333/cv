# Conception - testprojet3.html (Interactivité Utilisateur)

## Objectifs
* Ajouter une dimension participative au site (User Input).
* Manipuler le DOM en temps réel sans recharger la page.
* Créer une logique conditionnelle visuelle (changement de couleur dynamique).

## Outils
* VS Code
* Gemini
* Navigateur (Inspecteur d'éléments pour tester les événements)

## Sources
* [MDN Web Docs - L'élément Input Range](https://developer.mozilla.org/fr/docs/Web/HTML/Element/input/range)
* [W3Schools - JavaScript HTML DOM EventListener](https://www.w3schools.com/js/js_htmldom_eventlistener.asp)

## Réalisation

**1. Création de l'élément d'interface **
Pour permettre à l'utilisateur de donner son avis, j'ai consulté la documentation MDN et ajouté manuellement la balise input de type range dans mon code HTML, en définissant les bornes min (0) et max (100).

**2. Écoute de l'événement (Inspiration Tuto + Code perso)**
J'ai compris via W3Schools qu'il fallait utiliser `addEventListener('input', ...)` pour détecter quand l'utilisateur bouge le curseur. J'ai commencé à écrire la fonction pour récupérer la valeur `e.target.value`.

**3. Logique conditionnelle complexe (Prompt Gemini)**
Je voulais que la barre change de couleur automatiquement selon la note (Rouge si c'est mauvais, Vert si c'est bon). J'ai demandé à l'IA de m'écrire cette structure conditionnelle if/else optimisée.

Prompt Gemini :
"Je suis en train de créer un slider en JS. Je récupère la valeur dans une variable `val`. Peux-tu m'écrire le bloc `if/else` qui change la couleur de fond de ma div `#user-skill-fill` selon ces règles : Rouge en dessous de 40%, Orange en dessous de 75%, et Vert au-dessus ?"

**4. Intégration et Tests**
J'ai fusionné le code généré dans mon EventListener. J'ai ensuite testé le rendu en direct pour vérifier que la transition de couleur se faisait bien instantanément lors du glissement de la souris.
