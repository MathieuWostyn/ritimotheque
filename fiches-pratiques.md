---
description: Version provisoire  (en cours de rédaction)
---

# Fiches pratiques PMB

## La recherche dans le catalogue public PMB (côté OPAC)

Il y a deux accès pour la recherche dans PMB : un accès en mode gestion, un accès public (objet de cette fiche pratique).

La fenêtre de recherche PMB (accès public) n’a pas tout à fait les mêmes fonctions que la recherche en mode gestion.

### **1. Accéder à PMB**

A partir du site ritimo.org, dans la "boussole" en haut de la page d’accueil, cliquez sur le bouton «_Ritimothèque_ ».

Vous arrivez directement sur la page de recherche de PMB.

![](<.gitbook/assets/image (30).png>)

Par défaut, vous êtes dans l’onglet « recherche simple » qui vous permet de sélectionner :

* le type de document recherché (menu déroulant)
* le site (localisation d’un membre **ritimo**) (menu déroulant)
* un terme (ligne blanche)
* un filtre (cases à cocher, par défaut recherche sur tous les champs)

**Les champs de la notice qui sont inclus dans la recherche « Tous les champs » sont :**

* Titres
* Auteurs
* Notes et résumé
* Indexation (les descripteurs sont appelés « catégories » dans PMB)

### **2. Comment chercher ?**

{% hint style="info" %}
Les ponctuations sont ignorées lors de la recherche (cela équivaut à les remplacer par un espace), sauf si l'expression cherchée est placée entre guillemets.
{% endhint %}

#### **Expression booléenne**

Une **expression booléenne** qualifie une opération utilisant les opérateurs de l'algèbre de Boole: ET, OU, SAUF, etc.

* L'opérateur **OU** est représenté par un espace. C’est l’opérateur de PMB par défaut.
* L'opérateur **ET** est représenté par le plus (+)
* L'opérateur **SAUF** est représenté par un tiret (-).

**Opérateur OU**

Dans PMB, l'opérateur utilisé par défaut est le OU. Si vous cherchez deux mots séparés par un espace, la réponse donnera d'abord les résultats qui contiennent les deux termes à la fois, puis l'un OU l'autre.

Pour une recherche : _décroissance latouche_

* les notices contenant décroissance et latouche feront partie des premières réponses
* les notices contenant décroissance (seul) ou Latouche (seul) feront partie des réponses qui s’afficheront ensuite.

**Opérateur ET : +**

Pour une recherche : _décroissance + latouche_

* les notices contenant décroissance (seul) ou Latouche (seul) ne feront pas partie des réponses
* les notices contenant décroissance et latouche feront partie des réponses, même si Latouche n’est pas auteur (s’il est cité dans le résumé)

**Opérateur SAUF : -**

Pour une recherche : _décroissance - latouche_

* les notices contenant décroissance et latouche ne feront pas partie des réponses
* les notices contenant latouche ne feront pas partie des réponses

#### Troncature

La troncature permet de rechercher des termes qui ont une racine identique en substituant un ou plusieurs caractères par un symbole. Dans PMB, ce symbole est l'astérisque (\*). Elle est activée par défaut.

Elle permet de remplacer un ou plusieurs caractères dans l'expression recherchée :

* **enfant\*** cherchera les termes Enfant, Enfant des rues, Enfant soldat...
* **\*enfant** cherchera Enfant, Droit de l'enfant

#### Guillemets

Dans une recherche, une suite de caractères entre guillemets permet de chercher la suite de caractères telle que saisie (mais sans tenir compte des accents ou des majuscules).

Chercher "détruisent la planète" (avec les guillemets) donnera la réponse :

![](<.gitbook/assets/image (10).png>)

**Cas du tiret**

Il ne faut pas confondre le **trait d'union** avec l'**opérateur SAUF** : le même signe, le "-" est utilisé pour les deux.

\-L'opérateur SAUF est toujours précédé d'un espace « -»

\-Le tiret est collé au mot qui le précède «-»

* Royaume-Uni renvoie les résultats contenant Royaume Uni et Royaume-Uni.
* Royaume -Uni renvoie les résultats contenant Royaume sauf ceux contenant Uni.

**Parenthèses**

Les parenthèses permettent de regrouper différents mots dans les recherches et de changer l'ordre dans lequel les opérateurs seront pris en compte. Elle permettent d’éviter le « bruit » (=trop de réponses non pertinentes).

eau + (Israël Palestine) renverra les résultats contenant

* eau ET Israël
* eau ET Palestine
* eau ET Israël ET Palestine

eau + Israël Palestine renverra les résultats contenant

* eau ET Israël
* eau ET Palestine
* eau ET Israël ET Palestine
* Palestine
* Israël

**Mots vides**

Un mot vide est un mot qui n'est pas porteur d"information. Il ne sera pas pris en compte lors d'une recherche.

Par défaut dans PMB, certains mots sont déjà déclarés vides en fonction de la langue. Pour le français ce sont : le, la, les, l', du, de, des, d', a, un, une, et, t, au, aux, en.

Les mots vides sont systématiquement ignorés des recherches sauf lorsqu'ils sont placés entre guillemets. Lors d'une recherche sur une autorité (auteurs, éditeurs...), les mots-vides ne sont pas ignorés.

