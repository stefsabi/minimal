---
layout: default
title: Blog
permalink: /blog/
---

<div class="blog-hero">
  <div class="blog-hero-content">
    <h1>Investment Insights</h1>
    <p class="blog-subtitle">Thoughts on markets, companies, and long-term value creation</p>
  </div>
</div>

<div class="blog-content">
  <div class="blog-intro">
    <p>Exploring investment opportunities through fundamental analysis, with a focus on insurance, technology, and global markets.</p>
  </div>

  <div class="blog-grid">
    {% for post in site.posts %}
      <article class="blog-card">
        <div class="blog-card-content">
          <div class="blog-card-header">
            <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
            <time class="blog-date">{{ post.date | date: "%B %-d, %Y" }}</time>
          </div>
          
          {% if post.excerpt %}
            <p class="blog-excerpt">{{ post.excerpt }}</p>
          {% endif %}
          
          {% if post.tags %}
            <div class="blog-tags">
              {% for tag in post.tags %}
                <span class="blog-tag">{{ tag }}</span>
              {% endfor %}
            </div>
          {% endif %}
          
          <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read Article →</a>
        </div>
      </article>
    {% endfor %}
  </div>

  <div class="blog-footer">
    <p>For investment inquiries or discussions, please <a href="/minimal/contact/">get in touch</a>.</p>
  </div>
</div>