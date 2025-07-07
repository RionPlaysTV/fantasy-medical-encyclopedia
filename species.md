---
layout: default
title: "Species Index"
---

---
layout: default
title: "Species Index"
---

# 📚 Complete Species Index

Welcome to the comprehensive index of species documented in the Anatomica Fantastica archives. Each entry provides detailed medical, physiological, and cultural healing information essential for practitioners treating multispecies populations.

## 🧑‍⚕️ Currently Documented Species

<div class="species-index">
  {% assign sorted_species = site.species | sort: 'title' %}
  {% for species in sorted_species %}
    <div class="index-entry">
      <h3><a href="{{ species.url | relative_url }}">{{ species.title }}</a></h3>
      {% if species.lifespan %}
        <div class="species-meta">
          🧬 <strong>Lifespan:</strong> {{ species.lifespan }}
        </div>
      {% endif %}
      <p>{{ species.excerpt | strip_html | truncatewords: 25 }}</p>
      <a href="{{ species.url | relative_url }}" class="read-more">Read Full Medical Profile →</a>
    </div>
  {% endfor %}
</div>

## 🔍 Quick Medical Reference Guide

<div class="quick-reference">
  <h4>By Lifespan Categories</h4>
  <ul>
    <li><strong>Short-lived (Under 100 years):</strong> Humans, Orcs</li>
    <li><strong>Medium-lived (100-500 years):</strong> Dwarves</li>
    <li><strong>Long-lived (500+ years):</strong> Elves</li>
    <li><strong>Immortal:</strong> Fae, Dragons (conditional)</li>
  </ul>

  <h4>By Magical Sensitivity</h4>
  <ul>
    <li><strong>High Sensitivity:</strong> Elves, Fae</li>
    <li><strong>Moderate Sensitivity:</strong> Humans</li>
    <li><strong>Low Sensitivity:</strong> Dwarves, Orcs</li>
    <li><strong>Reality-Altering:</strong> Dragons, Fae</li>
  </ul>

  <h4>Emergency Treatment Priorities</h4>
  <ul>
    <li><strong>Iron Sensitivity:</strong> Elves, Fae - Remove all iron instruments immediately</li>
    <li><strong>High Dosage Requirements:</strong> Dwarves (50% increase), Orcs (150% increase)</li>
    <li><strong>Magical Interaction Risks:</strong> Dragons, Fae - Obtain explicit consent before magical healing</li>
    <li><strong>Cultural Considerations:</strong> All species - Respect traditional healing practices</li>
  </ul>
</div>

<div class="medical-alert critical">
  <strong>🚨 Emergency Protocol:</strong> When treating unknown or hybrid species, begin with minimal magical intervention and observe patient response. Always inquire about species heritage and known allergies before treatment.
</div>

---

*For detailed emergency protocols and species-specific treatment guidelines, refer to individual species medical profiles. When in doubt, consult the Transcendental Medical College emergency hotline.*
