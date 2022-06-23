# Test CMS monsitevert

Tests du CMS monsitevert et rédaction d'une documentation. Son fonctionnement s'appuie sur la doc du site GrapesJS.

# Dashboard documentation

## Pages
Créer une nouvelle page ou modifier une page existante. Fontawesome est pré-intégré.

### Premier menu en haut à droite (vert)

- Sauvegarder (la page)
- Retour (au dashboard avec toutes les pages)
- Icône de paramètre permet de modifier les paramètres généraux de la page (SEO, description, ect). Quand sa fenêtre est ouverte un icône poubelle permet de supprimer la page.


### Espace de travail à droite, menu :
- Gestionnaire de blocks permet d'ajouter les blocks avec un système de drag and drop et quelques otpions supplémentaires (ajout de texte et de formulaire par exemple. Notes :
    - Basique : pop-up ce déclenche à partir du block ou de la page où elle est posée. L'outil qui ressemble à un chéquier quand on passe la souris dessus permet d'ajouter le texte qu'elle affichera.
    - Composant > Option permet de placer une petite image liée à un petit texte
    - Forms : La plupart des éléments de cette section ont besoin du block Form pour être intégré à la page. Dans Dashboard > Paramètre > Formulaire de contact on intègre l'email qui reçoit les demandes. Ensuite dans les paramètres de notre formulaire on choisi la méthode et on intègre ce lien en action **/form/submit?redirectTo=/index**.
    - Extra :
        - Countdown : le compteur peut-être mis en place via l'icône de paramètre des blocks.
        - CustomCode : si appliquée sur le body efface la page au profit du nouveau code.

- Gestionnaire de calques ou architecture sémantique de la page : Permet de voir la hiérarchie des éléments dans le corps de page et de les pointer avec plus de précision en cliquant dessus. (Pratique pour les lignes dans des blocs ou les HR)

- Pinceaux/Gestionnaire de style permet une stylisation rapide du block par rapport à sa position, sa taille et des paramètres de font.

- Icône paramètres pour voir les paramètres en code (type de balise, id du block, etc). Ces paramètres changent selon le bloc (c'est ici qu'on mets les pages de liens des blocs "lien" par exemple).

- Open code: permet de modifier en code le bloc (avec html et css). On peut ajouter, modifier du texte, etc. Le css s'ajouté avec la propriété style dans la balise html est séparé dans un block css à part à l'enregistrement. Ensuite en sauvegardant un id est automatiquement généré pour ranger le css dans la section correspondante. Si on ne click pas sur "Sauvegarder" (en haut du bloc html et css) le code ajouté sera perdue en changeant de section(block dans la page ou panneau d'outil).

### Menu de l'espace de travail permettant de visualiser la page et ajouter des éléments
- Permet grâce à des bordures dashed
- oeil permet de prévisualiser. Pour retourner en arrière un petit oeil noir très discret (en haut à gauche de l'écran) permet de revenir à l'espace de création de page.


## Articles
## Catégories
## Menus
- Les liens de pages sont créer avec le slug ou /nomDeLaPage dans la création de page en paramètre et dans la création de menu en paramètre des lien qu'on ajoute à nos menus

## Thème
Permet de configurer la vue du header et du footer ainsi que l'ammbiance graphique du site. On ne peut pas créer un thème, seulement modifier celui créer par monsitevert pour nous.

## Paramètres
Dans cette section il est possible de prédéfinir plusieurs comportements via les sections suivantes :

### Global
- Titre, url, logo et favicon du site ainsi que 2 checkbox pour confirmer que le site n'utilise pas de cookies et afficher "mon site vert".
### Optimization des assets
- Compression des images jpeg, png et gif ainsi qu'une checkbox pour tester la version BETA de compression de tous les formats d'image.
### SEO
- Permet de choisir la langue, le comportement du robot, de nouveau l'URL du site, lien page 404 (à créer dans pages) avec son titre et sa description, lien utilisateur Twitter, image mise en avant et Id+json
### Formulaire de contact
- adresse email reçevant les demandes de contact et options de reCAPTCHA. Cette section sera changée pour être adaptée à plusieurs formulaires. 

# Travail perso et questions pour mieux comprendre le CMS

## To do

- Média queries pour rendre responsive cette partie et la partie map si besoin
- re-trouver comment mettre titre site dans entête thème (rapport avec le logo de mémoire)
- Page > Contact : faire wrapper, déplacer les input sous les labels (là c'est moche)


## Questions et remarques

- Beug pris en compte: l'outil code du panneau d'outils à droite ne garde pas en affichage la média query codée sur l'élément.

- Comment créer une bordure sur le texte et non sur le block de texte sans passer par le code ?

- Block > Extras > CustomCode : efface aussi entête et pied de page défini en Thème ? Ou seulement le body ?

- Remarque : Création de page > Gestionnaire de style > Décoration > Calque : le premier calque a par défaut moins de paramètres que le deuxième qu'on ajoute.

- Remarque : les conteneurs ont une marge supérieur négative (manque 9px en ordi et tablette et 8px en mobile) et déborde sur les autres éléments.

- thème en-tête secondaire la couleur secondaire ne change pas quand on modifie le rgb oo'

- Remarque : les nom de champs de couleurs pour theme ne sont pas très clair, on ne sait pas exactement si ça va coloré des blocs, des titres, des noms de champs(label ou input par exempl), ect.

- Comment changer la couleur d'un élément en classe active dans le menu défini en theme ?

- A partir d'un boutton dans la page (Nous contacter par exemple) comment créer des liens vers d'autres pages ?

- Peut-on rendre "hidden" un élément sans toucher au code ?

- Remarque : Bloc flexbox : les marges entre deux éléments ou deux flexboxs se décallent et ont besoin d'être bidouillée pour que ce soit droit (y compris en mode tablette)