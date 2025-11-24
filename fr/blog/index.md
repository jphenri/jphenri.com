---
layout: page
title: "Blog"
subtitle: "Notes, tests et comptes rendus"
nav_key: blog
lang: fr
en_url: /blog/
---

<div class="blog-banner blog-header-animated">

## 📝 Bienvenue sur le Blog (FR)

Ici, je partage mes analyses, expériences et découvertes autour de :

- **IA appliquée** (PME, automatisation, outils pratiques)
- **DevOps / TI** (Intune, Trellix, Linux, sécurité)
- **Home Lab** (tests, lab, Plex, gaming, distros)
- **Business 2.0** (stratégie, transformation numérique)

Chaque article est basé sur :  
**du réel, du terrain, et ce que j'expérimente dans mes projets ou au travail.**

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
