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
  - image_path: /assets/images/mm-customizable-feature.png
    alt: "channels"
    title: "Channels automatiques"
    excerpt: "Chaque match lancé dispose d'un channel privé entre les deux joueurs et vos organisateurs."
  - image_path: /assets/images/mm-responsive-feature.png
    alt: "discord integration"
    title: "Intégration avec Discord"
    excerpt: "Personne n'a besoin de créer de compte sur Challonge, tout est lié entre le bracket et le serveur !"
  - image_path: /assets/images/mm-free-feature.png
    alt: "inscriptions checkin"
    title: "Inscriptions et Check-in"
    excerpt: "Un système automatique et entièrement customisable d'inscriptions est disponible directement via Discord."

row2:
  - image_path: /assets/images/mm-free-feature.png
    alt: "100% gratuit"
    title: "100% gratuit"
    excerpt: "Vous êtes libres de l'inviter, voir même de l'installer et de l'héberger, aucune commande ne vous sera bloquée !"

row3:
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
