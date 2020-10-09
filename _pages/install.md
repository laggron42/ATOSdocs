---
permalink: /install/
title: "Installation"
toc: true
---

## Invitez le bot

Si vous avez la permission "Gérer le serveur", vous pouvez inviter Botnol sur votre serveur avec le lien suivant :

**https://discord.com/oauth2/authorize?client_id=612906116451532821&scope=bot&permissions=268692560**

## Configuration initiale de Red

Le préfixe par défaut est `!`. Cela veut dire que toutes les commandes commencent par ce caractère. Essayez par exemple `!ping` et voir si le bot réponds. Si il ne réponds pas, vérifier les permissions. Vous pouvez également le mentionner (ex: `@Botnol ping`).

### Changer le préfixe

Si vous souhaitez changer le préfixe, utilisez la commande `!set serverprefix <vos préfixes>`. Vous pouvez régler plusieurs préfixes.

> Exemples :
> 
> - `!set serverprefix ?`
> - `!set serverprefix $ botnol.`

### Définissez vos rôles de modérateur et d'administrateur

Les permissions des commandes sont basées sur ces deux rôles. Choisissez un ou plusieurs rôles considérés modérateurs ou administrateurs, et utilisez les commandes `!set addadminrole <nom du role>` pour les rôles d'administrateurs et `!set addmodrole` pour les rôles de modérateurs.

### Les commandes

Botnol possède plein de commandes, séparées en plusieurs catégories.

Tapez `!help` et le bot affichera la liste des commandes auxquelles vous avez accès. Cela veut dire que le bot n'affichera pas la même liste entre un administrateur et un simple membre.

Tapez `!help <Catégorie>` pour afficher la liste des commandes d'une catégorie en particulier (attention aux majuscules). Par exemple `!help Tournaments` pour les commandes liées aux tournois (je vais y revenir).

Tapez `!help <commande>` pour afficher une description plus détaillée d'une certaine commande.

Il existe également des "sous-commandes", c'est à dire des commandes sous une autre. Par exemple, la commande `!set serverprefix` est une sous-commande de `!set`. Tapez `!help set` pour voir la liste des sous-commandes, et `!help set serverprefix` pour voir la description détaillée de la sous-commande.

## Configuration du module Tournaments

Si vous installez ce bot, c'est probablement pour sa gestion avancée des tournois. Je vais vous expliquer les différentes étapes pour bien commencer.

Premièrement, configurer vos identifiants Challonge. Vous devez connaitre votre nom d'utilisateur ainsi que votre clé d'API (obtenable dans les paramètres utilisateur Challonge, catégorie "API Developer"). Tapez d'abord la commande `!challongeset username <votre pseudo>`, puis `!challongeset api` (ne collez pas directement votre clé, le bot vous la demandera en MP).

Ensuite, la commande `!tset` (ou `!tournamentset`) vous permet de configurer tous les réglages.

### Réglage des channels

Configurez les différents channels de votre serveur avec `!tset channels`.

- `!tset channels announcements` Channel des annonces pour le début des inscriptions, du check-in et du tournoi.
- `!tset channels checkin` Le check-in s'y déroulera (les gens y entreront `!in`). Si ce n'est pas réglé, les gens pourront check n'importe où.
- `!tset channels queue` Le bot y annoncera les sets lancés.
- `!tset channels register` Les inscriptions s'y dérouleront (les gens y entreront `!in` ou `!out`). Si ce n'est pas réglé, les gens pourront s'inscrire n'importe où.
- `!tset channels scores` Le channel pour régler le score de son set avec la commande `!win`. Si ce n'est pas réglé, les gens pourront régler leur score n'importe où.
- `!tset channels stream` Les sets passant en stream y seront annoncés.
- `!tset channels to` Le channel privé des T.O., où le bot annoncera les éventuels problèmes ou demandes pour le tournoi. **Contrairement aux autres channels qui sont optionnels, vous devez régler le channel des T.O.**

