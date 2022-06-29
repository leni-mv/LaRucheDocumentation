# Test CMS monsitevert

Tests du CMS monsitevert et rédaction d'une documentation. Son fonctionnement s'appuie sur la doc du site GrapesJS.


# Dashboard documentation

## Pages
Créer une nouvelle page ou modifier une page existante. La plus grosse partie de cette documentation !
Note : Fontawesome est pré-intégré, on peut donc intégré nos liens dans les pages directement.

Raccourcis utiles avant de regarder les menus :
- En maintenant Ctrl on peut selectionner plusieurs blocs pour les modifier ensemble.

### Premier menu en haut à droite (vert)

- Sauvegarder (la page)
- Retour (au dashboard avec visuel de toutes les pages)
- Icône de paramètre permet de modifier les paramètres généraux de la page (SEO, description, ect). Quand sa fenêtre est ouverte un icône poubelle permet de supprimer la page.


### Espace de travail à droite > menu :
- Gestionnaire de blocks permet d'ajouter les blocks avec un système de drag and drop et quelques otpions supplémentaires (ajout de texte et de formulaire par exemple. Notes :

|Basique       |       |       |       |       |
|---    |:-:    |:-:    |:-:    |--:    |
|   Nom |   Description    |  Détails     |
|   Flexbox    |   Permet d'ajouter deux colonne dans un block    |   En passant la souris dessus on à accés à l'outil "dupliquer" pour rajouter autant de colonnes que souhaité. En mode mobile les colonnes s'alignent à la verticale.    |
|   Slider   |   Ajoute un carroussel de 3images qui prends toute la largeur du bloc ou de la page.    |       |
|   Accordéon    |   Tableau horizontal d'éléments ouvrant chacuns sur du contenu    |   En cliquant sur un Accordéons on peut modifier son titre et son contenu ouvert.    |
|   Tooltip    |   Petit block    |       |
|   Tabs    |   Comme Accordéon en mode menu    |    En cliquant sur un Tabs on peut modifier son titre et son contenu ouvert.    |
|   Pop-up    |   Pop_up qui se déclanche à partir du bloque ou de la page sur laquelle elle a été posée.  |     L'outil qui ressemble à un chéquier quand on selectionne ce block permet d'ajouter le texte qu'elle affichera.    |
|   Texte    |   Insère du texte    |       |
|   Image    |   Insère une image    |   A l'insertion du block une fenêtre nous permet de déposer ou d'ajouter l'url d'images et d'en choisir une pour le block. En sélectionnant l'image dans la page, la barre d'outil du block affiche un crayon : outil de modification de l'image.     |
|   Lien    |   Créer un lien dans la page    |   On paramètre les liens dans l'onglet de paramètre. Pour ajouter une page ou un article en lien on prends son slug (dans les paramètres globaux de la page visée) et on l'ajoute au chemin du lien en paramètres.    |
|   Bloc    |   Conteneur sans marge pour organiser les sections de la page.    |   Aucunes marges    |
|   Séparateur    |    HR   |       |
|   Liste    |   Liste à puce    |       |
|   Liste numérotée   |   Liste partant de 1   |       |
|   Code Court    |    Insert des éléments dans la page à partir de balises html   |   Si appliqué sur le body efface le contenu de la page, attention!   |
|   Conteneur    |    Block avec marges externes.   |      |
|   Vidéo    |   Insère une vidéo    |   Lien de la vidéo à mettre en paramètre.    |
|   Carte    |   Permet d'afficher adresse(entreprise par exemple) sur une carte.    |    Dans paramètres on peut entrer l'adresse souhaitée pour que la map s'adapte.   |
|       |       |       |
|       |    **Composants**   |       |
|   Section Hero    |   Comme un block.    |       |
|       |       |       |

|       |   BETA - Bloc réutilisables    |       |
|    ---   |   ---    |    ---   |
|   Blocks    |   Block(s) créé par l'administrateur lors de la création d'une page    |   Barre d'outil quand on selectionne un bloque > disquette > Fenêtre pour confirmer l'enregistrement du block    |


|      |   **Forms**    |       |
|    ---   |   ---    |    ---   |
|   Form    |   Permet l'insertion de la plupart des blocks de cette section dans une page.    |    Affiche une structure de blocks par défaut qu'il est possible de modifier à sa convenance.   |
|   Input    |   input lié à un label (cf plus bas)    |   Liaison se fait dans les paramètres    |
|   Textarea    |       |       |
|   Select    |       |       |
|   Button    |   Boutton d'envoi (send/submit) ou d'annulation(reset)   |    Son type se défini dans les paramètres   |
|   Label    |   Label à lier à un input    |   Liaison se fait dans les paramètres    |
|   Checkbox    |   Checkbox qu'on peut lier à un label en paramètre    |       |
|   Radio    |   Boutton radio qu'on peut lier à un label en paramètre    |       |
| | |