**Surligneur**

On peut surligner les mots cherchés grâce à l’outil représenté par l'icone :

<div align="left">

<img src=".gitbook/assets/image (23).png" alt="">

</div>

### 3. Les réponses

#### **L’affichage des réponses**

![](<.gitbook/assets/image (20).png>)

* **L’icône du type de document** : les types de documents sont représentés par des symboles :
  * vidéo
  * article imprimé
  * document électronique
  * document imprimé
  * exposition
  * etc.
* **Déplier / replier une notice**
  * pour accéder à l’affichage long (entier) de la notice
  * revient à l’affichage court de la notice (titre et collation)

#### Tri par défaut des réponses

:point\_right: Par défaut, le titre est **surpondéré** dans la recherche tous champs.

Ensuite, PMB effectue par défaut un **Tri des réponses :** il affiche les réponses par ordre :

1. de pertinence (+ de mots recherchés en premier)
2. de date de publication (ordre chronologique inversé)
3. « commence par »
4. alphabétique de titre.

Si on cherche décroissance dans les titres et tous les champs, on obtiendra :

* En premier, les titres qui commencent par le mot « décroissance » (ex : Décroissance ou barbarie)
* Ensuite les titres qui contiennent le mot « décroissance » plus loin (ex : Petit traité de la décroissance sereine)
* En dernier les notices qui contiennent le descripteur (catégorie) décroissance.

S’il y a moins de 1000 réponses, on peut choisir un autre tri des réponses (voir ci-dessous). Dans ce cas, le tri créé s’applique sur la session.

**Trier les réponses selon d’autres critères**

Le tri des résultats d'une recherche consiste en un ré-ordonnancement des résultats obtenus.

Pour trier les résultats d'une recherche, cliquer sur l'icône après avoir affiché les résultats.

Exemple pour trier les résultats par ordre de publication décroissant :

En reprenant le résultat de recherche sur « décroissant » (167 titres trouvés pour la recherche 'décroissance')

![](<.gitbook/assets/image (2).png>)

Pour trier la recherche par ordre chronologique décroissant, il faut définir un nouveau tri :

* Sélectionner « année d’édition »
* Sélectionner « décroissant »
* « Enregistrer et appliquer le tri »

PMB affiche les documents publiés plus récemment en premier.

#### Affiner la recherche

Cette fonction permet d’ajouter un critère (ou plus) de recherche. Elle s’applique à la recherche en cours.

Exemple pour affiner les résultats en ajoutant un critère sur la localisation :

* Choisir le champ « Localisation » (attention il ne donne pas les réponses pour les articles et bulletins de périodiques)
* Sélectionner dans la liste « CDTM Montpellier »
* Valider en cliquant sur « Rechercher »

#### Utiliser les filtres sur l'ensemble des réponses

* Sous la fenêtre de recherche, cliquer sur « Voir toutes les notices » pour faire apparaitre les filtres dans la marge de droite
* Choisir le(s) filtre à appliquer en cochant la(es) cases correspondantes
* les filtres disponibles :
  * date de publication
  * type d'outil
  * type de document
  * public cible
  * type de contenu
* cliquer sur le bouton "filtrer" pour appliquer le filtre sur les réponses à la question posée

#### Utiliser le panier

L'icône **panier** permet de récupérer chaque notice dans un panier. Après avoir constitué un panier, vous pouvez :

* Sélectionner les notices
  * Vous devez sélectionner les notices une par une
  * Le panier s’affiche en haut de l’écran en précisant le nombre de notices qu’il contient
* Imprimer les notices (tout le panier ou les notices cochées) :
  * Pour afficher le contenu du panier, cliquer sur l’expression « Votre panier contient x notice(s) »
  * Pour imprimer le contenu du panier, cliquer sur le bouton « imprimer »
    * Imprimer : choisir « tout le panier » ou « les notices cochées »
    * Type d’affichage des notices : « ISBD » (description bibliographique internationale normalisée) ou « PUBLIC » (voir les exemples plus bas)
    * Format des notices : choisir « format court » ou « format long »
    * Imprimer l’entête de notice : fera apparaître le titre en gras au-dessus de la notice
    * Informations exemplaires : vous pouvez choisir d’imprimer ou pas les exemplaires attachés à une notice (permet de voir les cotes et les localisations)
    * Format de sortie : privilégier « traitement de texte » qui ouvrira une nouvelle fenêtre à enregistrer.
    * Valider vos choix en cliquant sur « imprimer ».
* Vider le panier

#### **Exemples d’impression**

**L’impression de type « ISBD » Format court**

![](<.gitbook/assets/image (13).png>)

**L’impression de type « ISBD » Format long**

![](<.gitbook/assets/image (26).png>)

#### L’impression de type « PUBLIC » Format court

![](<.gitbook/assets/image (42).png>)

**L’impression de type « PUBLIC » Format long**

![](<.gitbook/assets/image (46).png>)

### 4. Trier les notices : appliquer un tri sur des résultats de recherche ou un panier

Il est possible de trier les notices composant un résultat de recherche ou également les notices contenues dans un panier. Le tri n’est pas autorisé lorsque le résultat de la recherche ou le panier contient plus de 1000 notices.

#### 1. Exemple de tri sur le contenu d’un panier, par type de document

