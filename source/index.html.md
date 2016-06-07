# Documentation RailCommander

RailCommander est une application de vente de ticket de train révolutionnaire 
pensée pour l'achat express de tickets.

Nous proposons un moyen simple, rapide et personnalisé afin de choisir des
tickets en rapport à des informations pertinentes à l'utilisateur.

RailCommander est disponible sur Android, iOs et desktop pour toute les 
résolutions.

## Navigation (mobile)

### Accueil

<aside class="info">
Le contenu de la page diffère si un utilisateur est connecté.
</aside>

Si l'utilisateur n'est pas connecté, la vue contient un message de bienvenue,
une présentation de RailCommander et des liens vers connexion et inscription.

Si l'utilisateur est connecté, la vue contient un message de bienvenue,
des statistiques sur RailCommande et un lien vers les achats.

### Accueil/Filtres

La vue contient les filtres pour les voyages et le bouton vers la liste des 
voyages.

Les filtres rapides ne trient qu'un voyage (avec ses horaires correspondant).

Les filtres personnalisés ajustent la recherche.

Pour filtrer tous les voyages, il faut utiliser le bouton 'Je choisi mes voyages'.

<aside class="warning">
Le bouton vers la vue des voyages est visible que si les filtres obligatoires
sont valides.
</aside>

### Accueil/Voyages

Liste les voyages en fonction des filtres.

Un champ de recherche est disponible pour trier les voyages.

Un sliding de droite à gauche affiche un bouton supprimer.<br>
Ce bouton permet de supprimer les voyages non désirables.

Un bouton refresh permet de réafficher tous les voyages issues de la recherche.

<aside class="warning">
Le bouton vers la vue de confirmation est visible que si au moins un voyage est
sélectionné.
</aside>

### Accueil/Confirmation

Liste les voyages sélectionnés avec les sous étapes correspondantes.

Un sliding de droite à gauche affiche les boutons plus et moins.<br>
Ces boutons permettent de changé la quantité de ticket pour le voyage 
correspondant.

<aside class="warning">
Le bouton vers la vue suivante est visible que si au moins un voyage est
sélectionné.
</aside>

<aside class="info">
Le contenu de la page diffère si un utilisateur est connecté.
</aside>

Si l'utilisateur n'est pas connecté, la vue contient un lien vers connexion.

Si l'utilisateur est connecté, la vue contient un lien vers l'achat.

### Accueil/Connexion

Affiche le bouton vers la connexion.

<aside class="info">
Après une connexion, la vue contient un message de confirmation de connexion et
le lien vers la page d'achat.
</aside>

### Accueil/Achat

Liste des voyages sélectionnés.

La vue contient des citations de personnalités importantes.

Le bouton Paypal permet d'effectué l'achat des tickets.

<aside class="info">
Un message de confirmation est présent dans la vue après qu'un achat Paypal
soit effectué ainsi qu'un bouton vers les achats.
</aside>

### Accueil/Paypal

Lors d'un achat avec Paypal, un modal s'ouvre.

L'utilisateur doit renseigné ses informations de connexion.

Il pourra procédé au paiement.

Lorsque le paiement est réussi, le modal se ferme.

### Compte

Contient une liste vers d'autres vues concernant l'utilisateur.

<aside class="info">
Le contenu de la page diffère si un utilisateur est connecté.
</aside>

Si l'utilisateur n'est pas connecté, la vue contient des liens vers connexion et
la création d'un compte.

Si l'utilisateur est connecté, la vue contient des liens vers compte, achats,
statistiques et déconnexion.

### Compte/Compte

Contient les informations sur l'utilisateur connecté en lecture seule.

Un bouton vers l'édition du compte est présent.

### Compte/Compte/Edition

Contient les informations sur l'utilisateur connecté en lecture/écriture.

L'utilisateur peut modifier ses informations (sauf l'email qui est unique) puis
valider les modifications via le bouton de sauvegarde.

### Compte/Achats

Contient la liste des tickets achetés pour l'utilisateur connecté.

Sélectionner un ticket pour afficher les actions disponibles.<br>
Après sélection, un bouton imprimer le ticket est disponible.<br>
Ce bouton permet l'impression depuis le téléphone.

### Compte/Statistiques

Contient les statistiques liés à cet utilisateur.