|       |   Extras    |       |
|   ---    |   ---    |  ---     |
|   Custom Code    |   Permet l'ajout d'élément via des balises html    |    Si utilisé sur la balise body efface tout le contenu de la page.   |
|   Countdown    |    Ajoute un compteur Jours, heures, minutes.   |   Pour que le compteur se lance la date de fin se note dans les paramètres.    |
|       |       |       |

Notes :
- Forms : dans Dashboard > Paramètre > Formulaire de contact on intègre l'email qui reçoit les demandes. Ensuite dans les paramètres de notre formulaire on choisi la méthode et on intègre ce lien en action **/form/submit?redirectTo=/index**.

- Gestionnaire de calques ou architecture sémantique de la page : Permet de voir la hiérarchie des éléments dans le corps de page et de les pointer avec plus de précision en cliquant dessus. (Pratique pour les lignes dans des blocks ou les HR)

- Pinceaux/Gestionnaire de style permet une stylisation rapide du block par rapport à sa position, sa taille et des paramètres de font.

- Icône paramètres pour voir les paramètres en code (type de balise, id du block, etc). Ces paramètres changent selon le bloc (c'est ici qu'on mets les pages de liens des blocs "lien" par exemple).

- Open code: permet de modifier en code le bloc (avec html et css). On peut ajouter, modifier du texte, etc. Le css s'ajouté avec la propriété style dans la balise html est séparé dans un block css à part à l'enregistrement. Ensuite en sauvegardant un id est automatiquement généré pour ranger le css dans la section correspondante. Si on ne click pas sur "Sauvegarder" (en haut du bloc html et css) le code ajouté sera perdue en changeant de section(block dans la page ou panneau d'outil).

### Menu de l'espace de travail permettant de visualiser la page et ajouter des éléments
- Carré "Voir les composant" permet grâce à des bordures dashed de voir l'espace de chaque block.
- oeil "Prévisualisation" permet de prévisualiser. Pour retourner en arrière un petit oeil noir très discret (en haut à gauche de l'écran) permet de revenir à l'espace de création de page.
- La quadruple flèche mets l'espace de travail en pleine écran.
- </> "Voir le code" donne accés à tout le HTML et CSS de la page. Possible de faire un Ctrl + F dessus pour chercher les éléments. (pratique pour les id généré automatiquement ou les média queries le temps que le beugue pour l'autre outil de code soit résolu).
- Les fléches permettent de retourner en arrière ou en avant comme un Ctrl + z ou Ctrl + y.
- La flèche vers le bas permet d'importer du code. Attention efface tout le contenu de la page à son profit une fois importé. Cas d'utilisation pour les page qui ont besoin d'être coder ou modifiée via un éditeur de code et remplacée par le code mis à jour par exemple.
- Poubelle efface le contenu de la page. Une pop-up de confirmation apparait avant suppression.

### Menu de l'espace de travail à gauche permettant de gérer le responsive :

Permet de travailler le responsive sur 3 tailles d'écran différent.
- Ordinateur : mode par défaut de l'espace de travail. Ce qui est fait sur les pages en mode Desktop s'applique à la tablette et au mobile
- Tablette : Réduit l'écran en mode tablette. Ce qui est fait sur la page en mode tablette s'applique au mobile mais pas au desktop.
- Mobile : permet de visualiser la page avec la largeur d'un téléphone. Ce qui est fait sur la page en mode mobile ne s'applique qu'au mobile.


## Articles

Permet d'ajouter des éléments comme des articles, des produits, des projets clients, etc et de les ranger dans des catégories. Ensuite grâce aux catégories il sera possible de générer une page qui n'affiche que les articles affilié à telle ou telle catégorie.

Créer un article : affiche une page qui reprend le code de la page d'accueil.
Créer une catégories (remplir les champs). Maintenant il est possible d'ajouter cette catégorie aux articles juste en modifiant les paramètres globaux dans l'espace de travail pour modifier l'article.

Note : Il est possible d'affilier à plusieurs catégories un article.

## Catégories

Permet de créer des catégories pour les articles ce qui permettra ensuite de filtrer les articles par catégorie sur le site.

## Menus
- Les liens de pages sont créer avec le slug ou /nomDeLaPage dans la création de page en paramètre et dans la création de menu en paramètre des lien qu'on ajoute à nos menus

## Thème
Permet de créer l'ambiance graphique du site. On ne peut pas créer un thème, seulement modifier celui créer par monsitevert pour nous.
- Entête : permet de donner le titre en logo du site et de lui passer un slug pour qu'il retourne une page (note: est prévu de lui passer une page sinon error 404 si l'utilisateur click dessus).
- Bas de page : permet d'ajouter du texte et du texte de copyright dans le footer.
- La section "Style" donne une couleur principal et une couleur de contraste pour les éléments principaux et secondaires du site, le header, le footer, les pages, les articles ainsi que la police et la taille d'écriture par défaut des titres et textes du site.
- "Code personalisé : Permet d'ajouter du code à la fin de la balise head pour le navigateur et à la fin de la balise body pour les pages.

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

## Données des formulaires
Pour le moment permet de visualiser les test sur l'envoi de formulaires. Sera peut-être amené à changer avec la mise en place de formulaires multiples.

## Redirections (section à détailler)
Permet de visualiser les redirections.

## Analytics (version beta)
Donne un outils d'analyse des performance du site et des comportements utilisateurs dessus.

## Audit (version beta)
Permet d'évaluer si notre site est responsable energétiquement avec un classement energétique partant de A pour les meilleurs.

## Aide et support

Permet d'envoyer un message (à Fred) aux dév qui s'occupe de la conception de monsitevert pour répondre à nos questions et résoudre nos problèmes.

## Prévisualisation

Permet de prévisualiser tout le site en situation réelle (contrairement à l'outil de prévisualistaion de page). Pour le moment il faut relancer la prévisualisation à chaque modification pour qu'elle soit prise en compte.

## Publier

Permet de publier le site.

## Utilisateurs
Information de compte de l'administrateur.
On peut éditer ou supprimer le compte avec le crayon ou la poubelle dans la colonne "Action".

## Mon compte
Permet de changer les informations de compte (nom, mail, mdp).

# Travail perso et questions pour mieux comprendre le CMS

## To do

- re-trouver comment mettre titre site dans entête thème (rapport avec le logo de mémoire)


## Questions et remarques

- Beug pris en compte: l'outil code du panneau d'outils à droite ne garde pas en affichage la média query codée sur l'élément.

- Comment créer une bordure sur le texte et non sur le block de texte sans passer par le code ?
**Réponse** : Typographie, ombre de texte créer un calque et c'est partie !

- Block > Extras > CustomCode : efface aussi entête et pied de page défini en Thème ? Ou seulement le body ?

- Remarque : Création de page > Gestionnaire de style > Décoration > Calque : le premier calque a par défaut moins de paramètres que le deuxième qu'on ajoute.

- Remarque : les conteneurs ont une marge supérieur négative (manque 9px en ordi et tablette et 8px en mobile) et déborde sur les autres éléments.

- thème en-tête secondaire la couleur secondaire ne change pas quand on modifie le rgb oo'

- Remarque : les nom de champs de couleurs pour theme ne sont pas très clair, on ne sait pas exactement si ça va coloré des  blocks, des titres, des noms de champs(label ou input par exempl), ect.

- Comment changer la couleur d'un élément en classe active dans le menu défini en theme ?

- A partir d'un boutton dans la page (Nous contacter par exemple) comment créer des liens vers d'autres pages ?

- Peut-on rendre "hidden" un élément sans toucher au code ?

- Remarque : Block flexbox : les marges entre deux éléments ou deux flexboxs se décallent et ont besoin d'être bidouillée pour que ce soit droit (y compris en mode tablette)

- Thème :
    - Entête : "button - texte" et "button - lien" on est censé mettre le titre de site et la page vers laquelle il renvoit ? Ou c'est autre chose ?
    - Entête couleurs : De "couleur principal" à "Entête - couleur de contraste" aucune couleur ne permet de changer le noir par défaut quand on est sur une page. 

- Prévisualisation : rafraichir la page ne permet pas de mettre à jour les modification il faut relancer la prévisualisation à chaque modification (pour travailler sur header et footer pas pratique)

- pour les lien entre les pages, si ils ne sont pas définie dans le menu je n'arrive pas à les connecter aux pages avec "/NomDeLaPage". J'arrive sur la page erreur 404 directement.

- Pop-up : est-il possible de la déclencher en cliquant sur un boutton par exemple ou elle se déclenche forçément à l'ouvertur de la page ?

- Articles, même pb que pour les liens : comment les relier à un bloque d'une page. Pas de menu dédié pour les articles.

- Page > Article1 : Le bloc de lien et image ne se plie pas a la border radius de son bloc parent (le bloc de colonne).

- Si l'on souhaite un effet d'animation (hover par exemple) il faut le rajouter dans la partie code du CSS.

- Remarque : surplux de marge à droite : beug du block container

- Peut-on retiré la marge par défaut pour tablette et mobile (car même en mettant tout à 0 une marge subsiste sur ces deux templates)

- Remarques : Image > Crayon de modification > Menu en haut > historique : On a pas l'historique de modifications (qui serait très utile pour retourner en arrière) mais seulement un dossier load.