```
Onglet Catalogue > Paniers > Gestion
```

* Sélectionner un panier en cliquant sur son nom => il affiche le contenu du panier.
* Pour faire apparaître les options de gestion d’un panier, cliquer à nouveau sur le nom du panier qui s'affiche dans le cadre au-dessus de la liste des notices.
* Cliquer sur l'icône "a-z" pour faire apparaître la fenêtre des tris disponibles.
* Sélectionner le tri "Type de document" en cliquant sur son nom pour appliquer le tri au panier de notices => le tri appliqué est le suivant : d'abord les ouvrages et articles, puis les vidéos, les expos, les documents multimédia, les jeux et enfin les dossiers pédagogiques...

#### 2. Créer un nouveau tri

Les tris enregistrés sont utilisables pour des recherches ultérieures

* Cliquer sur Définir un nouveau tri
* Sélectionner le critère de tri puis double-cliquer pour le passer dans la colonne des critères de tri retenus.
* Il est possible d’appliquer plusieurs critères de tri successifs

Les flèches vertes de gauche permettent de modifier l’ordre des critères de tri les uns par rapport aux autres. Les flèches vertes du milieu permettent de choisir un tri croissant ou décroissant. Le bouton « A - Z / 0 - 9 » permet de choisir un tri alphanumérique ou numérique.

## Ajouter un exemplaire

Les exemplaires correspondent aux documents physiques présents dans les centres de documentation. Chaque exemplaire est lié à une notice. Que cela soit à la suite de la saisie d’une notice (dans ce cas, passer directement au point 2.) ou après avoir sélectionné un document dans le catalogue, il s’agit ici d’indiquer que vous avez un exemplaire du document.

### 1. Sélectionner le document pour ajouter votre exemplaire

```
Onglet Catalogue > recherche
```

* Saisir le titre du document dans la ligne prévue à cet effet
* Cliquer sur rechercher : La page de résultat s’affiche
* Cliquer sur le titre du document concerné : La notice et les exemplaires liés s’affichent :

![](<.gitbook/assets/image (4).png>)

### 2. Ajouter votre exemplaire

Pour ajouter votre exemplaire, vous avez deux possibilités :

* Utiliser le numéro unique attribué automatiquement par PMB (à éviter)
* Ajouter votre propre numéro d’exemplaire => méthode recommandée

#### 2.1. Utiliser le numéro unique attribué automatiquement par PMB

* La case « Génération automatique » doit être cochée
* Cliquer sur « Ajouter un exemplaire ». C’est un peu long car il va attribuer automatiquement un numéro d’exemplaire, il va chercher les numéros disponibles. Une nouvelle fenêtre s’ouvre :

![](<.gitbook/assets/image (52).png>)

Un numéro d’exemplaire a été attribué automatiquement. Ce numéro est unique et servira pour le prêt. Renseigner les champs de la manière suivante :

* **Cote** (obligatoire): Indiquer votre cote (inutile de mettre les initiales de votre centre)
* **Support** (obligatoire) : Sélectionner le format physique du document (par exemple, dvd pour une vidéo, livre pour un texte imprimé, etc).
* **Localisation** (obligatoire) : par défaut le nom de votre centre.
* **Section** (obligatoire) : préciser l’emplacement des exemplaires dans une localisation (par défaut : fonds principal).
* **Propriétaire** : préciser, le cas échéant, à qui appartient l’exemplaire (dans le cas d’un dépôt par une autre association, par exemple).
* **Statut** (obligatoire) : préciser si l’exemplaire est empruntable, en consultation sur place, etc.
* **Message exemplaire** : préciser si le document est endommagé.
* **Prix** : facultatif, permet de récupérer la somme en cas de perte.
* Puis Enregistrer pour finaliser l'opération.

:point\_right:N’oubliez pas de noter le numéro d’exemplaire à l’intérieur du document.

#### 2.2. Créer un numéro propre au centre (cela peut être le numéro d’inventaire du centre)

* La case « Génération automatique » doit être décochée
* Saisir le numéro d’exemplaire du centre **ATTENTION ! Comme ce numéro doit être unique, chaque centre doit faire précéder le numéro de ses initiales**.
* Cliquer sur « Ajouter un exemplaire ». La fenêtre de l’exemplaire s’ouvre, continuer, comme expliqué au point 2.1

### 3. Modifier votre exemplaire

Vous pouvez à tout moment modifier les informations concernant votre exemplaire.

![](<.gitbook/assets/image (27).png>)

A partir de cette ligne, il suffit de cliquer sur le No d’exemplaire pour ouvrir la fenêtre d’exemplaire et faire vos modifications.

### 4. Supprimer un exemplaire

La suppression des exemplaires perdus ou pilonnés est effectuée par l'administratrice de PMB.

* Mettre les exemplaires dans un panier intitulé, par exemple, "Exemplaires à supprimer, nom du centre"
* Envoyer la demande de suppression à NSamuel et lui indiquant le nom du panier.

## Le traitement des périodiques, bulletins et articles

Le catalogue Ritimothèque contient plus de 800 titres de périodiques.

La gestion des périodiques dans PMB permet notamment :

* d'indiquer l'état de vos collections (dans un onglet spécifique)
* d'utiliser le bulletinage automatique pour les périodiques que vous prêtez et auxquels vous souhaitez associer un exemplaire par numéro (ou bulletin).
* de connaître les gardiens des collections.

