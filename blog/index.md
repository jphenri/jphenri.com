---
layout: page
title: "Blog"
subtitle: "Notes, tests and write-ups"
nav_key: blog
lang: en
fr_url: /fr/blog/
---

<div class="blog-banner blog-header-animated">

## 📝 Welcome to the Blog (EN)

Here I share my notes, experiments and lessons learned around:

- **Applied AI** (for small businesses, automation, practical tools)
- **DevOps / IT** (Intune, Trellix, Linux, security)
- **Home Lab** (lab tests, Plex, gaming, distros)
- **Business 2.0** (strategy, digital transformation)

Everything here is based on **real-world work, labs and client projects**, not theory.

</div>

<section class="latest-posts">
  <h2>Latest posts</h2>

  {% assign posts_en = site.posts | where: "lang", "en" | sort: "date" | reverse %}

  {% if posts_en.size == 0 %}
    <p class="latest-posts-empty">
      No English posts yet. First one is coming soon.
    </p>
  {% else %}
    <div class="latest-posts-grid">
      {% for post in posts_en limit:5 %}
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
          Read more →
        </a>
      </article>
      {% endfor %}
    </div>
  {% endif %}
</section>

---

### How posts work

Any file in `_posts` with:

```yaml
lang: en
layout: post
