# Convention de nommage — Festival Résonances

## 1. Objectif

Ce document définit les conventions de nommage des composants et des layouts du site Festival Résonances.

L'organisation repose sur la méthodologie SMACSS afin de faciliter la réutilisation, la maintenance et l'évolution des styles.

Les noms sont écrits en minuscules, avec des mots séparés par des tirets (kebab-case).

## 2. Préfixes retenus

* `l-` : désigne un layout ou un élément de structure d'une page ( `l-container`).
* `is-` : désigne un état actif ou temporaire ( `is-active`).
* `has-` : indique la présence d'un état particulier (`has-error`).
* `theme-` : désigne un thème visuel ( `theme-lac`).

Les modules réutilisables ne possèdent pas de préfixe obligatoire.

## 3. Inventaire des composants

* `site-header` : représente l'en-tête commun aux cinq pages. Il contient le logo et la navigation principale. Il peut présenter un lien actif.
* `site-nav` : représente la navigation principale du site. Elle est présente sur toutes les pages et possède un état actif.
* `btn` : désigne les boutons d'action utilisés sur les différentes pages. Il possède trois variantes : principal, secondaire et contour.
* `hero` : désigne le grand bandeau de présentation de la page d'accueil, avec une image et du texte.
* `artist-card` : représente une carte d'artiste utilisée sur l'accueil, le programme et la fiche artiste. Elle possède une version standard et une version tête d'affiche.
* `stage-badge` : identifie la scène associée à un artiste. Il existe trois variantes : lac, forêt et kiosque.
* `stage-card` : présente les trois scènes du festival sur la page d'accueil. Chaque scène possède sa propre couleur.
* `program-filter` : permet de filtrer les artistes sur la page programme. Il possède un état par défaut et un état sélectionné.
* `ticket-card` : présente les différentes formules de billetterie. Il possède une version standard et une version recommandée.
* `form-field` : représente les champs de formulaire de la billetterie. Il possède un état par défaut, un état de focus et un état d'erreur.
* `booking-form` : regroupe les champs nécessaires à la réservation et à la validation du formulaire.
* `info-card` : présente les informations pratiques concernant les accès, les horaires et les services sur place.
* `faq-item` : représente une question fréquente sur la page des informations pratiques. Elle peut être ouverte ou fermée.
* `contact-banner` : désigne le bandeau invitant les visiteurs à contacter l'organisation, accompagné d'un bouton.
* `site-footer` : représente le pied de page commun aux cinq pages. Il regroupe les liens utiles et les informations de la newsletter.

## 4. Inventaire des layouts

Les layouts correspondent aux grandes zones qui organisent le contenu des pages. Ils sont identifiés par le préfixe `l-`.

* `l-container` : permet de limiter et de centrer la largeur du contenu.
* `l-header` : organise les différents éléments de l'en-tête.
* `l-main` : structure la zone principale de chaque page.
* `l-section` : organise les grandes sections et leurs espacements.
* `l-artist-grid` : organise les cartes d'artistes sous forme de grille.
* `l-ticket-grid` : organise les différentes formules de billetterie.
* `l-info-grid` : organise les cartes d'informations pratiques.
* `l-footer` : organise les différentes zones du pied de page.

## 5. États des composants

Les états sont identifiés par les préfixes `is-` et `has-`.

* `is-active` : indique qu'un élément est sélectionné, par exemple un filtre du programme.
* `is-open` : indique qu'une question de la FAQ est ouverte.
* `has-error` : indique qu'un champ de formulaire contient une erreur.

Les pseudo-classes CSS `:hover`, `:focus-visible` et `:checked` sont utilisées pour gérer les interactions lorsque cela est adapté.

## 6. Thèmes visuels

Les thèmes permettent d'identifier les trois scènes du festival et de conserver une cohérence visuelle.

* `theme-lac` : correspond à la Scène du Lac. Sa couleur principale est `#1F4E8C` et son texte est blanc (`#FFFFFF`).
* `theme-foret` : correspond à la Scène de la Forêt. Sa couleur principale est `#2F6B3A` et son texte est blanc (`#FFFFFF`).
* `theme-kiosque` : correspond au Kiosque. Sa couleur principale est `#B87A1E` et son texte est `#1C1B2E`.

## 7. Règles générales de nommage

* Utiliser des noms explicites et compréhensibles.
* Écrire les noms en minuscules et séparer les mots par des tirets.
* Réutiliser les mêmes noms pour les mêmes composants.
* Distinguer les modules des layouts.
* Utiliser les classes d'état uniquement lorsqu'un état doit être représenté.
* Mettre à jour ce document si les noms évoluent pendant le développement.

## 8. Organisation SMACSS

Les styles sont répartis dans les catégories suivantes :

* `abstracts/` : contient les variables et les mixins réutilisables.
* `base/` : contient le reset et les styles typographiques des éléments HTML.
* `layout/` : contient les règles de structure générale des pages.
* `modules/` : contient les composants réutilisables du site.
* `state/` : contient les styles des différents états des composants.
* `theme/` : contient les couleurs et les variations visuelles du festival.

Le fichier `main.scss` constitue le point d'entrée de la compilation Sass.