:point\_right:Rappel de la structure des données concernant les périodiques dans PMB : Chaque périodique fait l’objet d’une notice mère à laquelle sont rattachés les bulletins (chaque numéro du périodique). À chacun de ces bulletins peuvent se rattacher :

* Un ou plusieurs exemplaires
* Une ou plusieurs notices de dépouillement d’article

Chaque bulletin peut comporter une « notice de bulletin », qui lui est directement liée.

Le **bulletinage** consiste à enregistrer dans PMB les numéros de périodiques et de les exemplariser (indispensable pour pouvoir les prêter aux lecteur·rices avec la fonction prêt de PMB). L'intérêt du bulletinage est de faciliter la gestion des collections, de contrôler les numéros manquants et les fins d'abonnements.

Pour pouvoir effectuer le bulletinage, il est nécessaire d'avoir préalablement créé un abonnement.

### 1. Chercher la notice de revue à partir du nom de la revue

```
Onglet Catalogue > recherche > périodiques
```

![](<.gitbook/assets/image (48).png>)

* Inscrire un ou plusieurs mots du titre dans l'écran de recherche
* Cliquer sur rechercher
* Deux cas de figure :
*
  * La revue n’existe pas dans la base : il faut créer la notice mère.
  * La revue existe. Possibilité d’ajouter un bulletin, un exemplaire et éventuellement une ou plusieurs notices de dépouillement.

### 2. Créer la notice mère pour une nouvelle revue

```
Onglet Catalogue > Périodiques > Nouveau périodique
```

![](<.gitbook/assets/image (17).png>)

S'il s'agit d'une revue en ligne ou sur cédérom, choisir le type de notice qui convient (document électronique) puis  saisir la notice (en respectant les règles d’écritures et les champs obligatoires) :

* Titre
* Auteur (en général, c’est une collectivité – personne morale)
* Éditeur
* ISSN : cliquer sur le bouton, qui ouvre une nouvelle fenêtre
* Notes générales : rapide description de la revue.
* Catégories
* Langue
* URL associée (adresse Internet de la revue)
* Producteur de la notice
* Date de saisie
* Statut de la notice

### 3. Ajouter un bulletin

#### 3.1. Chercher la notice de revue à partir du nom de la revue

```
Onglet Catalogue > recherche > périodiques
```

* Cliquer sur le nom de la revue choisie : la notice de la revue s’affiche

![](<.gitbook/assets/image (19).png>)

A partir de cet écran, vous pouvez :

* modifier la notice de la revue (notice mère).
* supprimer la revue (attention : cette opération supprime tous les bulletins, notices et exemplaires rattachés à cette revue).
* remplacer la notice mère de la revue par une autre (utile en cas de doublons suite à la conversion : cette opération rattache tous les bulletins à une seule et même notice mère)

Plus bas, la liste des bulletins s'affiche dans l’onglet bulletin (à condition de sélectionner « toutes les localisations ») : Les onglets « **Abonnements** » et « **Modèles prévisionnels** » concernent le bulletinage automatique (pas encore activé). L'onglet « **état des collections** » permet d’indiquer, pour chaque localisation, l’état de sa collection.

![](<.gitbook/assets/image (5).png>)

Les paniers de la colonne de gauche permettent de mettre un bulletin, une notice de bulletin ou un ou plusieurs exemplaires de bulletins dans un panier, en fonction du type de panier choisi.

Les paniers de droite permettent de mettre dans un panier de notices les notices de dépouillement liées à un bulletin.

A partir de cet écran vous pouvez cliquer sur un bulletin pour le modifier, ajouter un exemplaire, visualiser les dépouillements d’articles liés au bulletin, en ajouter.

![](<.gitbook/assets/image (50).png>)

#### 3.2. Ajouter votre bulletin

* Cliquer sur le nom de la revue choisie : la notice de la revue s’affiche.
* Cliquer sur le bouton **Ajouter un numéro ou un bulletin** : la notice de bulletin s'affiche.

![](<.gitbook/assets/image (25).png>)

Saisir les informations :

* Numérotation : veiller à la conformité selon les règles d’écritures.
* Date de parution : toujours sous la forme jj/mm/aaaa. Exemple : pour un mensuel de janvier 2012, indiquer 01/01/2012. L'utilisation du calendrier intégré à PMB, facultative, permet de s'assurer que l'on utilise la graphie correcte.
* Libellé de période : attention, c’est le libellé qui s’affiche sur la liste des bulletins. Saisir sous les formes suivantes :
*
  * Pour un quotidien, un hebdomadaire, un bimensuel: jj/mm/aaa ;
  * Pour un mensuel, un trimestriel... : mm/aaaa
* Code commercial (inutile)
* Titre du bulletin : il est possible d'indiquer dans ce champ le titre d'un numéro spécial : son intitulé apparaît dans la liste des bulletins. Ce champ n'est obligatoire et interrogeable que si l'on veut créer une notice de bulletin.
* Autres champs : Les autres champs servent à créer une notice de bulletin, c'est-à-dire une notice concernant l'intégralité du numéro (respecter les règles d’écritures). Cette saisie est facultative ; elle peut servir à saisir un numéro thématique qui ne sera pas dépouillé article par article.

