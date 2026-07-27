---
layout: default
title: News
permalink: /news/
scroll_top_btn:
  enable: true
---
<div class="content-wrapper">
<header class="w-100">
{% include components/navbar/navbar.html
  classList="navbar-light navbar-bg-light"
  logoAlt="logo-dark"
  centerNav=true
  otherClassList="d-flex ms-auto"
  onePage=true
%}
</header>
<!-- /header -->

<section class="wrapper news-hero">
  <div class="container py-12 py-md-14">
    <div class="row justify-content-center text-center">
      <div class="col-lg-8">
        <span class="news-hero-category text-uppercase fs-13 fw-bold">CARAVEL</span>
        <h1 class="news-hero-title mt-3 mb-0">All News</h1>
      </div>
    </div>
  </div>
</section>

<section class="wrapper bg-light">
  <div class="container py-14 py-md-16">
    <div class="row gy-8">
      {% assign news_items = site.news | sort: 'date' | reverse %}
      {% for item in news_items %}
      <div class="col-md-6 col-lg-4">
        <article class="h-100 d-flex flex-column">
          <div class="news-card-img rounded mb-5">
            {% if item.image %}<img src="{{ item.image | relative_url }}" alt="{{ item.title }}">{% endif %}
          </div>
          <div class="post-header d-flex align-items-center justify-content-between mb-3">
            <span class="text-line text-caravel-coral text-uppercase fs-13 fw-bold">{{ item.category }}</span>
            <span class="news-card-date fs-13">{{ item.date | date: "%-d %B %Y" }}</span>
          </div>
          <h3 class="h4 mb-3"><a class="link-dark" href="{{ item.url | relative_url }}">{{ item.title }}</a></h3>
          <p class="news-card-text mb-3">{{ item.excerpt }}</p>
          <a href="{{ item.url | relative_url }}" class="news-card-link hover d-inline-flex align-items-center mt-auto">Read more <i class="uil uil-arrow-right fs-16 ms-1"></i></a>
        </article>
      </div>
      {% endfor %}
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container -->
</section>

{% include components/footer/caravel-footer.html %}
</div>
