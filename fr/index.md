---
layout: home
title: "Accueil"
nav_key: home
lang: fr
en_url: /
---

<!-- 🔥 Hero + Cards (ton ancien contenu du layout home.html) -->
<section class="hero">
  <div class="hero-inner">
    <p class="hero-kicker">
      IA · DevOps · Transformation numérique
    </p>

    <h1 class="hero-title">
      Construire le <span>Business 2.0</span> avec la technologie
    </h1>

    <p class="hero-subtitle">
      Je suis J.P. Henri – analyste TI, consultant IA et créateur de contenu basé à Gatineau.
      J'aide les PME à moderniser leurs opérations avec l’IA, l’automatisation et le bon sens.
    </p>

    <div class="hero-actions">
      <a href="#business" class="btn btn-primary">Découvrir Business 2.0</a>
      <a href="#contact" class="btn btn-ghost">Parler de votre projet</a>
    </div>
  </div>
</section>

<section class="cards-grid">

  <article class="card">
    <h2>Business 2.0 pour PME</h2>
    <p>
      Diagnostic numérique, automatisation des tâches répétitives,
      IA générative et optimisation des processus pour les petites entreprises.
    </p>
    <a href="#business" class="card-link">Voir l’approche</a>
  </article>

  <article class="card">
    <h2>DevOps / IT</h2>
    <p>
      Gestion poste de travail, Intune, automatisation Linux
      et bonnes pratiques de conformité pour environnements complexes.
    </p>
    <a href="#projects" class="card-link">Voir les sujets</a>
  </article>

  <article class="card">
    <h2>Projet</h2>
    <p>
      Mes projets réunissent transformation numérique pour PME,
      sites web rapides sur GitHub Pages, workflows IA,
      expérimentations TI et optimisation Business 2.0 appliquée au terrain.
    </p>
    <a href="#projects" class="card-link">Voir le projet</a>
  </article>

</section>

<!-- 🔥 Ton contenu one-page actuel -->
<section id="business" class="section">
  <h2>Business 2.0</h2>
  <p class="section-lead">
    Business 2.0, c’est ma façon d’utiliser la technologie pour aider des petites entreprises réelles,
    sans usines à gaz ni buzzwords inutiles.
  </p>
  <p>
    La plupart des PME n’ont pas besoin d’un nouveau “gros système”. Elles ont besoin de
    <strong>clarifier leurs processus</strong>, de réduire le travail répétitif et de mieux voir
    ce qui se passe dans leur entreprise. On part donc de la réalité : atelier, comptoir,
    courriels, fichiers Excel, conversation avec les clients.
  </p>
  <ul>
    <li><strong>Comprendre le terrain</strong> : comment le travail se fait aujourd’hui, pas en théorie.</li>
    <li><strong>Alléger avant d’ajouter</strong> : enlever la friction et le bruit avant d’ajouter de nouveaux outils.</li>
    <li><strong>Automatiser là où ça compte</strong> : seulement si ça sauve réellement du temps ou diminue le risque.</li>
    <li><strong>Utiliser l’IA comme assistant</strong> : pour le contenu, la doc, les décisions, pas pour remplacer les humains.</li>
    <li><strong>Mesurer l’impact</strong> : temps gagné, erreurs réduites, clients mieux servis.</li>
  </ul>
  <p>
    Tout ce que je teste finit tôt ou tard dans un projet concret — souvent chez des commerces locaux
    comme ceux présentés ci-dessous.
  </p>
</section>

**
<section id="projects" class="section">
  <h2>Projets</h2>
  <p class="section-lead">
    Quelques projets concrets où j’applique Business 2.0, TI, web et IA.
  </p>

  <section class="projects-grid">

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Business 2.0 · Commerce local</span>
        <h3 class="project-card-title"><a href="https://chezgerry1958.com">Chez Gerry 1958</a></h3>
        <p class="project-card-meta">Cordonnerie haut de gamme · Gatineau</p>
      </div>
      <p class="project-card-desc">Site web, SEO, contenu avant/après et automatisation légère.</p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Site statique</span>
        <h3 class="project-card-title"><a href="https://chucks-casse-croute.com">Chuck’s Casse-Croute</a></h3>
        <p class="project-card-meta">Vitrine légère · GitHub Pages</p>
      </div>
      <p class="project-card-desc">Site rapide, simple, sans CMS pour un casse-croûte local.</p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">E-commerce</span>
        <h3 class="project-card-title"><a href="https://web.archive.org/...">Pronatureqc.com (2015–2018)</a></h3>
        <p class="project-card-meta">Boutique en ligne · Archive</p>
      </div>
      <p class="project-card-desc">Catalogue massif, SEO, paiement sécurisé.</p>
    </article>

    <article class="project-card">
      <div class="project-card-header">
        <span class="project-badge">Consultation TI</span>
        <h3 class="project-card-title"><a href="https://web.archive.org/...">Assystech SENC</a></h3>
        <p class="project-card-meta">Dév. Web · Infra</p>
      </div>
      <p class="project-card-desc">Support et optimisation TI pour PME.</p>
    </article>

  </section>
</section>**

<section id="blog" class="section">
  <h2>Blog</h2>
  <p class="section-lead">Derniers articles en français.</p>

  <div class="latest-posts-grid">
    {% assign posts_fr = site.posts | where: "lang", "fr" | sort: "date" | reverse %}
    {% for post in posts_fr limit:3 %}
      <article class="post-card">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="post-card-meta">{{ post.date | date: "%Y-%m-%d" }}</p>
        <p class="post-card-excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
      </article>
    {% endfor %}
  </div>

  <p class="section-more"><a href="/fr/blog/">Voir tous les articles →</a></p>
</section>

<section id="contact" class="section section-contact">
  <h2>Contact</h2>
  <p class="section-lead">
    Vous avez une idée ou un projet, mais vous ne savez pas par où commencer ?
  </p>
  <p>
    Je m’intéresse particulièrement aux petites entreprises, aux projets locaux et aux équipes
    qui veulent moderniser leurs opérations sans perdre leur identité. On peut commencer par
    une simple discussion pour clarifier votre contexte.
  </p>
  <ul>
    <li>📧 Courriel : <a href="mailto:contact@jphenri.ca">contact@jphenri.ca</a></li>
    <li>🔗 LinkedIn : (ajoutez votre lien ici)</li>
  </ul>
  <p>
    Vous n’avez pas besoin d’un cahier de charges complet. Quelques lignes sur qui vous êtes,
    ce que vous faites et ce qui bloque en ce moment suffisent pour démarrer.
  </p>
</section>

