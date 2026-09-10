---
layout: default
title: Accueil
nav_order: 1
---

<div class="nhc-hero">
  <div class="nhc-hero-content">
    <div class="nhc-hero-kicker">Nuclear Haunted Cup #3</div>
    <h1 class="nhc-hero-title">Apocalypse</h1>
    <p class="nhc-hero-subtitle">
      Règlement officiel du tournoi communautaire Phasmophobia organisé par Nuclear_Live.
      Retrouvez ici les règles, le déroulement, les participants et toutes les informations utiles avant le lancement.
    </p>

    <div class="nhc-tag-row">
      <span class="nhc-tag"><span class="nhc-tag-dot"></span> Phasmophobia</span>
      <span class="nhc-tag"><span class="nhc-tag-dot"></span> Édition #3</span>
      <span class="nhc-tag"><span class="nhc-tag-dot"></span> Thème Apocalypse</span>
    </div>
  </div>

  <div class="nhc-hero-logo-wrap">
    <img
      class="nhc-hero-logo"
      src="{{ '/logo-nuclear-live.png' | relative_url }}"
      alt="Logo Nuclear Live"
    >
  </div>

  <button class="nhc-trex" type="button" onclick="toggleTrexSound()" aria-label="T-Rex">
  <img src="{{ '/assets/downloads/trex.png' | relative_url }}" alt="">
</button>
</div>

<div class="nhc-actions">
  <a class="nhc-action" href="{{ '/reglement.html' | relative_url }}">Consulter le règlement</a>
  <a class="nhc-action nhc-action-secondary" href="{{ '/participants.html' | relative_url }}">Voir les participants</a>
  <a class="nhc-action nhc-action-secondary" href="{{ '/faq.html' | relative_url }}">FAQ</a>
  <a class="nhc-action nhc-action-secondary" href="https://www.twitch.tv/nuclear_live" target="_blank" rel="noopener noreferrer">Nuclear_Live</a>
</div>

<div class="nhc-section-title">Dossier tournoi</div>

<div class="nhc-info-grid">
  <div class="nhc-info-card">
    <span class="nhc-info-label">Date du tournoi</span>
    <span class="nhc-info-value">Samedi 7 novembre 2026</span>
  </div>

  <div class="nhc-info-card">
    <span class="nhc-info-label">Lancement officiel</span>
    <span class="nhc-info-value">21h00</span>
  </div>

  <div class="nhc-info-card">
    <span class="nhc-info-label">Version du règlement</span>
    <span class="nhc-info-value">2.0</span>
  </div>

  <div class="nhc-info-card">
    <span class="nhc-info-label">Dernière mise à jour</span>
    <span class="nhc-info-value">10/09/2026</span>
  </div>
</div>

<div class="nhc-section-title">Accès rapide</div>

<div class="nhc-link-grid">
  <a class="nhc-link-card" href="{{ '/deroulement-tournoi.html' | relative_url }}">
    <span class="nhc-link-icon">⌁</span>
    <span class="nhc-link-copy">
      <strong>Déroulement du tournoi</strong>
      <span>Format général, progression et fonctionnement des parties.</span>
    </span>
    <span class="nhc-link-arrow">›</span>
  </a>

  <a class="nhc-link-card" href="{{ '/calcul-points.html' | relative_url }}">
    <span class="nhc-link-icon">✦</span>
    <span class="nhc-link-copy">
      <strong>Calcul des points</strong>
      <span>Identification, objectifs, preuves, bonus et malus.</span>
    </span>
    <span class="nhc-link-arrow">›</span>
  </a>

  <a class="nhc-link-card" href="{{ '/elements-interdits.html' | relative_url }}">
    <span class="nhc-link-icon">⚠</span>
    <span class="nhc-link-copy">
      <strong>Éléments interdits</strong>
      <span>Glitchs, usebugs, aides extérieures et modifications visuelles.</span>
    </span>
    <span class="nhc-link-arrow">›</span>
  </a>

  <a class="nhc-link-card" href="{{ '/incidents-techniques.html' | relative_url }}">
    <span class="nhc-link-icon">⚙</span>
    <span class="nhc-link-copy">
      <strong>Incidents techniques</strong>
      <span>Procédure à suivre en cas de crash, coupure ou problème de partie.</span>
    </span>
    <span class="nhc-link-arrow">›</span>
  </a>
</div>

<div class="nhc-box nhc-important">
  <span class="nhc-box-title">Important</span>
  Le règlement est encore en cours de préparation.<br><br>
  Toute modification importante sera également annoncée sur le
  <a href="https://discord.com/invite/UE3cT4q" target="_blank" rel="noopener noreferrer">Discord officiel</a>.
</div>

<audio id="trex-sound" preload="auto">
  <source src="{{ '/assets/downloads/jurassic-park.mp3' | relative_url }}" type="audio/mpeg">
</audio>

<script>
function toggleTrexSound() {
  const sound = document.getElementById("trex-sound");

  if (sound.paused) {
    sound.currentTime = 0;
    sound.play();
  } else {
    sound.pause();
    sound.currentTime = 0;
  }
}
</script>
