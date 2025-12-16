# Conception  - testprojet3.html (Intégration Multimédia)

## Objectifs
* Enrichir le site avec du contenu externe (Vidéo).
* Comprendre et utiliser la balise HTML `<iframe>`.
* Adapter la mise en page pour intégrer un lecteur média.

## Outils
* VS Code
* YouTube (Fonction "Partager" > "Intégrer")
* Navigateur

## Sources
* [MDN Web Docs - Élément Iframe](https://developer.mozilla.org/fr/docs/Web/HTML/Element/iframe)
* [Support Google - Intégrer des vidéos](https://support.google.com/youtube/answer/171780)

## Réalisation

**1. Récupération du code d'intégration (Source Externe)**
Je suis allé sur ma vidéo YouTube, j'ai cliqué sur "Partager" puis "Intégrer". YouTube m'a fourni un bloc de code HTML prêt à l'emploi commençant par `<iframe...`.

**2. Intégration dans le HTML **
J'ai copié ce code dans ma page `testprojet3.html`, à l'endroit désiré (sous les compétences). J'ai découvert que la balise `<iframe>` permet d'ouvrir une "fenêtre" vers un autre site à l'intérieur du mien.

**3. Ajustement des dimensions (CSS/HTML)**
Pour que la vidéo ne soit ni trop petite ni trop grande, j'ai modifié les attributs `width` (largeur) et `height` (hauteur) directement dans la balise ou via le CSS, afin qu'elle s'aligne correctement avec le reste de mon design.
