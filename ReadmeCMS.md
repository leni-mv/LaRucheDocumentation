# Test CMS monsitevert

Tests du CMS monsitevert et rédaction d'une documentation.

# Dashboard documentation

## Pages
Créer une nouvelle page ou modifier une page existante.

### Premier menu en haut à droite (vert)

- Sauvegarder (la page)
- Retour (au dashboard avec toutes les pages)
- Icône de paramètre permet de modifier les paramètres généraux de la page (SEO, description, ect). Quand sa fenêtre est ouverte un icône poubelle permet de supprimer la page.


### Espace de travail à droite, menu :
- Gestionnaire de blocks permet d'ajouter les blocks avec un système de drag and drop et quelques otpions supplémentaires (ajout de texte et de formulaire par exemple. Notes :
    - Composant > Option permet de placer une petite image liée à un petit texte
    - Forms : La plupart des éléments de cette section ont besoin du block Form pour être intégré à la page.
- Gestionnaire de calques ou architecture sémantique de la page : Permet de voir la hiérarchie des éléments dans le corps de page et de les pointer avec plus de précision en cliquant dessus. (Pratique pour les lignes dans des blocs ou les HR)
- Pinceaux/Gestionnaire de style permet une stylisation rapide du block par rapport à sa position, sa taille et des paramètres de font.
- Icône paramètres pour voir les paramètres en code (type de balise, id du block, etc). Ces paramètres changent selon le bloc (c'est ici qu'on mets les pages de liens des blocs "lien" par exemple).
- Open code: permet de modifier en code le bloc (avec html et css). On peut ajouter, modifier du texte, etc. Le css s'ajouté avec la propriété style dans la balise html est séparé dans un block css à part à l'enregistrement. Ensuite en sauvegardant un id est automatiquement généré pour ranger le css dans la section correspondante. Si on ne click pas sur "Sauvegarder" (en haut du bloc html et css) le code ajouté est perdue.

### Menu de l'espace de travail permettant de visualiser la page et ajouter des éléments
- Permet grâce à des bordures dashed
- oeil permet de prévisualiser. Pour retourner en arrière un petit oeil noir très discret (en haut à gauche de l'écran) permet de revenir à l'espace de création de page.


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

- Image d'accueil mettre par dessus "La Ruche" avec effet d'ombrage pour que le texte se voit.
- Coller map au texte (il y a un bloc texte et image, si on peut mettre map dedans ce serait trop parfait !!)
- Entre la map et le bien vivre bien travailler mettre 3-4 emplacements images pour les photos des lieux
- Coller pointes images bien vivre bien travailler : les redimensionner ppour qu'elles prenent 50% de l'espace (css width 100% du block ou canva). Voir pour modifier taille de l'image.
- Média queries pour rendre responsive cette partie et la partie map si besoin;

- Voir comment intégrer des petits symboles pour styliser
- On ne peut pas ajouter un block sur une image (prévue comme image de fond). Besoin d'aller dans le code pour en faire une image background. Je test comme ça mais pas sûr que ça marche oo


## Questions et remarques

- Liens :
    - Où est-ce qu'on obtiens les liens de pages (si il s'agit bien d'une demande de lien de page) pour les mettre dans les thèmes du site par exemple ?
    - Est-ce que dans Pages > Paramètre de page c'est le nom ou le slug de la page qu'on utilise ?

- Dans paramètre > SEO :
    - Qu'est-ce que index, follow, noindex, nofollow ?
    - L'image mise en avant apparait dans le navigateur de recherche ?
    - Qu'est-ce que Id+json ?


- qu'est-ce que les classes "hero-section" et "hero-content" (vous avez une documentation concernant vos classes ?)

- Dans page > basique qu'est-ce que :
    - tooltip
    - Accordéon ? (genre de dropdown ?)
    - tabs (j'ai pas compris comment ça s'utilise)
    - Pop-up : on la lie à un bouton ou à une page pour qu'elle se déclenche ?
    - Lien (question posée plus haut) comment lier les pages entre elles ?
    - La différence entre conteneur et block
- Après basic > grille :
    - Conteneur + 2colonnes : je ne trouves pas les colonnes en passant la souris et elles n'aparaissent pas dans le corps
    - Quand j'ajoute d'autres éléments ils apparaissent dans le corps mais quand je passe la souris je n'ai que le bloque mère
    - Qu'est-ce que "cellule"
- After > Extra :
    - comment s'utilise le Countdown ? C'est un compteur automatique ?)
    - Custom Code c'est la même chose que dans l'icône code (on ne mets que du html/css, ou on peut faire autre chose ? Et je n'arrive pas à l'utiliser)

- Parfois le block devient une ligne (par quel processus ? Utilisation de flexboxs ?), comportement différent d'un bloc : rajoute de la marge sur la vue en desktop entre 2 colonnes. Pour sections "bien vivre et bien travailler" j'ai dû mettre le fond sur la ligne plutôt que sur la colonne pour qu'il n'y ai pas de marge entre la couleur et la photo.


- Remarque : quand on cherche dans le code (un id par exemple) ce serait pratique d'avoir un genre de Ctrl + f pour trouver les id (et classe) rapidement.

- Je n'arrive pas à mettre un block par dessus une image que je voulais en fond (La Ruche en acceuil et le formulaire de contact sur page contact *-*)

- l'outil code du panneau d'outils à droite ne garde pas en affichage la média query codée sur l'élément, il faut les chercher dans le fichier code source de la page. Pas très pratique pour vérifier et modifier/adapter le code. (media query only screen c'est les miens)

- Sur contact button "envoyer", comment s'assurer que ça marche ?