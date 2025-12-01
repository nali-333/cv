# Projet prévu : Barres de compétences animées (Anime.js)

## Contexte et objectif
Je suis débutant en développement web et j'ai pour projet d'améliorer visuellement mon CV en ligne en ajoutant des barres de compétences animées. Je souhaite qu'au chargement de la page (ou au scroll), chaque barre se remplisse progressivement pour représenter mon niveau sur des soft skills important de mon parcours.

## Plan d’action
1. Préparer le HTML : remplacer la partie "Mon approche et mes atouts"de mon CV pour ajouter une section « Compétences » dans ma page CV et créer une structure de barres avec des attributs `data-skill`.  
2. Styliser en CSS : définir l’apparence des barres (fond, hauteur, coins arrondis, label).  
3. Animer en JS avec Anime.js : lire les `data-skill` et animer la largeur.
4. Test et ajustements : vérifier sur mobile/desktop, ajuster durées et pourcentages.  
5. Si possible : déclencher l’animation au scroll et ajouter un compteur numérique qui s’incrémente.

## Mon niveau et objectifs d’apprentissage
- En tant que débutant j’en profiterai pour me familiariser avec la liaison HTML/CSS/JS et l’utilisation d’une bibliothèque externe (Anime.js).  
- Objectifs : comprendre comment cibler plusieurs éléments, orchestrer des animations simples, et intégrer proprement le code à mon CV existant.
- Personnaliser les couleurs par compétence ou ajouter des icônes.

# Projet : Barres de compétences animées (Anime.js)

## Contexte et objectif
Je suis débutant en développement web et j'ai pour projet d'améliorer visuellement mon CV en ligne en ajoutant des barres de compétences animées. Je souhaite qu'au chargement de la page (ou au scroll), chaque barre se remplisse progressivement pour représenter mon niveau sur des soft skills importants de mon parcours.

## Plan d’action
1. **Préparer le HTML :** Remplacer la partie "Mon approche et mes atouts" de mon CV pour ajouter une section « Compétences » et créer une structure de barres avec des attributs `data-skill`.
2. **Styliser en CSS :** Définir l’apparence des barres (fond, hauteur, coins arrondis, label).
3. **Animer en JS avec Anime.js :** Lire les `data-skill` et animer la largeur.
4. **Test et ajustements :** Vérifier sur mobile/desktop, ajuster durées et pourcentages.
5. **Si possible :** Déclencher l’animation au scroll et ajouter un compteur numérique qui s’incrémente.

## Mon niveau et objectifs d’apprentissage
- En tant que débutant, j’en profiterai pour me familiariser avec la liaison HTML/CSS/JS et l’utilisation d’une bibliothèque externe (**Anime.js**).
- **Objectifs :** Comprendre comment cibler plusieurs éléments, orchestrer des animations simples, et intégrer proprement le code à mon CV existant.
- Personnaliser les couleurs par compétence ou ajouter des icônes.

---

##  Mise en œuvre et Documentation

Evolution du projet, documentée étape par étape avec les interactions IA (Modèle utilisé : Google Gemini).

###  Version 1 : Première implémentation 
**Fichier :** [testprojet.html](https://nali-333.github.io/cv/testprojet.html)
* **Objectif :** Valider le fonctionnement de la librairie **Anime.js** sur une structure HTML simple.
* **Prompt Technique utilisé :**
    > "Je souhaite implémenter une animation de barre de progression avec la bibliothèque Anime.js. 
* **Analyse de la solution :** L'IA a proposé un script utilisant `document.querySelectorAll` pour cibler les barres, puis une boucle `anime()` basique. J'ai compris comment la propriété CSS est manipulée par le moteur d'animation.

###  Version 2 : Refonte du Design (UI/UX)
**Fichier :** [testprojet1.html](https://nali-333.github.io/cv/testprojet1.html)
* **Objectif :** Améliorer l'esthétique pour un rendu professionnel (Dark Mode, contrastes) correspondant à ma charte graphique.
* **Prompt Technique utilisé :**
    > "Le rendu actuel est trop basique. Je souhaite moderniser l'interface avec un thème sombre. Pourriez-vous proposer un CSS utilisant des contrastes forts et des couleurs   pour chaque compétence ?"


###  Version 3 : Approche Algorithmique & Interactivité 
**Fichier :** [testprojet3.html](https://nali-333.github.io/cv/testprojet3.html)
* **Objectif Majeur :** Refactoriser le code pour respecter les principes du cours et ajouter une interaction utilisateur.
* **Prompt Technique utilisé :**
    > "Mon code actuel déclare les barres 'en dur' dans le HTML,  Je souhaite **générer le DOM de manière algorithmique**  De plus, comment puis-je ajouter une barre d'évaluation  pour interagir avec Anime.js en temps réel ?"
* **Solution Implémentée :**
    1.  **Structure de données :** Création d'un tableau d'objets `skillsData` (séparation fond/forme).
    2.  **Génération DOM :** Utilisation d'une boucle `forEach` couplée à `document.createElement` pour injecter les éléments dynamiquement.
    3.  **Event Listener :** Ajout d'une écoute sur l'événement `input` du slider pour mettre à jour la largeur et la couleur de la barre instantanément.




