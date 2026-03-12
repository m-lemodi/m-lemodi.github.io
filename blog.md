---
layout: default
title: Blog
description: Mes articles et réflexions sur l'informatique et la technologie
---

<section class="blog-section">
  <h2>Mon Blog</h2>
  <p>Bienvenue sur mon blog où je partage mes réflexions sur l'informatique, le développement, le DevOps et la cybersécurité.</p>

  <div class="posts-list">
    {% for post in site.posts %}
    <article class="post-preview">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <div class="post-meta">
        <span class="post-date">{{ post.date | date: "%d %B %Y" }}</span>
        {% if post.author %}
        <span class="post-author">par {{ post.author }}</span>
        {% endif %}
      </div>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ post.url }}" class="read-more">Lire la suite →</a>
    </article>
    {% endfor %}
  </div>

  {% if paginator.total_pages > 1 %}
  <div class="pagination">
    {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}" class="prev">← Précédent</a>
    {% endif %}

    <span class="page-number">Page {{ paginator.page }} sur {{ paginator.total_pages }}</span>

    {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" class="next">Suivant →</a>
    {% endif %}
  </div>
  {% endif %}
</section>