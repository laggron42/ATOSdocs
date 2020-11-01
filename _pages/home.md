---
layout: splash
permalink: /
hidden: false
header:
  overlay_color: "#5e616c"
  overlay_filter: 0.3
  overlay_image: /assets/images/homepage.png
  actions:
    - label: "<i class='fas fa-download'></i> Installer maintenant"
      url: "/install-red/"
excerpt: >
  Un bot Discord pour organiser vos tournois Challonge directement sur Discord !
row1:
  - image_path: /assets/images/mm-free-feature.png
    alt: "organisation gestion"
    title: "Organisation et gestion"
    excerpt: "Des outils puissants à votre disposition pour gérer tout un tournoi facilement, testé jusqu'à 128 joueurs"
  - image_path: /assets/images/mm-responsive-feature.png
    alt: "discord integration"
    title: "Intégration avec Discord"
    excerpt: "Personne n'a besoin de créer de compte sur Challonge, tout est lié entre le bracket et votre serveur !"
  - image_path: /assets/images/mm-customizable-feature.png
    alt: "automatisation"
    title: "Grande automatisation"
    excerpt: "Le bot automatise quasiment tout le travail des organisateurs, tout ce qu'il vous reste à faire c'est surveiller dans l'ensemble !"

row2:
  - image_path: /assets/images/mm-free-feature.png
    alt: "Channels automatiques"
    title: "Channels automatiques"
    excerpt: >
      Des channels privés sont créés automatiquement pour chaque match, regroupant les deux joueurs pouvant discuter tranquillement. <br/>
      Ils ont à disposition des outils pour leur jeu, pour afficher les règles, les stages, ou encore appeler un organisateur <br/><br/>
      Les organisateurs, eux, ont une vue d'ensemble sur tous les channels et peuvent intervenir facilement dans un match sans déranger le reste !

row3:
  - image_path: /assets/images/mm-free-feature.png
    alt: "Inscriptions et check-in intégrés"
    title: "Inscriptions et check-in intégrés"
    excerpt: >
      Le bot intègre un système d'inscriptions et de check-in. Après une configuration simple, les gens n'auront plus qu'à entrer `!in` pour partciper !<br/><br/>
      Les options proposées s'adaptent aussi bien aux petits tournois qu'aux tournois majeurs, construit pour fonctionner avec de grands afflux de membres rapidement !

row4:
  - alt: "100% gratuit"
    title: "100% gratuit"
    excerpt: "Vous êtes libres de l'inviter, voir même de l'installer et de l'héberger, aucune commande ne vous sera bloquée, aucun message n'ira insister pour un Patreon !"

row5:
  - image_path: https://imgur.com/pY1WUFX.png
    alt: "powered by Red"
    title: "Powered by Red-DiscordBot"
    excerpt: >
      A.T.O.S. est une instance de Red-DiscordBot, un bot open-source hébergeable. <br/>
      Les fonctions de tournois ne sont qu'un module, faisant partie de ma collection de modules, <a
      href="https://github.com/retke/Laggrons-Dumb-Cogs">Laggron's Dumb Cogs</a>.
    url: "/what-is-red/"
    btn_label: "En savoir plus"
    btn_class: "btn--danger"

---

{% include feature_row id="row1" %}

{% include feature_row id="row2" type="left" %}

{% include feature_row id="row3" type="right" %}

{% include feature_row id="row4" type="center" %}

{% include feature_row id="row5" type="right" %}
