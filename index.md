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
    - image: /assets/img/erc.png
      alt: "European Research Council (ERC)"
    - image: /assets/img/eurecom.png
      alt: "EURECOM Sophia Antipolis"
    - image: /assets/img/ue.png
      alt: "Funded by the European Union"

# News Section
news_section:
  enable: true
  items:
    - category: "Publication"
      date: "12 May 2026"
      title: "CARAVEL paper accepted at MICCAI 2026"
      text: "Our latest work on cerebrovascular tree reconstruction has been accepted."
      url: "#"
    - category: "Event"
      date: "28 April 2026"
      title: "CARAVEL at MICCAI 2025"
      text: "We presented our recent results in Tokyo, Japan."
      url: "#"
    - category: "Opportunity"
      date: "10 April 2026"
      title: "PhD position on AI for brain vasculature"
      text: "Join our team and work on exciting research challenges."
      url: "#"

# Research Section
research_section:
  enable: true
  title: "Understanding the cerebrovascular tree, from <span class=\"text-caravel-coral\">image</span> to <span class=\"text-caravel-coral\">insight</span>."
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
    - date: "Sep 2025"
      type: "conference"
      tag: "Conference"
      title: "VesselVerse: A Dataset and Collaborative Framework for Vessel Annotation"
      venue: "MICCAI 2025, 28th International Conference on Medical Image Computing and Computer Assisted Intervention"
      url: "#"
    - date: "Apr 2024"
      type: "journal"
      tag: "Journal"
      title: "Graph representations of the brain vessel tree"
      venue: "IEEE Transactions on Medical Imaging"
      url: "#"
    - date: "Oct 2023"
      type: "preprint"
      tag: "Preprint"
      title: "Computational methods for cerebrovascular image understanding"
      venue: "NeuroImage"
      url: "#"

# Team Section
team_section:
  enable: true
  title: "The people behind <span class=\"text-caravel-coral\">CARAVEL</span>"
  description: "A multidisciplinary team working together to advance the understanding of the brain vessel tree through imaging and computational methods."
  lead:
    name: "Maria A. Zuluaga"
    bio: "Professor at <a href=\"#\">EURECOM</a> and Affiliate Faculty in the School of Biomedical Engineering & Imaging Sciences at <a href=\"#\">King's College London</a>."
    website: "#"
    linkedin: "#"
    scholar: "#"
  members:
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
    - name: "Name Surname3"
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

# Footer Section
footer_section:
  links:
    - label: "Research"
      url: "#research"
    - label: "News"
      url: "#news"
    - label: "Publications"
      url: "#publications"
    - label: "Team"
      url: "#team"
    - label: "Contacts"
      url: "#contacts"
  social:
    - icon: "uil-globe"
      url: "#"
    - icon: "uil-linkedin-alt"
      url: "#"
    - icon: "uil-graduation-cap"
      url: "#"
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