Nombre de tickets achetés, argent dépensé, kilomètres parcourus, like de 
RailCommander et succès pour obtenir des réductions sur les tarifs.

Possibilité de changer son like.

### Informations

Contient une liste vers d'autres vues concernant toutes les informations
sur RailCommander.

### Informations/A propos de nous

Contient des informations sur RailCommander.

L'histoire de RailCommander avec son commencement et des valeurs qui nous
importe et que nous mettons en place.

### Informations/Team

Contient la liste des collaborateurs intervenants pour RailCommander.

Un zoom est possible en sélectionnant un utilisateur afin d'obtenir des 
informations supplémentaires.

### Informations/Team/Zoom

Contient les détails pour le collaborateur sélectionné.

### Informations/Statistiques générales

Contient des statistiques à propos des achats de RailCommander.

Contient le taux de satisfaction, les kilomètres parcourus, le nombre de ticket
achetés et l'argent dépensé en tickets pour tous les utilisateurs.

### Informations/Statistiques

Contient les statistiques de l'utilisateur connecté.
Voir *Compte/Statistiques*.

### Informations/Mentions légales

Contient toutes les mentions légales de RailCommander.

Une surprise attend les courageux lecteur à la fin.

### Connexion

Contient sous forme de modal le formulaire pour se connecté avec Google,
Facebook et RailCommander.

Contient également les boutons vers la création de compte ou le mot de passe
oublié.

### Inscription

Contient sous forme de modal le formulaire pour s'inscrire avec RailCommander.

### Mot de passe oublié

Contient sous forme de modal le formulaire pour obtenir un nouveau mot de passe.

Cette action envoi le mot de passe par mail.

## Navigation (desktop)

### Accueil

Contient un message de bienvenue, une présentation de RailCommander, des
statistiques et nos valeurs.

### Filtres

La vue contient les filtres pour les voyages et le bouton vers la liste des 
voyages.

Les filtres rapides ne trient qu'un voyage (avec ses horaires correspondant).

Les filtres personnalisés ajustent la recherche.

Pour filtrer tous les voyages, il faut utiliser le bouton 'Je cherche mon voyage'.

### Voyages

Liste les voyages en fonction des filtres.

Un champ de recherche est disponible pour trier les voyages.

Il est possible de trier par ordre croissant ou décroissant les données en
sélectionnant les headers du tableau de voyages.

<aside class="warning">
Le bouton vers la vue de confirmation est visible que si au moins un voyage est
sélectionné.
</aside>

### Confirmation

Liste les voyages sélectionnés avec les sous étapes correspondantes.

Une colonne du tableau contient les boutons plus et moins.<br>
Ces boutons permettent de changé la quantité de ticket pour le voyage 
correspondant.

<aside class="warning">
Le bouton vers la vue suivante est visible que si au moins un voyage est
sélectionné.
</aside>

<aside class="info">
Le contenu de la page diffère si un utilisateur est connecté.
</aside>

Si l'utilisateur n'est pas connecté, la vue contient un lien vers connexion.

Si l'utilisateur est connecté, la vue contient un lien vers l'achat.

### Connexion

Affiche le bouton vers la connexion.

<aside class="info">
Après une connexion, la vue contient un message de confirmation de connexion et
le lien vers la page d'achat.
</aside>

### Achat

Liste des voyages sélectionnés.

Le bouton Paypal permet d'effectué l'achat des tickets.

<aside class="info">
Après un achat Paypal, l'utilisateur sera redirigé vers la vue d'impression.
</aside>

### Paypal

Lors d'un achat avec Paypal, un modal s'ouvre.

L'utilisateur doit renseigné ses informations de connexion.

Il pourra procédé au paiement.

### Impression

Liste des voyages venants d'être achetés avec Paypal.

Permet l'impression des tickets.

### Compte

<aside class="info">
Visible que si l'utilisateur est connecté.
</aside>

Contient sous forme de modal les informations sur l'utilisateur connecté en lecture/écriture.

L'utilisateur peut modifier ses informations (sauf l'email qui est unique) puis
valider les modifications via le bouton de sauvegarde.

### Achats

<aside class="info">
Visible que si l'utilisateur est connecté.
</aside>

Contient sous forme de modal la liste des tickets achetés, les succès et les 
statistiques de l'utilisateur connecté.

Un bouton permet l'impression des tickets.

### Applications mobiles

