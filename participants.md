---
layout: default
title: Participants
nav_order: 3
has_children: true
---

# Participants

Découvrez les participants de la Nuclear Haunted Cup #3 : Apocalypse.  
Chaque participant disposera de sa propre page avec ses informations, sa chaîne et sa présentation.  
Les profils seront ajoutés progressivement.

{% assign nhc_participants = site.pages | where: "parent", "Participants" | sort: "nav_order" %}

{% if nhc_participants.size > 0 %}
<div class="nhc-participant-grid">
{% for participant in nhc_participants %}
  <a class="nhc-participant-card" style="text-decoration: none; color: inherit;" href="{{ participant.url | relative_url }}" aria-label="Voir la fiche de {{ participant.title | escape }}">
    {% if participant.participant_image %}
    <img class="nhc-participant-card-image" src="{{ participant.participant_image | relative_url }}" alt="Avatar de {{ participant.title | escape }}">
    {% endif %}
    <div class="nhc-participant-card-body">
      <span class="nhc-participant-card-name">{{ participant.title }}</span>
      <span class="nhc-participant-card-status">NHC #3</span>
    </div>
  </a>
{% endfor %}
</div>
{% else %}
<div class="nhc-box nhc-pending nhc-reveal-waiting">
  <span class="nhc-box-title">Participants bientôt dévoilés</span>
  Les profils seront ajoutés progressivement.
</div>
{% endif %}
