---
layout: splash
permalink: /what-is-red/
title: Powered by Red
header:
  overlay_color: "#5e616c"
  overlay_image: assets/images/redbot-header.png
  overlay_filter: 0.3
  caption: "Artwork de [Sinlaire](https://sinlaire.deviantart.com/) pour Red Discord Bot"
  actions:
    - label: "<i class='fas fa-info-circle'></i> En savoir plus"
      url: "https://github.com/Cog-Creators/Red-DiscordBot/"
author_profile: true
excerpt: >
  Botnol est une instance de Red-DiscordBot, un bot modulaire open-source, accessible à tous !
---

## Qu'est-ce que Red bot ?

Red est un bot open source auto hébergeable, c'est à dire qu'il n'existe pas de bot que vous pouvez inviter, c'est à vous d'installer le programme, créer un compte bot sur Discord, puis vous n'avez plus qu'à rentrer les informations pour avoir votre propre bot fonctionnel en un rien de temps !

Il est entièrement customisable, vous pouvez non seulement changer le nom, la photo de profil, ou même le statut de votre bot, mais il est surtout modulaire !

En installant Red, vous avez une vingtaine de modules disponibles que vous pouvez activer ou non, comme vous le souhaitez. Vous pouvez donc par exemple décider d'activer l'audio ainsi que les outils de modération, en gardant ce dont vous n'avez pas besoin désactivé.

### Les modules communautaires

En plus des modules proposés de base, il existe une grande communauté proposant des modules supplémentaires, installables facilement, afin d'étendre encore plus les capacités de votre bot selon vos besoin !

Il existe plus de 300 modules approuvés, offrant toutes les fonctions dont vous pouvez avoir besoin : levels, automod, mini jeux, annonces, outils d'administration...

## Et les tournois dans tout ça ?

Toutes les fonctions et commandes liées aux tournois ne sont qu'un simple module pour ce bot ! Ce module nommé "Tournaments" fait partie de ma collection de modules installables pour Red : **[Laggron's Dumb Cogs](https://github.com/retke/Laggrons-Dumb-Cogs)** !

Parmi cette collection de modules se trouve également WarnSystem, le système de modération intégré au bot (dont vous vous servez probablement pas, mais j'avais quand même envie de le noter, c'est mon 2e module majeur).

## Pourquoi utiliser Red, et ne pas créer un bot dédié ?

Même si j'ai les capacités de faire mon propre bot, on voit aujourd'hui énormément de bots dont 90% des fonctions sont les mêmes partout (modération, audio, commandes...), avec 10% de fonctions uniques qui intéressent les gens, on retrouve donc plein de bots différents pour une seule fonction sur les serveurs.

Je préfère donc coder avec Red, car nous, codeurs, n'avons plus besoin de devoir refaire la même base à chaque fois. On se concentre sur une chose : les commandes que l'on souhaite coder, ces fameux 10% de fonctions uniques, puis on laisse les gens installer cette partie indépendament du reste s'ils le souhaitent.

## Du coup, je peux héberger moi même le bot ?

Il est pensé pour ça, avant même de penser aux autres serveurs !

Vous n'avez qu'à suivre les instructions d'installation pour Red sur votre OS :

<a href="https://docs.discord.red/" class="btn btn--danger btn--large">Installer Red</a>

Une fois que c'est installé, prenez un peu le temps de découvrir comment il fonctionne. Lisez [le guide d'introduction à Red](https://docs.discord.red/en/stable/getting_started.html) *que j'ai écrit btw* et explorez un peu les modules disponible.

### Installer Tournaments sur Red

`[p]` est considéré comme votre préfixe.
{: .notice--info}

1. Assurez vous que Downloader est chargé :
   ```
   [p]load downloader
   ```

2. Ajoutez mon repository, Laggron's Dumb Cogs :
   ```
   [p]repo add Laggrons-Dumb-Cogs https://github.com/retke/Laggrons-Dumb-Cogs
   ```
   N'oubliez pas de confirmer la notice en disant "I agree".

3. Installez Tournaments :
   ```
   [p]cog install Laggrons-Dumb-Cogs tournaments
   ```

4. Chargez le cog !
   ```
   [p]load tournaments
   ```

Et voilà, Tournaments est prêt à être utilisé, aucune configuration supplémentaire n'est nécessaire !
