---
layout: default
title: Home
---

<div class="hero-section">
  <div class="hero-content">
    <div class="hero-text">
      <h1>Mariya Messerli</h1>
      <p class="hero-subtitle">Investor & Financial Professional</p>
      <p class="hero-description">
        I am an investor managing my own family funds, based in Switzerland. 
        My investment philosophy is global and long-term focused with aim to compound value over decades.
      </p>
      <div class="hero-cta">
        <a href="/about/" class="cta-button">Learn More</a>
        <a href="/blog/" class="cta-button secondary">Read Blog</a>
      </div>
    </div>
    <div class="hero-image">
      <img src="/assets/img/mariya-messerli.jpg" alt="Mariya Messerli" class="profile-image">
    </div>
  </div>
</div>

<div class="featured-section">
  <h2>Latest Insights</h2>
  <div class="featured-posts">
    {% for post in site.posts limit:3 %}
      <div class="featured-post">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="post-date">{{ post.date | date: "%B %-d, %Y" }}</p>
        {% if post.tags %}
          <div class="tags">
            {% for tag in post.tags limit:2 %}
              <span class="tag">{{ tag }}</span>
            {% endfor %}
          </div>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</div>
