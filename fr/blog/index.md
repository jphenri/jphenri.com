---
layout: page
title: "Blog"
subtitle: "Notes, tests et comptes rendus"
nav_key: blog
lang: fr
en_url: /blog/
---

<div class="blog-banner blog-header-animated">

<h2>📝 Bienvenue sur le Blog (FR)</h2>

<p>
Ici, je partage mes analyses, expériences et découvertes autour de :
</p>

<ul>
  <li><strong>IA appliquée</strong> (PME, automatisation, outils pratiques)</li>
  <li><strong>DevOps / TI</strong> (Intune, Trellix, Linux, sécurité)</li>
  <li><strong>Home Lab</strong> (tests, Plex, gaming, distros)</li>
  <li><strong>Business 2.0</strong> (stratégie, transformation numérique)</li>
</ul>

<p>
Chaque article est basé sur <strong>du réel, du terrain</strong> – ce que j'apprends dans mes projets, dans mon lab et dans mon travail.
</p>

</div>

<section class="latest-posts">
  <h2>Derniers articles</h2>

  {% assign posts_fr = site.posts | where: "lang", "fr" | sort: "date" | reverse %}

  {% if posts_fr.size == 0 %}
    <p class="latest-posts-empty">
      Aucun article en français pour le moment. Le premier arrive bientôt.
    </p>
  {% else %}
    <div class="latest-posts-grid">
      {% for post in posts_fr limit:5 %}
      <article class="post-card">
        <h3>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <p class="post-card-meta">
          {{ post.date | date: "%Y-%m-%d" }}
        </p>
        {% if post.excerpt %}
          <p class="post-card-excerpt">
            {{ post.excerpt | strip_html | truncate: 150 }}
          </p>
        {% endif %}
        <a class="post-card-link" href="{{ post.url | relative_url }}">
          Lire la suite →
        </a>
      </article>
      {% endfor %}
    </div>
  {% endif %}
</section>

---

## 🇬🇧 Version anglaise

→ Pour lire le blog anglais, rendez-vous ici :  
**[Blog (EN)](/blog/)**

---

### Comment les articles fonctionnent

Tout article publié dans `_posts` avec :

```yaml
lang: fr
layout: post
