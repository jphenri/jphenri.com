---
layout: home
title: "Home"
nav_key: home
lang: en
fr_url: /fr/
---

<!-- 🔥 Hero + Cards (original home.html content) -->
<section class="hero">
  <div class="hero-inner">
    <p class="hero-kicker">AI · DevOps · Digital Transformation</p>

    <h1 class="hero-title">
      Building <span>Business 2.0</span> with technology
    </h1>

    <p class="hero-subtitle">
      I’m J.P. Henri – IT analyst, AI consultant and content creator based in Gatineau.
      I help small businesses modernize with AI, automation and practical strategy.
    </p>

    <div class="hero-actions">
      <a href="#business" class="btn btn-primary">Explore Business 2.0</a>
      <a href="#contact" class="btn btn-ghost">Talk about your project</a>
    </div>
  </div>
</section>

<section class="cards-grid">

  <article class="card">
    <h2>Business 2.0 for SMEs</h2>
    <p>Digital diagnostics, automation, generative AI and process optimization.</p>
    <a href="#business" class="card-link">See the approach</a>
  </article>

  <article class="card">
    <h2>DevOps / IT</h2>
    <p>Endpoint management, Linux automation and compliance best practices.</p>
    <a href="#projects" class="card-link">View topics</a>
  </article>

  <article class="card">
    <h2>Project</h2>
    <p>
      My projects combine small business digital transformation,
      fast GitHub Pages websites, AI workflows and real-world experimentation.
    </p>
    <a href="#projects" class="card-link">See the project</a>
  </article>

</section>

<!-- 🔥 Main one-page content -->
<section id="business" class="section">
  <h2>Business 2.0</h2>
  <p>
    <strong>Business 2.0</strong> is my practical framework for using technology in a realistic,
    simple and sustainable way for small businesses.
  </p>
</section>

<section id="projects" class="section">
  <h2>Projects</h2>
  <p class="section-lead">Examples of applied IT, AI and Business 2.0.</p>

  <section class="projects-grid">

    <article class="project-card">
      <h3><a href="https://chezgerry1958.com">Chez Gerry 1958</a></h3>
      <p class="project-card-meta">Premium shoe restoration</p>
      <p>Website, SEO, content strategy and workflow optimization.</p>
    </article>

    <article class="project-card">
      <h3><a href="https://chucks-casse-croute.com">Chuck’s Casse-Croute</a></h3>
      <p class="project-card-meta">Static site</p>
      <p>Simple, fast and low-maintenance showcase website.</p>
    </article>

    <article class="project-card">
      <h3><a href="#">Pronatureqc.com</a></h3>
      <p class="project-card-meta">Archived e-commerce</p>
      <p>Large product catalog, SEO and checkout integration.</p>
    </article>

    <article class="project-card">
      <h3><a href="#">Assystech SENC</a></h3>
      <p class="project-card-meta">IT consulting</p>
      <p>Web development, infrastructure and support.</p>
    </article>

  </section>
</section>

<section id="blog" class="section">
  <h2>Blog</h2>
  <p class="section-lead">Recent English posts.</p>

  <div class="latest-posts-grid">
    {% assign posts_en = site.posts | where: "lang", "en" | sort: "date" | reverse %}
    {% for post in posts_en limit:3 %}
      <article class="post-card">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="post-card-meta">{{ post.date | date: "%Y-%m-%d" }}</p>
        <p class="post-card-excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
      </article>
    {% endfor %}
  </div>

  <p class="section-more"><a href="/blog/">View all posts →</a></p>
</section>

<section id="contact" class="section section-contact">
  <h2>Contact</h2>
  <p>Get in touch for a project or idea:</p>
  <ul>
    <li>📧 <a href="mailto:contact@jphenri.ca">contact@jphenri.ca</a></li>
    <li>🔗 LinkedIn (add your link)</li>
  </ul>
</section>