#### 3.3. Ajouter un exemplaire

Pour les revues comme pour les monographies il est possible d'ajouter son exemplaire. A partir du bulletin, il est possible d'ajouter directement un exemplaire.

![](<.gitbook/assets/image (1).png>)

Saisir le numéro d'exemplaire dans le champ n° exemplaire (ou le créer automatiquement en laissant l’option « génération automatique » cochée)  Cliquer sur le bouton ajouter un exemplaire.

#### 3.4 Ajouter un dépouillement

A partir du bulletin, il est possible d'ajouter une notice de dépouillement.

![](<.gitbook/assets/image (40).png>)

* Cliquer sur le bouton : Ajouter un dépouillement, un écran de saisie de notice s'ouvre
* Renseigner les champs, puis enregistrer.

### 4. Les fonctions PMB pour la gestion des périodiques

#### **L'onglet bulletin**

Le bulletin est un numéro du périodique. Chaque bulletin peut avoir zéro, un ou plusieurs exemplaires.

L'onglet bulletin permet d'accéder à l'affichage de l'ensemble des bulletins associés au périodique, il permet donc de consulter la liste des bulletins.

* **Numérotation** : numéro du bulletin.
* **Date de parution** : sert à trier les numéros par ordre chronologique.
* **Libellé de période** : intitulé de la période que couvre le numéro (souvent indiquée à côté du numéro). Exemple : semaine du 17 au 24 novembre 2015.
* **Titre** : Titre principal du numéro (celui que l'on retrouve sur la couverture).
* **Art** : nombres d'articles attachés au bulletin
* **Doc** : nombre de documents numériques attachés au bulletin
* **Expl** : nombre d'exemplaires attachés au bulletin.

#### **L'onglet** **abonnements**

Cet onglet donne accès à la procédure qui permet d'indiquer à PMB que vous recevez régulièrement un périodique afin de contrôler vos collections et mettre en place le bulletinage automatique.

\=> Règle à appliquer impérativement : démarrer votre abonnement en 2016, les exemplaires précédents peuvent être ajoutés à la main directement pour éviter les doublons et problèmes.

**=>** Cliquez sur **ajouter un abonnement**

* **Nom de l'abonnement** : indiquer le nom de votre choix (par exemple le nom de votre centre)
* **Liste des modèles** : sélectionner un modèle dans la liste proposée puis **Valider**
* **Date de début** : choisir la date de début dans l'année courante
* **Date de fin** : vous pouvez choisir une date de fin éloignée pour ne pas avoir à corriger chaque année cette indication.
* Cocher **`exemplarisation automatique`** permet de générer un numéro d'exemplaire automatiquement à la réception du périodique, en fonction du script de numérotation (de manière transparente).

Si l'exemplarisation automatique n'est pas activée dans l'abonnement, il faudra saisir un numéro d'exemplaire pour affecter un code-barres à chaque numéro reçu.

\= > **Attention lors de la saisie des informations ci-dessous : la moindre erreur va générer des doublons et désorganiser l'ensemble des bulletins** :

* **`numéro de départ`**` `` ``: ` permet de préciser le premier numéro de l'abonnement et de définir ainsi le calcul des numéros ultérieurs. Ce numéro doit impérativement être en adéquation avec le début de votre abonnement indiqué plus haut.
* **`Numéro de départ du volume`** : permet de préciser le premier numéro de volume de l'abonnement et de définir ainsi le calcul des numéros de volume ultérieurs.
* **`Numéro de départ du tome`** : permet de préciser le premier numéro de tome de l'abonnement et de définir ainsi le calcul des numéros de tome ultérieurs. (Non activé dans le modèle présenté en exemple donc non visible dans la capture).
* **`Délai avant retard`** : délai à partir duquel les numéros non reçus sont considérés en alerte.
* **`Délai critique`** : délai à partir duquel les numéros non reçus sont considérés en alerte critique.

Une fois tous les paramètres définis, cliquer sur **`Générer la grille`** pour afficher le calendrier des jours de réception des numéros de périodique.

* **Re-générer la grille** : En re-générant la grille des numéros à recevoir, PMB recalcule tous les numéros étant à recevoir. Si vous avez déjà enregistré la réception de numéros correspondants à l'abonnement, ces numéros vont apparaître comme étant de nouveau à recevoir.

#### **L'onglet** **modèles prévisionnels**

* Le modèle prévisionnel permet de définir la périodicité des numéros du périodique sur les années à venir, en dehors de toute considération d'abonnement.
* Les différents cahiers du périodique doivent être définis ici, sous la forme d'un modèle par cahier.

\=> Décision de la commission PMB : les utilisateurs ne sont plus autorisés à créer les modèles prévisionnels. Cette fonction est maintenant centralisée dans le réseau car il y a trop d'erreurs.

#### **L'onglet** **état des collections**

Permet de montrer la localisation des collections (visible sur l'OPAC) ou faire un catalogue de vos collections de périodiques.

Pour ajouter votre collection, cliquez sur **Ajouter une collection**

* **Collection** : indiquez depuis quel numéro/date vous recevez la revue
* **Lacunes : indiquez les numéros manquants**
* **Statut** : indiquez si vous ne recevez plus la revue : sélectionnez «titre arrêté».

{% hint style="info" %}
Pour retrouver rapidement vos collections signalées (afin de les corriger) : **Recherche Multicritères > État des collections > Localisation des collections**
{% endhint %}

## La relecture des notices

Régulièrement (une fois par mois), il faut envoyer ses notices pour la relecture par le parrain.

Déroulement en trois étapes :

* 1\) Après la saisie, chaque producteur relit d’abord ses notices en internes, elles ont donc le statut : Relecture interne.
* 2\) Lorsqu’elles sont prêtes à être relues par le parrain, il faut les imprimer et envoyer ce fichier au parrain. Changer leur statut : A vérifier Nom\_du\_parrain.
* 3\) Lorsqu’elles sont corrigées suites aux remarques du parrain, elles sont prêtes à être intégrées dans l’OPAC. Changer leur statut : A valider N Samuel
*
  * Ex : Je suis le CDTM de Montpellier, je veux envoyer mes notices du mois de janvier à mon relecteur : la MCM Nantes.