### Réglage des rôles

Ensuite, configurez les différents rôles. Vous devez donner le nom complet du rôle avec la commande, ou son ID.

- `!tset roles participant` Le rôle attribué aux participants lors de l'inscription. **Le réglage de ce rôle est requis.**
- `!tset roles streamer` Le rôle qui aura accès aux commandes de streamer.
- `!tset roles to` Le rôle de vos T.O.s, donnant accès aux commandes liées (sauf `!tset`). **Vous n'avez pas besoin de configurer cela si vous avez déjà configué des rôles d'admin ou de modo avec les commandes `!set addadminrole/addmodrole`, ce qui est recommandé.** N'utilisez ce réglage que si vos T.O.s ne sont pas déjà modérateurs.

Vous pouvez également configurer un rôle de joueur (limitant les inscriptions à ce rôle, tout en le mentionnant pour l'ouverture des inscriptions) dans une prochaine étape.

### Réglages divers

Quelques autres réglages utiles :

- `!tset delay` Définis le temps (en minutes) avant qu'un joueur soit considéré comme AFK, et disqualifié. 10 minutes par défaut.
- `!tset startbo5` Définis quand est-ce que les sets passent de BO3 à BO5 (utilisez `!help tset startbo5` pour plus de détails).
- `!tset register` Règle les heures d'ouverture et de fermeture automatique des inscriptions. Vous pouvez toujours les lancer/fermer manuellement.
- `!tset checkin` Règle les heures d'ouverture et de fermeture automatique du check-in. Vous pouvez toujours le lancer/fermer manuellement.
- `!tset warntime` Définis le temps avant d'avertir les joueurs et les T.O.s de la durée de leur match.
- `!tset autostopregister` Définis si le bot doit automatiquement arrêter les inscriptions lorsque le tournoi est plein.
- `!tset twostageregister` Permet la mise en place d'inscriptions en deux temps, en donnant une 2e heure d'ouverture des inscriptions. Cela permet par exemple de faire des inscriptions de dernière minute pour remplir les dernières places.

### Réglages des jeux

Dernière étape : le réglage des différents jeux. Certains paramètres dépendent des jeux de vos tournois.

D'abord, ajoutez votre jeu avec `!tset games add`. **Le nom du jeu doit être le nom complet tel qu'il est affiché sur Challonge.**

Ensuite, le bot vous donnera directement la liste des autres commandes que vous pouvez utilisez. Vous allez pouvoir définir le ruleset, la liste des stages (+ counters) légaux, le rôle de joueur, le mode de ban, et même les infos Braacket pour le seeding auto.

-----

Pour récapituler, utilisez `!tset settings` et `!tset games show` et vérifiez que tous les réglages sont corrects.

Une fois que tout est bon, on peut configurer notre premier tournoi !

## Lancer un tournoi

D'abord, créez un tournoi sur Challonge, configurez le comme vous le souhaitez (attention à bien régler la date de lancement, car les horaires des inscriptions et du check-in sont basés dessus). Vous pouvez également régler une limite de participants que le bot va appliquer pour les inscriptions.

Ensuite, utilisez la commande `!setup <lien du Challonge>`. Le bot affichera un récapitulatif des réglages, puis confirmez.

A partir de cette étape, la commande `!tinfo` deviens accessible à tout moment, vous affichant le statut actuel du tournoi et des informations utiles en lien avec la phase actuelle.

Il n'y a plus qu'à attendre le lancement des inscriptions et du check-in, vous n'avez rien à faire ! Si vous avez désactivé l'automatisation, lancez manuellement avec `!register start` et `!checkin start`.

Une fois les inscriptions et le check-in terminé, vous pouvez lancer le tournoi (ce n'est pas automatique) avec `!start`. Les sets vont être lancés avec leurs channels au fur et à mesure.

Lorsque le tournoi est terminé, n'oubliez pas d'utiliser `!end` pour correctement mettre fin au tournoi et nettoyer ce qu'il reste.
