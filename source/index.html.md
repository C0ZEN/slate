# Documentation Ticket Manager

Ticket Manager est une application SaaS qui permet de suivre l'évolution des 
incidents via un système de tickets.

Cette documentation réalisée par SupTrac permet d'en apprendre plus sur les 
droits des utilisateurs et sur le comportement et la démarche pour 
suivre et créer des tickets le plus facilement possible.
 

## Routing

**Connexion : /login**

Permet d'établir la connexion avec l'application.<br>
Nécéssite un *username* et *password*.

**Tous les tickets : /all-tickets**

Liste des tickets.

**Nouveaux tickets : /home**

Liste des tickets avec le statut *New*.

**Mes tickets : /my-tickets**

Liste des tickets avec le statut *In progress*.<br>
<aside class="warning">
Seul un développeur peut accéder à cette vue.
</aside>
<br>

**Ajouter un ticket : /add-ticket**

Permet l'ajout d'un nouveau ticket.<br>
<aside class="warning">
Seul un créateur peut accéder à cette vue.
</aside>
<br>

**Détails : /tickets/:id**

Permet d'avoir plus d'informations sur un ticket.<br>
Permet l'exécution d'actions sur le ticket.

## Simulation créateur

Cette section est un exemple de toutes les possibilités que propose Ticket
Manager pour un créateur.

### 1. Création

Après connexion, rendez-vous sur la vue pour créer un ticket.<br>
Pour ce faire, cliquez sur le bouton *Add a ticket*.<br>

Sur cette vue, vous devrez remplir tous les champs.<br>
Les champs grisés ne sont pas modifiables et contiennent des informations 
à propos du ticket.<br>
Remplissez les champs *Summary*, *Description* et *Priority*.<br>

Vous serez abonner par défaut au ticket.<br>
Quand vous êtes abonné à un ticket, vous recevrez un mail dès qu'un commentaire
est posté sur celui-ci.<br>
Vous pouvez vous désabonner en décochant l'option *Subscribe to notifications*.

Cliquez sur *New ticket* pour valider la création du ticket.<br>
Vous serez prévenu par alerte et notification du résultat de cette création.
Vous pouvez créer de suite un nouveau ticket, nous supprimons les champs 
variables pour vous faire gagnez du temps.

### 2. Visualisation

Vous venez de créer un ticket.<br>
Vous pouvez maintenant le trouver dans la vue des nouveaux tickets.<br>
Pour ce faire, cliquez sur le bouton *New tickets*.

Par défaut, les tickets sont triés par plus anciens aux plus récents.<br>
Vous pouvez modifier les tris des façons suivantes :
- Utilisez le champ de recherche - impacte toutes les données
- Cliquez sur les colonnes pour trier sur celle-ci (filtre alphabétique ou 
par critère en fonction des colonnes)
- Recliquez sur celle-ci pour inverser le sens du tri

### 3. Détails

Pour obtenir plus d'informations sur un ticket et surtout effectuer des actions
sur celui-ci, vous devez le sélectionner.<br>
Pour ce faire, cliquez sur le bouton *Get details* dans la liste.

**3.1. Détails**

La première partie contient toutes les informations à propos de ce ticket.
Vous retrouverez toutes les informations issues du formulaire de création du 
ticket et d'autres informations complémentaires.

Vous pouvez également vous désabonner des notifications par mail en cliquant 
sur la cloche en haut à droite.

**3.2. Edition**

Si vous souhaitez modifier les informations saisi au préalable lors de la 
création du ticket, un bouton est disponible à cet effet.<br>
<aside class="warning">
Ce bouton n'est visible que par le créateur de ce ticket.
</aside>
<br>

Au clique sur le bouton, le formulaire apparaît.<br>
Il ne vous reste plus qu'à modifier ces informations puis valider.<br>
La modification n'est pas disponible pour un ticket clôturé.

**3.3. Suppression**

Si vous souhaitez supprimer un ticket, un autre bouton est également
présent à cet effet.<br>
Les conditions d'accessibilité et de visibilité sont les mêmes que pour le
bouton d'édition.

Au clic sur le bouton, un modal s'ouvre afin de faire une seconde 
vérification.<br>
Cliquez à nouveau sur supprimer pour supprimer définitivement le ticket.

## Simulation développeur

### 1. Visualisation

La vue de tous les tickets et des nouveaux tickets est disponible au même 
titre que pour un créateur.<br>
Il existe cependant une vue supplémentaire.<br>
Cliquez sur le bouton *My tickets* pour vous y rendre.

Cette vue liste tous les tickets qui appartiennent au développeur connecté et
qui ont le statut en *In progress*.<br>
Vous pouvez filtrer les tickets au même titres que les autres liste.

### 2. Détails

Pour obtenir plus d'informations sur un ticket et surtout effectué des actions
sur celui-ci, vous devez le sélectionner.<br>
Pour ce faire, cliquez sur le bouton *Get details* dans la liste.

**3.1. Détails**

La première partie contient toutes les informations à propos de ce ticket.
Vous retrouvez toutes les informations issues du formulaire de création du 
ticket et d'autres informations complémentaires.

Vous pouvez également vous désabonnez des notifications par mail en cliquant 
sur la cloche en haut à droite.

**3.2. Travailler**

Si le ticket a le statut à *New*, alors vous pouvez vous l'approprié.<br>
S'approprié un ticket permet vous permet de le commenté.<br>
Il ne peut y avoir qu'un développeur assigné par ticket.

Lorsqu'un développeur est assigné à un ticket, le ticket passe au statut de
*In progress*.<br>
Le bouton *Commenter* est également disponible.

**3.3. Commenter**

Cliquez sur le bouton *Commenter* ouvre un modal.<br>
Ce modal contient un formulaire qui permet de commenté le ticket.<br>
Comme pour un ticket, les champs sont obligatoires et certaines informations 
sont déjà fournies et non modifiables.

Une fois le commentaire ajouter, il sera visible en dessous des boutons d'
actions.<br>
Vous pouvez commenté un ticket même si celui-ci a le statut à *Done* pour 
fournir des informations supplémentaires au besoin.

**3.4. Stoper**

Si vous avez souhaitez clôturé le ticket, vous pouvez cliquez sur le bouton
*Stop working*.<br>
Le statut du ticket passera à *Done*.

Vous pourrez toujours commenté le ticket mais le créateur de celui-ci
ne pourra plus le modifier ou le supprimer.

## Sécurité

**Mots de passe**

Les mots de passe sont *salés* en base de donnée afin de veiller à une sécurité
de vos données optimales.

**Stockage**

Vos inofrmations d'indetifications sont stockées dans le *LocalStorage* afin de
persister la connexion et d'offrir un gain de temps sur la connexion.

**Droits**

Lors de l'accès à une page, nous vérifions les droits pour éviter toute 
intrusion dans notre appliation.


## Crédits

Ticket Manager est une application conçu par SupTrac.<br>
Tous les droits reviennent à SupTrac.

Remerciements :

- BOUTHORS Clément
- COMPERE Benoit
- EGO Romain
- TESTELIN Geoffrey