### 1. Chercher les notices à relire

```
Onglet Catalogue > recherche > multi-critères
```

* Ajouter un critère de recherche sur « Notices>Statut de la notice
* Sélectionner « relecture interne
* Ajouter un critère de recherche sur « Personnalisables des notices>Producteur de la notice »
* Sélectionner « CDTM MONTPELLIER »

Créer une recherche prédéfinie permettra de lancer la recherche automatiquement le mois prochain :

![](<.gitbook/assets/image (57).png>)

* Cliquer sur mémoriser en recherche prédéfinie
* Donner un nom : « Fiches à relire » puis enregistrer (pas de raccourci, c’est inutile, ne pas cocher actif dans le bandeau de recherche).

Pour retrouver la recherche prédéfinie, aller dans :

```
Catalogue > recherche > prédéfinies
```

Sélectionner la recherche en cliquant dessus : Cliquer sur rechercher.

### 2. Imprimer les notices à relire

![](<.gitbook/assets/image (53).png>)

* Sans déplier les notices, cliquer sur l’icône de l’imprimante
* Dans la nouvelle fenêtre, remplir les champs suivants :
*

```
* Étendue de l’impression : « Toutes les notices du résultat de la recherche »
```

```
* Format des notices : « Format long »
* Informations exemplaires : cocher « Imprimer les exemplaires »
* Format de sortie : cocher « Traitement de texte »

Cliquer sur « imprimer » Une nouvelle fenêtre s’ouvre pour vous permettre de choisir le traitement de texte dans lequel vous allez enregistrer votre fichier (en général Word ou Open Office) :
```

![](<.gitbook/assets/image (31).png>)

Lorsque vous validez le choix, en cliquant sur OK, le fichier est automatiquement ouvert avec l’ensemble des notices.

* Supprimez les images (couvertures automatiquement chargées)
* Enregistrez ce fichier dans un dossier spécifique (dossier de rangement des fichiers PMB à envoyer), en lui donnant un nom reconnaissable par votre parrain : CIIP012012.doc (par exemple).
* Envoyez ce fichier à votre parrain par courrier électronique.

Après envoi du fichier au parrain, il faut penser à changer le statut des notices en lui donnant le nom « A vérifier MCM Nantes » (qui notre parrain pour ce mois-ci).

### 3. Introduire les corrections

A réception des corrections du parrain, il faudra corriger chaque notice ou simplement changer son statut. Pour retrouver ces notices, il faudra aller dans :

```
Onglet Catalogue > recherche > multi-critères
```

* Ajouter un critère de recherche sur « Notices>Statut de la notice »
* Sélectionner « MCM Nantes »
* Ajouter un critère de recherche sur « Personnalisables des notices>Producteur de la notice » Sélectionner « CDTM Montpellier »
* Rechercher

Modifier chaque notice corrigée et finaliser en lui donnant le statut « A valider N Samuel ».

![](<.gitbook/assets/image (14).png>)

##

## **Créer une étagère virtuelle**

{% hint style="info" %}
On peut comparer les étagères virtuelles aux étagères physiques de votre bibliothèque qui permettent de présenter vos nouveautés ou une sélection de références de votre centre de ressources que vous avez effectuée sur une thématique particulière.
{% endhint %}

{% hint style="info" %}
Les étagères virtuelles sont constituées de paniers de notices. Leur création et leur gestion nécessitent de connaître la gestion des paniers.
{% endhint %}

### **1. Créer une étagère**

```
Onglet Catalogue > Étagères > Gestion
```

Choisir « Ajouter une étagère ». Puis, dans la nouvelle fenêtre :

![](<.gitbook/assets/image (21).png>)

* Saisissez le nom de votre étagère (qui sera visible par le public)
* Définissez sa validité (par défaut « permanente » mais vous pouvez préciser une durée définie)

{% hint style="danger" %}
**Ne pas cocher l'option qui propose de l**'**afficher en page d'accueil**
{% endhint %}

* le champ « Nom long ou commentaire » vous permet de détailler le contenu de votre étagère. Ce commentaire sera visible par vos lecteur·rices.
* le champ « Commentaire de gestion » est à usage interne, il n'est pas visible par le public
* Enregistrez

### **2. Alimenter l'étagère**

