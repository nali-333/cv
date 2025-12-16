# Conception  - testprojet5.html (Portfolio Universitaire)

## Objectifs
* Ajouter une nouvelle section dédiée aux projets universitaires.
* Intégrer des cartes de présentation (Cards) avec images et descriptions.
* Générer des images d'illustration automatiques via des liens (Placeholders).

## Outils
* VS Code
* Gemini (Utilisé à 100% pour la génération de cette section)
* Navigateur



## Réalisation

**1. Ajout de la section "Projets" (Prompt de Structure)**
Je voulais insérer mes travaux d'école au milieu de la page existante. Pour cette partie spécifique, je n'ai rien codé à la main. J'ai demandé à l'IA de générer le bloc HTML complet.

> Prompt Gemini : "Ajoute une nouvelle section 'Projets Universitaires' sous les compétences. Je veux une présentation en grille avec 3 cartes de projets. Chaque carte doit avoir une image, un titre et un petit texte."

**2. Génération des Images d'illustration (Prompt Visuel)**
N'ayant pas mes propres images sous la main, j'ai demandé à l'IA comment intégrer des visuels fictifs automatiquement. Elle m'a expliqué comment utiliser des services de "Placeholders" via des URL.

> Prompt Gemini : "Je n'ai pas encore les images. Peux-tu mettre des liens d'images temporaires (placeholders) dans le code `<img>` qui affichent des thèmes technologiques aléatoires ?"

**3. Style et Intégration (Approche 100% Prompt)**
J'ai copié-collé le résultat fourni par Gemini. Le code CSS (pour l'alignement des cartes et l'esthétique) et le HTML ont été générés en une seule fois par l'IA pour s'adapter au design que j'avais déjà mis en place dans la version précédente.
