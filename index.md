---
layout: home
title: "Home"
nav_key: home
lang: en
fr_url: /fr/
---
<section id="hero" class="hero">
  <p class="hero-kicker">jphenri.ca · IT, AI & Business 2.0</p>
  <h1>Helping small businesses and teams level up with tech that actually fits reality.</h1>
  <p class="hero-subtitle">
    I build and experiment with websites, workflows and tools that make sense for
    real-world small businesses, not just slide decks.
  </p>
  <div class="hero-actions">
    <a href="#projects" class="hero-btn primary">View projects</a>
    <a href="#contact" class="hero-btn ghost">Get in touch</a>
  </div>
</section>

<section id="business" class="section">
  <h2>Business 2.0</h2>
  <p>
    For me, <strong>Business 2.0</strong> means using technology to simplify a small business –
    not to bury it under tools, dashboards and logins.
  </p>
  <ul>
    <li>Start from reality: what actually happens at the counter, in the shop, in the inbox.</li>
    <li>Use AI and automation as assistants, not as “magic replacements”.</li>
    <li>Keep processes understandable by humans first.</li>
    <li>Measure what matters: time saved, clarity gained, customers better served.</li>
  </ul>
  <p>
    Most of what I test ends up applied in <a href="#projects">my projects</a> with real businesses.
  </p>
</section>

<section id="projects" class="section">
  <h2>Projects</h2>
  <p class="section-lead">
    A selection of projects that show how I think about small business, web and IT.
  </p>

  <section class="projects-grid">

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Business 2.0 · Local SMB</span>
        <h3 class="project-card-title">
          <a href="https://chezgerry1958.com" target="_blank" rel="noopener noreferrer">
            Chez Gerry 1958
          </a>
        </h3>
        <p class="project-card-meta">Premium shoe restoration · Gatineau, Québec</p>
      </div>
      <p class="project-card-desc">
        Long-term digital transformation for a high-end cobbler: clean UX, structured services,
        strong local SEO and authentic content that shows the real work behind the repairs.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Static site · Food project</span>
        <h3 class="project-card-title">
          <a href="https://chucks-casse-croute.com" target="_blank" rel="noopener noreferrer">
            Chuck’s Casse-Croute
          </a>
        </h3>
        <p class="project-card-meta">Micro-restaurant website · GitHub Pages</p>
      </div>
      <p class="project-card-desc">
        Ultra-lightweight static site on GitHub Pages for a local casse-croûte. Fast, minimal,
        no CMS — just a clean link to share with customers.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">E-commerce · Outdoor & hunting</span>
        <h3 class="project-card-title">
          <a href="https://web.archive.org/web/20171012223444/https://www.pronatureqc.com/"
             target="_blank" rel="noopener noreferrer">
            Pronatureqc.com (2015–2018)
          </a>
        </h3>
        <p class="project-card-meta">Full e-commerce platform · Archived</p>
      </div>
      <p class="project-card-desc">
        Large catalog store for outdoor and hunting products: search, inventory, secure checkout
        and SEO to keep it visible.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">IT consulting · Web</span>
        <h3 class="project-card-title">
          <a href="https://web.archive.org/web/20181229095915/https://assystech.com/"
             target="_blank" rel="noopener noreferrer">
            Assystech SENC (2015–2019)
          </a>
        </h3>
        <p class="project-card-meta">Consulting & custom web projects</p>
      </div>
      <p class="project-card-desc">
        Co-owned consulting business delivering infrastructure, websites and support for SMBs
        needing a long-term technical partner.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Personal lab · Knowledge hub</span>
        <h3 class="project-card-title">
          <a href="https://jphenri.ca" target="_blank" rel="noopener noreferrer">
            jphenri.ca
          </a>
        </h3>
        <p class="project-card-meta">Bilingual static site · GitHub Pages + Jekyll</p>
      </div>
      <p class="project-card-desc">
        This site itself: a place to document IT, AI and Business 2.0 experiments in EN/FR
        with a clean static architecture.
      </p>
    </article>

  </section>
</section>

<section id="blog" class="section">
  <h2>Blog</h2>
  <p class="section-lead">
    Selected posts in English. More coming as I publish and translate.
  </p>

  <div class="latest-posts-grid">
    {% assign posts_en = site.posts | where: "lang", "en" | sort: "date" | reverse %}
    {% for post in posts_en limit:3 %}
      <article class="post-card">
        <h3>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <p class="post-card-meta">
          {{ post.date | date: "%Y-%m-%d" }}
        </p>
        {% if post.summary %}
          <p class="post-card-excerpt">
            {{ post.summary }}
          </p>
        {% elsif post.excerpt %}
          <p class="post-card-excerpt">
            {{ post.excerpt | strip_html | truncate: 150 }}
          </p>
        {% endif %}
      </article>
    {% endfor %}
  </div>

  <p class="section-more">
    <a href="/blog/">View all posts →</a>
  </p>
</section>

<section id="contact" class="section section-contact">
  <h2>Contact</h2>
  <p>
    If you’d like to talk about small business projects, web, AI workflows or IT,
    the best way is to send me a short message with context.
  </p>
  <ul>
    <li>Email: <a href="mailto:contact@jphenri.ca">contact@jphenri.ca</a></li>
    <li>LinkedIn: <a href="https://www.linkedin.com" target="_blank" rel="noopener noreferrer">LinkedIn profile (placeholder)</a></li>
  </ul>
  <p>
    I don’t take on every project, but I do read everything.
  </p>
</section>