* Créez un panier de notices
* Sélectionnez les notices que vous souhaitez déposer dans votre étagère virtuelle et ajoutez-les à votre panier, puis rendez vous dans le menu :

```
Catalogue > Étagères > Constitution
```

* Sélectionnez parmi tous vos paniers qui s'affichent celui avec lequel vous voulez remplir votre étagère virtuelle
* Enregistrez

L'étagère virtuelle est maintenant créée et remplie.

### 3. P**artager votre étagère virtuelle**

Voir la liste de vos étagères virtuelles en vous rendant dans :

```
Catalogue > Étagères > Consitution
```

![](<.gitbook/assets/image (9).png>)

Dans la colonne « Visible en page d'accueil ? », vous trouvez l'URL vers l'affichage de votre étagère dans l'environnement de l'OPAC :

![](<.gitbook/assets/image (22).png>)

Vous pouvez copier ce lien et le partager avec vos lecteur·rices en le copiant dans un courriel, en l'ajoutant sur une page de votre site, etc.

## **La circulation des documents**

L'onglet Circulation de PMB permet de réaliser des prêts, des retours de documents, des réservations, d'enregistrer des lecteur·rices...



{% hint style="info" %}
**ritimo** peut fournir les statistiques annuelles de prêt pour chaque localisation
{% endhint %}

{% hint style="info" %}
Il est nécessaire de **créer des lecteur·rices** pour pouvoir utiliser cette fonction
{% endhint %}

{% hint style="danger" %}
Il est indispensable de respecter le **Règlement général sur la protection des données (RGPD)** adopté par le Parlement européen le 27 avril 2016 et dont les dispositions sont directement applicables depuis le 25 mai 2018.

Une donnée personnelle est entendue comme toute information se rapportant à une personne physique identifiée ou identifiable, directement ou indirectement grâce à un identifiant (ex : numéro de carte d’adhérent à la bibliothèque)

* Les données de l’emprunteur sont conservées pendant la durée du service (le temps du prêt) et sont supprimées un an à compter de la date de fin du prêt précédent.
* Les informations relatives à chaque prêt sont supprimées à la fin du 4ème mois suivant le retour du document. (configuration PMB à faire)

**Responsabilité de ritimo :**

* Veiller à la sécurité des données et notifier les violations auprès de la CNIL.
* Veiller à ne pas conserver les données des lecteurs plus d’un an après la fin de l’adhésion => suppression automatique.

**Responsabilité des membres et relais qui utilisent le service :**

* A chaque création de fiche lecteur : limiter les informations recueillies à ce qui est strictement nécessaire.
* Les personnes concernées par les traitements de données doivent être informées de la finalité, des données collectées, de leurs destinataires, de leur durée de conservation et des droits qu’elles détiennent sur ces données. Le consentement appartient à l’utilisateur·rice, il ou elle doit pouvoir le retirer simplement et à tout moment.
* Supprimer les données des lecteur·rices si pas de ré-adhésion (ménage une fois pas an impératif).
* Ne pas consulter les adhérents des autres localisations du réseau.

Il est obligatoire d'établir un **registre des activités de traitement** qui permet de recenser vos traitements de données et de disposer d’une vue d’ensemble de ce que vous faites avec les données personnelles.

_Pour en savoir plus :_ [_https://www.cnil.fr/sites/default/files/atoms/files/ns09.pdf_](https://www.cnil.fr/sites/default/files/atoms/files/ns09.pdf) _et_&#x20;

[https://biblionumericus.fr/2018/03/14/rgpd-et-bibliotheques-cartographie-des-traitements-de-donnees-personnelles/](https://biblionumericus.fr/2018/03/14/rgpd-et-bibliotheques-cartographie-des-traitements-de-donnees-personnelles/)
{% endhint %}

### 1. Création d'un nouveau groupe de lecteur·rices

{% hint style="info" %}
L'utilisation d'un catalogue unique pour l'ensemble des bibliothèques du réseau **ritimo** nécessite de créer un **groupe de lecteur·rices** par localisation.

Par souci de confidentialité, il est recommandé de faire bien attention à n'utiliser / ne visualiser que le groupe de lecteur·rices associé à votre localisation.
{% endhint %}

Envoyer la demande de création à la gestion centralisée de la Ritimothèque.

### 2. Créer un nouveau lecteur·rice

```
Circulation > Nouveau lecteur
```

#### 2.1 créer un code barre

![](<.gitbook/assets/Screenshot 2021-06-15 at 15-19-02 Nouveau lecteur - PMB (1).png>)

Chaque lecteur·rice est associé·e à un numéro unique. Il convient de créer **un système de numérotation** différent de celui des exemplaires, afin d'éviter tout risque de confusion.

:point\_right: Préconisation de **ritimo** pour constituer le système de numérotation :

* préfixe constitué de la lettre **L** (comme lecteur·rice)
* premières lettres du nom de la bibliothèque / localisation
* numéro

Exemple pour un·e lecteur·rice du Cicodes : LCICO0001

Une fois le code-barres défini, cliquez sur `Suivant` afin d'accéder à l'écran de saisie des informations du/de la lecteur·rice.

#### 2.2. Renseigner les champs

Remplissez le formulaire en complétant les champs.

![](<.gitbook/assets/Screenshot 2021-06-15 at 15-22-08 Nouveau lecteur.png>)

Ne renseigner que les champs indispensables pour l'activité de la bibliothèque (ainsi, **le sexe de la personne, l'année de naissance pour les adultes, la profession, etc. ne devraient pas être demandés**), il faut pouvoir justifier la nécessité de récolter ces informations.

_Les informations personnelles_ :

* Nom
* Prénom
* Adresse
* Téléphone
* e-mail
* Profession
* Sexe
* Année de naissance.

_Informations de gestion_ :

* catégorie à choisir : association / collectivité / individuel
* code statistique : adhérent·e / membre/relais ritimo / salarié e / stagiaire / autre
* ajouter à un groupe (nom du centre)
* localisation (nom du centre)
* date d’adhésion

La date de début d'adhésion s'affiche automatiquement à la date de saisie. Pour la modifier, cliquez sur le bouton correspondant. Choisissez ensuite la date souhaitée à l'aide du calendrier.

La date de fin d'adhésion est calculée par PMB (la durée d'adhésion paramétrée par ritimo est de 365 jours). Elle ne s'affiche qu'après l'enregistrement de la fiche lecteur.

