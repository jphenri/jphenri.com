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
    <p>Digital diagnostics, generative AI and process optimization.</p>
    <a href="#business" class="card-link">See the approach</a>
  </article>

  <article class="card">
    <h2>Social media automation</h2>
    <p>Tiktok, Youtube shorts, Facebook/Instagram reel automation and compliance best practices.</p>
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
  <p class="section-lead">
    Business 2.0 is my practical framework for using technology in a realistic, simple and sustainable way
    for small businesses.
  </p>
  <p>
    Most small businesses don’t need a dozen new tools — they need <strong>clarity</strong>, less manual work
    and better visibility on what really matters. My work starts from what already exists in the shop,
    the inbox, the spreadsheets and the conversations with clients, then adds just enough structure,
    automation and AI to make a difference.
  </p>
  <ul>
    <li><strong>Understand the reality</strong>: how work actually flows today (not how it “should” work).</li>
    <li><strong>Simplify first</strong>: remove friction and noise before adding new systems.</li>
    <li><strong>Add targeted automation</strong>: only where it saves real time or reduces risk.</li>
    <li><strong>Use AI as an assistant</strong>: to help with content, documentation and decision-making, not to replace people.</li>
    <li><strong>Measure the impact</strong>: time saved, fewer errors, better customer experience.</li>
  </ul>
  <p>
    Everything I test in my lab eventually ends up applied in real projects with real businesses —
    like the ones below.
  </p>
</section>


<section id="projects" class="section">
  <h2>Projects</h2>
  <p class="section-lead">
    Examples of applied IT, AI and Business 2.0 — always tied to real businesses and clear outcomes.
  </p>

  <section class="projects-grid">

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Business 2.0 · SMB</span>
        <h3 class="project-card-title">
          <a href="https://chezgerry1958.com" target="_blank">Chez Gerry 1958</a>
        </h3>
        <p class="project-card-meta">Premium shoe restoration · Gatineau, Québec</p>
      </div>
      <p class="project-card-desc">
        Long-term digital transformation for a high-end cobbler: website, clear service catalog,
        local SEO, content that shows real before/after work, and backend processes that make it
        easier to handle mail-in repairs.
      </p>
      <p class="project-card-desc">
        This project is my main sandbox for testing how far you can push Business 2.0 inside a
        single local shop without losing its personality.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Static site · Food</span>
        <h3 class="project-card-title">
          <a href="https://chucks-casse-croute.com" target="_blank">Chuck’s Casse-Croute</a>
        </h3>
        <p class="project-card-meta">Lightweight restaurant site · GitHub Pages</p>
      </div>
      <p class="project-card-desc">
        A fast, minimal and low-maintenance website for a local casse-croûte. Built entirely
        with static files on GitHub Pages, it’s an example of how a very small business can
        still look professional online without a heavy CMS.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">E-commerce · Outdoor</span>
        <h3 class="project-card-title">
          <a href="https://web.archive.org/web/20171012223444/https://www.pronatureqc.com/" target="_blank">
            Pronatureqc.com (2015–2018)
          </a>
        </h3>
        <p class="project-card-meta">Full online store · Archived</p>
      </div>
      <p class="project-card-desc">
        Large-catalog e-commerce site for outdoor and hunting products. Work included navigation
        structure, product content, search optimization and performance, all while staying aligned
        with the brand’s identity.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">IT consulting</span>
        <h3 class="project-card-title">
          <a href="https://web.archive.org/web/20181229095915/https://assystech.com/" target="_blank">
            Assystech SENC (2015–2019)
          </a>
        </h3>
        <p class="project-card-meta">Consulting · Web development</p>
      </div>
      <p class="project-card-desc">
        Co-founded IT consulting and web development company. I worked with small and
        medium-sized businesses on infrastructure decisions, custom websites and ongoing
        technical support.
      </p>
      <p class="project-card-desc">
        The experience shaped how I now approach Business 2.0: long-term relationships,
        clear language and solutions that match each client’s real constraints.
      </p>
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
  <p class="section-lead">
    If you have a project or idea and you’re not sure where to start, we can begin with a simple conversation.
  </p>
  <p>
    I’m especially interested in small businesses, local projects and teams who want to modernize
    without losing their identity. Whether it’s a website, a workflow, documentation or an AI use case,
    the first step is understanding your reality.
  </p>
  <ul>
    <li>🔗 LinkedIn: <a href="https://www.linkedin.com/in/jphenriIT/">LinkedIn</a></li>
  </ul>
  <p>
    You don’t need a full brief. A few lines about who you are, what you do and what’s blocking you
    is more than enough to start.
  </p>
</section>