Contient sous forme de modal de la publicité pour RailCommander indiquant
que nous possédons également une application mobile.

### A propos de nous

Contient sous forme de modal la liste des collaborateurs intervenants pour 
RailCommander.

### Mentions légales

Contient sous forme de modal toutes les mentions légales de RailCommander.

### Connexion

Contient sous forme de modal le formulaire pour se connecté avec Google,
Facebook et RailCommander.

Contient également les boutons vers la création de compte ou le mot de passe
oublié.

### Inscription

Contient sous forme de modal le formulaire pour s'inscrire avec RailCommander.

### Mot de passe oublié

Contient sous forme de modal le formulaire pour obtenir un nouveau mot de passe.

Cette action envoi le mot de passe par mail.

## Simulation d'achat

Dans cette section, nous allons voir comment acheté des tickets avec RailCommander.

### Filtrer

Aller dans la vue des filtres, la première étape du procédé.

Vous devez remplir les champs obligatoires.<br>
En l'occurence, il s'agit de la ville d'arrivée et la ville de départ.<br>
Vous pouvez dès à présent passé à l'étape 2 ou filtrer plus précisement
votre recherche de voyage.

Les autres filtres disponibles sont les suivants :
- Prix maximum
- Date de départ (jour)
- Heures de départ (créneau, heure minimale/maximale)

Pour valider votre recherche, vous avez trois solutions :
- Le moins cher (affiche le voyage le moins cher)
- Le plus rapide (affiche le voyage le plus rapide)
- Tous (affiche tous les voyages en fonction des filtres)

Dans cette simulation, nous prenons la troisième option.

### Choisir

Vous êtes maintenant dans la vue avec votre liste de voyage.

Vous avez plusieurs possibilités qui s'offrent à vous.<br>
Sélectionnez par un clique les voyages qui vous intéressent.

Notez que vous devez sélectionné au moins un voyage pour passer à la vue 
suivante.

Dans cette simulation, nous sélectionnons les deux premiers voyages puis nous 
allons à l'étape suivante.

### Valider

Vous êtes maintenant dans la vue avec votre liste de voyage sélectionnés.

Vous pouvez visualiser en détails chaque sous étape du voyage.<br>
Par exemple, le trajet Lille-Marseille effectue dans un premier temps un 
Lille-Paris, puis Paris-Lyon et pour finir Lyon-Marseille.<br>
Ces trois étapes sont donc visualiable sur cette vue.

Vous pouvez modifier la quantité de ticket achetés.

Dans cette simulation, prenons deux tickets pour nos voyages puis allons à l'
étape suivante.

### Connexion

Vous êtes maintenant dans la vue de connexion.

Vous n'êtes toujours pas connecté à RailCommander.<br>
Le moment est venu de vous connecté.

Dans cette simulation, nous allons nous connecter avec notre compte RailCommander
mais vous pouvez aussi utiliser votre compte Google ou Facebook ou créer un 
compte RailCommander.

Une fois la connexion effectuée, nous allons à l'étape suivante.

### Achat

Vous êtes maintenant dans la vue d'achat.

Vous pouvez visualiser les voyages précédemment sélectionné avec leur quantité.

Procédons maintenant au paiement avec Paypal.<br>
Cliquez sur le bouton Paypal.<br>
Connectez-vous avec votre compte Paypal.<br>
Procédez maintenant au paiement des tickets.<br>
Une fois le paiement effectué, un lien vous permet de revenir sur RailCommander.

Vous êtes maintenant sur la vue des tickets et vous pouvez les imprimer.

<aside class="info">
Vous recevrez également mail de confirmation avec les tickets en pdf.
</aside>

## Sécurité

**Mots de passe**

Les mots de passe sont *hashés* et *salés* en base de donnée afin de veiller à 
une sécurité des données optimales.

**Stockage**

Les informations d'indetifications sont stockées dans le *LocalStorage* afin de
persister les données et d'offrir un gain de temps sur la connexion.
Il en va de même pour le choix des filtres et voyages.

**Droits**

Lors de l'accès à une page, nous vérifions les droits pour éviter toute 
intrusion dans notre application.

## Crédits

Tous les droits reviennent à RailCommander.
Lisez les conditions d'utilisations pour plus de détails.

**Remerciements :**

- BOUTHORS Clément
- COMPERE Benoit
- EGO Romain
- TESTELIN Geoffrey
