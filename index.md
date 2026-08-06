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
      title: "Image-based extraction"
      text: "Developing robust methods to detect and reconstruct the brain vessel tree from neurovascular images across different modalities and resolutions."
    - image: "/assets/img/research_2.png"
      title: "Modelling & representation"
      text: "Building structured, multi-scale representations of the vascular network to capture its complexity and connectivity."
    - image: "/assets/img/research_3.png"
      title: "Analysis & understanding"
      text: "Designing computational approaches to analyse vascular patterns and support scientific insight into brain structure."

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
  items:
    - date: "Dec 2025"
      type: "preprint"
      tag: "Preprint"
      title: "An Automated Framework for Large-Scale Graph-Based Cerebrovascular Analysis"
      venue: "arXiv preprint (accepted at IEEE ISBI 2026)"
      url: "https://arxiv.org/abs/2512.03869"
    - date: "Sep 2025"
      type: "conference"
      tag: "Conference"
      title: "VesselVerse: A Dataset and Collaborative Framework for Vessel Annotation"
      venue: "MICCAI 2025, 28th International Conference on Medical Image Computing and Computer Assisted Intervention"
      url: "https://www.eurecom.fr/en/publication/8225"
    - date: "Feb 2025"
      type: "journal"
      tag: "Journal"
      title: "FUTURE-AI: International Consensus Guideline for Trustworthy and Deployable Artificial Intelligence in Healthcare"
      venue: "BMJ"
      url: "https://pmc.ncbi.nlm.nih.gov/articles/PMC11832024/"
    - date: "Jan 2022"
      type: "journal"
      tag: "Journal"
      title: "Vessel-CAPTCHA: An Efficient Learning Framework for Vessel Annotation and Segmentation"
      venue: "Medical Image Analysis"
      url: "https://www.sciencedirect.com/science/article/pii/S136184152100308X"
    - date: "Jun 2018"
      type: "journal"
      tag: "Journal"
      title: "Interactive Medical Image Segmentation Using Deep Learning with Image-Specific Fine-Tuning"
      venue: "IEEE Transactions on Medical Imaging"
      url: "https://pubmed.ncbi.nlm.nih.gov/29969407/"
    - date: "Aug 2015"
      type: "journal"
      tag: "Journal"
      title: "Stability, Structure and Scale: Improvements in Multi-Modal Vessel Extraction for SEEG Trajectory Planning"
      venue: "International Journal of Computer Assisted Radiology and Surgery"
      url: "https://pubmed.ncbi.nlm.nih.gov/25847663/"

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
    url: "#"

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
```
