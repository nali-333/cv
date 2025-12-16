# Conception 16/12/2025 - testprojet6.html (UI Tactile & Optimisation)

## Objectifs
* Améliorer l'ergonomie suite aux retours pédagogiques (Professeur).
* Remplacer un élément natif (`<input>`) par un composant graphique personnalisé.
* Gérer des interactions souris complexes (Clic et Glisser "Drag & Drop").

## Outils
* VS Code
* Gemini (Génération de la logique JS)
* Navigateur

## Sources
* [MDN Web Docs - Mouse Events](https://developer.mozilla.org/fr/docs/Web/API/Element/mousemove_event)

## Réalisation

**1. Analyse du besoin (Retour Professeur)**
Suite à la présentation de la version précédente, le professeur m'a conseillé de modifier la barre de notation. Le système "Slider + Texte en dessous" a été jugé peu intuitif et visuellement daté. L'objectif était de fusionner ces deux éléments en une seule barre interactive moderne.

**2. Génération du composant (Prompt Gemini)**
Ne sachant pas comment coder une barre de progression cliquable "from scratch" (de zéro), j'ai décrit le comportement fonctionnel exact à l'IA pour qu'elle génère le HTML et le JS à ma place.

> Prompt Gemini : "Je veux remplacer mon slider `<input type="range">` par une 'Barre Tactile' personnalisée. Elle doit ressembler à une barre de volume : un fond gris, et quand je clique ou glisse la souris dessus, elle se remplit avec un dégradé violet. Le texte du pourcentage doit être affiché par-dessus, au centre."

**3. Intégration et Ajustements**
J'ai remplacé le bloc HTML de l'ancien slider par le code généré (une `div` conteneur et une `div` de remplissage). J'ai ensuite intégré le script qui calcule la position de la souris (`clientX`) pour ajuster la largeur de la barre en temps réel. J'ai veillé à retirer la logique de changement de couleur (Rouge/Vert) pour garder une esthétique unie, conformément au design "Firefox Night".

## Diagramme de flux – Projet 6

```mermaid
flowchart TD
  A[Debut : Chargement Portfolio] --> B[Initialisation DOM + CSS]
  B --> C[Animation d'entree Anime.js]
  
  C --> D{Action Utilisateur}

  %% Branche 1 : Le Scroll
  D -- Scroll --> E[Detection Defilement]
  E --> F{Position > 50px ?}
  F -- Oui --> G[Navbar : Mode Opacity/Blur]
  F -- Non --> H[Navbar : Mode Transparent]
  E --> I[Intersection Observer : Animation des sections]

  %% Branche 2 : La Galerie Projet 5
  D -- Clic Boutons Galerie --> J[Changement Index Projet]
  J --> K[Recuperation Donnes JS]
  K --> L[Mise à jour Image + Texte]
  L --> D

  %% Branche 3 : La Barre Tactile Projet 6
  D -- Clic / Glisser Jauge --> M[Event Mousedown / Move]
  M --> N[Calcul Position X Souris]
  N --> O[Conversion en %]
  O --> P[Mise a jour Largeur Barre + Texte]
  P --> D
