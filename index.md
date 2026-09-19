---
layout: default
title: Home
permalink: /
custom_color: grape
custom_font: space
scroll_top_btn:
  enable: true

# Banner Section
banner:
  enable: true
  badge: "NEW"
  text: "LATEST NEWS - CARAVEL paper accepted at MICCAI 2026"
  link:
    label: "Read more"
    url: "#"
    target: "_blank"

# Hero Section
hero:
  title: "Mapping the hidden architecture"
  title_highlight: "of the brain"
  subtitle: "CARAVEL develops reliable AI methods to extract, model and analyse the brain vessel tree across multiple imaging scales."
  # Set to true to show the animated video instead of the static image below
  use_video: true
  video: /assets/video/CARAVEL_hero_video.mp4
  image: /assets/img/hero_image.png
  buttons:
    - label: "Explore the project"
      url: "#research"
      icon: "uil uil-arrow-right"
    - label: "Meet the team"
      url: "#team"
      style: "outline"

# Partners / Funding Section
partners:
  enable: true
  logos:
    - image: /assets/img/LOGO_ERC-FLAG_FP.png
      alt: "Funded by the European Union - European Research Council"
      wide: true
    - image: /assets/img/eurecom.png
      alt: "EURECOM Sophia Antipolis"

# News Section
news_section:
  enable: true

# Research Section
research_section:
  enable: true
  title: "Understanding the cerebrovascular tree, <br/> from <span class=\"text-caravel-coral\">image</span> to <span class=\"text-caravel-coral\">insight</span>."
  description: "CARAVEL studies the cerebrovascular system using advanced imaging and trustworthy AI to extract, model and analyse brain vessel trees across multiple spatial scales."
  focus_label: "Our research focuses on"
  items:
    - image: "/assets/img/research_1.png"
      title: "Brain vessel tree representation"
      text: "Building structured, multi-scale representations of the cerebrovascular network that capture its complexity and connectivity across imaging modalities."
    - image: "/assets/img/research_2.png"
      title: "Segmentation & Modeling"
      text: "Developing robust, trustworthy AI methods to detect, segment and model the brain vessel tree from neurovascular images."
    - image: "/assets/img/research_3.png"
      title: "Neurovascular atlas construction"
      text: "Constructing a spatio-temporal atlas of the cerebral vascular system to capture anatomical variability across scales and populations."
    - image: "/assets/img/research_4.png"
      title: "Clinical Usage"
      text: "Translating CARAVEL's methods into tools that support clinical decision-making and neurovascular risk assessment."
    - image: "/assets/img/research_5.png"
      title: "Reproducibility & open-source"
      text: "Releasing open datasets, code and benchmarks so the research community can validate, reuse and build on CARAVEL's results."

# Publications Section
publications_section:
  enable: true
  filters:
    - label: "All"
      filter: "all"
    - label: "Journals"
      filter: "journal"
    - label: "Conferences"
      filter: "conference"
    - label: "Preprints"
      filter: "preprint"
  # Newest paper first. Copy one block, paste it at the top, change the text.
  # type must be one of: journal, conference, preprint (small letters).
  # tag is the label shown on the card: Journal, Conference or Preprint.
  # To show a "Code" button, add a line:  github: "https://github.com/..."
  items:
    - date: "Mon YYYY"
      type: "conference"
      tag: "Conference"
      title: "Title of the conference paper"
      venue: "Name of the conference (e.g. MICCAI 2026)"
      url: "https://link-to-the-paper"
      github: "https://github.com/your-repo"
    - date: "Mon YYYY"
      type: "journal"
      tag: "Journal"
      title: "Title of the journal paper"
      venue: "Name of the journal"
      url: "https://link-to-the-paper"
    - date: "Mon YYYY"
      type: "preprint"
      tag: "Preprint"
      title: "Title of the preprint"
      venue: "arXiv preprint"
      url: "https://link-to-the-paper"

# Team Section
team_section:
  enable: true
  title: "The people behind <span class=\"text-caravel-coral\">CARAVEL</span>"
  description: "A multidisciplinary team working together to advance the understanding of the brain vessel tree through imaging and computational methods."
  lead:
    name: "Maria A. Zuluaga"
    photo: "/assets/img/team/zuluaga.jpeg"
    bio: "Professor at <a href=\"#\">EURECOM</a> and Affiliate Faculty in the School of Biomedical Engineering & Imaging Sciences at <a href=\"#\">King's College London</a>."
    website: "#"
    linkedin: "#"
    scholar: "#"
  members:
    # Add a "photo: /assets/img/team/<file>.jpeg" line once a real photo is available;
    # without it, the grey circle placeholder is shown automatically.
    - name: "Name Surname"
      role: "PhD Student at EURECOM"
      website: "#"
      linkedin: "#"
      scholar: "#"
    - name: "Name Surname"
      role: "PhD Student at EURECOM"
      website: "#"
      linkedin: "#"
      scholar: "#"
    - name: "Name Surname"
      role: "PhD Student at EURECOM"
      website: "#"
      linkedin: "#"
      scholar: "#"
    - name: "Name Surname"
      role: "PhD Student at EURECOM"
      website: "#"
      linkedin: "#"
      scholar: "#"
  cta:
    text: "Interested in joining the team?"
    label: "View open positions"
    url: "mailto:maria.zuluaga@eurecom.fr"

# Contacts Section
contacts_section:
  enable: true
  title: "Get in touch"
  subtitle: "Got any questions? Don't hesitate to get in touch."
  items:
    - icon: "uil-location-pin-alt"
      label: "Address"
      value: "450 Route des Chappes - 06410 Biot, France"
    - icon: "uil-envelope"
      label: "Email"
      value: "maria.zuluaga@eurecom.fr"
      url: "mailto:maria.zuluaga@eurecom.fr"
    - icon: "uil-university"
      label: "Institution"
      value: "EURECOM"
---
<div class="content-wrapper">
<header class="w-100">
{% include components/sections/home/banner.html %}

{% include components/navbar/navbar.html 
  classList="navbar-light navbar-bg-light"
  logoAlt="logo-dark"
  centerNav=true
  otherClassList="d-flex ms-auto"
  onePage=true
%}
</header>
<!-- /header -->

{% include components/sections/home/hero.html %}
{% include components/sections/home/partners.html %}
{% include components/sections/home/news.html %}
{% include components/sections/home/research.html %}
{% include components/sections/home/publications.html %}
{% include components/sections/home/team.html %}
{% include components/sections/home/contacts.html %}
{% include components/footer/caravel-footer.html %}
</div>