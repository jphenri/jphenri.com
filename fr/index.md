---
layout: home
title: "Accueil"
nav_key: home
lang: fr
en_url: /
---

<section id="hero" class="hero">
  <p class="hero-kicker">jphenri.ca · TI, IA & Business 2.0</p>
  <h1>Aider les petites entreprises à évoluer avec de la techno qui respecte leur réalité.</h1>
  <p class="hero-subtitle">
    Je construis et j’expérimente des sites, workflows et outils pensés pour des PME réelles,
    pas pour des slides de présentation.
  </p>
  <div class="hero-actions">
    <a href="#projects" class="hero-btn primary">Voir les projets</a>
    <a href="#contact" class="hero-btn ghost">Me contacter</a>
  </div>
</section>

<section id="business" class="section">
  <h2>Business 2.0</h2>
  <p>
    Pour moi, <strong>Business 2.0</strong>, c’est une PME qui utilise la technologie pour
    simplifier sa vie, pas pour se rajouter une couche de complexité.
  </p>
  <ul>
    <li>On part du terrain : ce qui se passe vraiment à l’atelier, au comptoir, dans la boîte courriel.</li>
    <li>L’IA et l’automatisation servent d’assistants, pas de “magie” qui remplace tout.</li>
    <li>Les processus restent compréhensibles par les humains.</li>
    <li>On mesure ce qui compte vraiment : temps gagné, clarté, service au client.</li>
  </ul>
  <p>
    La plupart de ces idées sont testées dans de vrais projets, comme ceux ci-dessous.
  </p>
</section>

<section id="projects" class="section">
  <h2>Projets</h2>
  <p class="section-lead">
    Quelques projets qui montrent comment je pense TI, web et Business 2.0 sur le terrain.
  </p>

  <section class="projects-grid">

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Business 2.0 · Commerce local</span>
        <h3 class="project-card-title">
          <a href="https://chezgerry1958.com" target="_blank" rel="noopener noreferrer">
            Chez Gerry 1958
          </a>
        </h3>
        <p class="project-card-meta">Cordonnerie haut de gamme · Gatineau, Québec</p>
      </div>
      <p class="project-card-desc">
        Projet de transformation numérique continue : site web, SEO, fiches services claires
        et contenu qui montre réellement le travail de restauration de chaussures.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Site statique · Restauration</span>
        <h3 class="project-card-title">
          <a href="https://chucks-casse-croute.com" target="_blank" rel="noopener noreferrer">
            Chuck’s Casse-Croute
          </a>
        </h3>
        <p class="project-card-meta">Site vitrine léger · GitHub Pages</p>
      </div>
      <p class="project-card-desc">
        Site ultra léger pour un casse-croûte local, sans CMS ni base de données, pensé pour
        être rapide, simple et facile à partager avec les clients.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">E-commerce · Plein air</span>
        <h3 class="project-card-title">
          <a href="https://web.archive.org/web/20171012223444/https://www.pronatureqc.com/"
             target="_blank" rel="noopener noreferrer">
            Pronatureqc.com (2015–2018)
          </a>
        </h3>
        <p class="project-card-meta">Plateforme de vente en ligne · Archive</p>
      </div>
      <p class="project-card-desc">
        Boutique en ligne complète pour produits de chasse et plein air : catalogue important,
        navigation optimisée et SEO pour rester visible.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Consultation TI & Web</span>
        <h3 class="project-card-title">
          <a href="https://web.archive.org/web/20181229095915/https://assystech.com/"
             target="_blank" rel="noopener noreferrer">
            Assystech SENC (2015–2019)
          </a>
        </h3>
        <p class="project-card-meta">Consultation TI · Dév. web</p>
      </div>
      <p class="project-card-desc">
        Entreprise de consultation TI et développement web cofondée, avec mandat d’accompagner
        des PME dans leur infrastructure, leurs sites et leur support.
      </p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Lab perso · Hub de connaissances</span>
        <h3 class="project-card-title">
          <a href="https://jphenri.ca" target="_blank" rel="noopener noreferrer">
            jphenri.ca
          </a>
        </h3>
        <p class="project-card-meta">Site statique bilingue · GitHub Pages + Jekyll</p>
      </div>
      <p class="project-card-desc">
        Ce site lui-même : un laboratoire pour documenter TI, IA et Business 2.0 en français
        et en anglais, sur une base statique propre.
      </p>
    </article>

  </section>
</section>

<section id="blog" class="section">
  <h2>Blog</h2>
  <p class="section-lead">
    Quelques articles récents en français. D’autres arrivent au fil des projets.
  </p>

  <div class="latest-posts-grid">
    {% assign posts_fr = site.posts | where: "lang", "fr" | sort: "date" | reverse %}
    {% for post in posts_fr limit:3 %}
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
    <a href="/fr/blog/">Voir tous les articles →</a>
  </p>
</section>

<section id="contact" class="section section-contact">
  <h2>Contact</h2>
  <p>
    Si vous voulez parler d’un projet (PME, site web, workflows IA, TI),
    envoyez-moi un court message avec un peu de contexte.
  </p>
  <ul>
    <li>Courriel : <a href="mailto:contact@jphenri.ca">contact@jphenri.ca</a></li>
    <li>LinkedIn : <a href="https://www.linkedin.com" target="_blank" rel="noopener noreferrer">Profil LinkedIn (exemple)</a></li>
  </ul>
  <p>
    Je ne prends pas tous les mandats, mais je lis tout.
  </p>
</section>