Il est possible de donner un identifiant OPAC à la personne. Cela lui permettre d'accéder à ses informations personnelles.

Cliquez sur `Enregistrer` pour terminer l'inscription et accéder à la fiche.

### 3. Prêter un document

```
Circulation > Prêt de document
```

![](<.gitbook/assets/Screenshot 2021-06-15 at 15-56-19 Circulation Prêt de documents.png>)

Par défaut, la localisation de votre bibliothèque s'affiche. Vous pouvez accédez à la fiche du/ de la lecteur·rice de deux façons :

* en saisissant le code-barres du lecteur.
* en saisissant le début ou la totalité du nom de famille du lecteur.

Dans la fiche lecteur·rice, le curseur est automatiquement placé dans le champ `Ajouter un prêt` :

![](<.gitbook/assets/Screenshot 2021-06-15 at 15-59-57 Circulation Prêt de documents.png>)

Saisissez le code-barres du document (son numéro d'exemplaire) pour effectuer le prêt. Le document prêté s'affiche automatiquement dans la liste des prêts en cours.

*   **Annuler un prêt**

    Il est possible d'annuler le dernier prêt enregistré (dans ce cas, le prêt n'est pas comptabilisé dans les statistiques, contrairement à un prêt suivi d'un retour immédiat).

    Pour cela, cliquez sur le bouton `Annuler`
*   **Imprimer le ticket de prêt**

    Vous pouvez également `imprimer un ticket de prêt`. Une fenêtre pop-up s'ouvre dans laquelle vous retrouvez les prêts en cours sous forme de courrier.

{% hint style="info" %}
**Messages d'alerte**

Différents messages d'alerte peuvent s'afficher lors de l'enregistrement d'un prêt. Il est donc indispensable de regarder l'écran à chaque opération de prêt.
{% endhint %}

* **"Document exclu du prêt"** : si le document possède un statut interdisant le prêt, le message "Ce document est exclu du prêt" apparaît. Trois choix sont possibles : annuler le prêt, forcer le prêt (en cliquant sur `Prêter`), Consulter et/ou modifier l'exemplaire en cliquant sur `Voir l'exemplaire`
* **"Document déjà en prêt" : si** l'exemplaire demandé est déjà emprunté par un lecteur, un message apparaît lors de l'enregistrement. Il est possible d'enregistrer la réservation du document.
* **Prolongation :** il est possible de prolonger le prêt d'un exemplaire : dans la liste des prêts en cours, la date de retour de chaque document est affichée sur la droite. Il suffit de modifier la date dans le calendrier. _Attention : un point d'exclamation rouge indique, dans le tableau des prêts, que le document en cours de prêt est réservé par un autre lecteur. Il faut donc en tenir compte avant de valider une nouvelle prolongation._

### 4. Restitution d'un document

```
Circulation > Prêt de document
```

![](<.gitbook/assets/Screenshot 2021-06-15 at 16-17-11 Circulation Retour de documents.png>)

Le curseur est automatiquement placé dans le formulaire de retour.

Saisissez le code-barres de l'exemplaire pour enregistrer le retour.

Une fois le retour effectué, un message de confirmation est affiché pour vérifier éventuellement que le code-barres correspond bien au document rendu.

**Effectuer un autre retour de document :** Lors de l'enregistrement du retour d'un document, le curseur se positionne de nouveau automatiquement dans le formulaire de retour : il est donc possible de retourner des exemplaires les uns à la suite des autres.

{% hint style="info" %}
**Messages d'alerte**

Différents messages d'alerte peuvent s'afficher lors du retour d'un prêt. Il est donc indispensable de regarder l'écran à chaque opération de prêt.
{% endhint %}

### 5. Suppression des fiches lecteur·rices périmées

{% hint style="info" %}
**Une fois par an,** il est indispensable de **supprimer les fiches lecteur·rices** qui n'ont pas été renouvelées (la durée de conservation ne doit jamais dépasser la date de fin d'adhésion + un an).
{% endhint %}

* Entrer le nom du/de la lecteur·rice pour afficher sa fiche
* Cliquer sur le bouton "supprimer" (fonctionne à condition qu'il n'y ait plus aucun prêt en cours).
