# Test CMS monsitevert

Tests du CMS monsitevert et rédaction d'une documentation.

# Dashboard documentation

## Pages
- Créer une nouvelle page ou modifier une page existante
- L'icône de paramètre en haut à droite vert permet de modifier les paramètres généraux de la page (SEO, description, ect). L'icône poubelle permet de supprimer la page.
- Dans le menu à droite on a accès à 4icônes :
    - Icône permettant d'ajouter les blocks avec un système de drag and drop et quelques otpions supplémentaires (ajout de texte et de formulaire)
    - Icône des blocks et de leur hiérarchie. Permet également de les pointer avec plus de précision que sur le model à modifier à gauche.
    - Pinceaux permet une stylisation rapide du block par rapport à sa position, sa taille et des paramètres de font.
    - Icône paramètres pour voir les paramètres en code (type de balise, id du block, etc).
    Icône de code permet de modifier en code le bloc (html et css). On peut ajouter, modifier du texte, etc. Le css s'ajoute avec la propriété style dans la balise html. Ensuite en sauvegardant un id est automatiquement généré pour ranger le css dans la section correspondante.


## Articles
## Catégories
## Menus
## Thème

## Paramètres

Dans cette section il est possible de prédéfinir plusieurs comportements via les sections suivantes :

### Global
- Titre, url, logo et favicon du site ainsi que 2 checkbox pour confirmer que le site n'utilise pas de cookies et afficher "mon site vert".
### Optimization des assets
- Compression des images jpeg, png et gif ainsi qu'une checkbox pour tester la version BETA de compression de tous les formats d'image.
### SEO
- Permet de choisir la langue, le comportement du robot, de nouveau l'URL du site, lien page 404 (à créer dans pages) avec son titre et sa description, lien utilisateur Twitter, image mise en avant et Id+json
### Formulaire de contact
- adresse email reçevant les demandes de contact et options de reCAPTCHA

# Travail perso et questions pour mieux comprendre le CMS

## To do

- Recréer template acceuil Koudetat pour bien voir visuellement ce que tu peux faire

## Questions et remarques

- Où est-ce qu'on obtiens les liens de pages (si il s'agit bien d'une demande de lien de page) pour les mettre dans les thèmes du site par exemple ? Est-ce que dans Pages > Paramètre de page c'est le nom ou le slug de la page qu'on utilise ?

- Dans paramètre > SEO :
    - Qu'est-ce que index, follow, noindex, nofollow ?
    - L'image mise en avant apparait dans le navigateur de recherche ?
    - Qu'est-ce que Id+json ?


- qu'est-ce que les classes "hero-section" et "hero-content" (vous avez une documentation concernant vos classes ?)

- Peut-on générer nos propre classes ou tout est préconfiguré de base (pas possible d'ajouter nos classe et nos id pour le css)?