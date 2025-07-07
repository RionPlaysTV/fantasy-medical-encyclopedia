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
        <p><strong>Lifespan:</strong> {{ species.lifespan }}</p>
      {% endif %}
      <p>{{ species.excerpt | strip_html | truncatewords: 25 }}</p>
      <a href="{{ species.url | relative_url }}" class="read-more">Read Full Entry →</a>
    </div>
  {% endfor %}
</div>

## 🔍 Quick Reference Guide

### By Lifespan
- **Short-lived (Under 100 years):** Humans, Goblins, Orcs
- **Medium-lived (100-500 years):** Dwarves, Halflings
- **Long-lived (500+ years):** Elves, Fae, Dragons

### By Magical Sensitivity
- **High Sensitivity:** Elves, Fae, Angels
- **Moderate Sensitivity:** Humans, Beastkin
- **Low Sensitivity:** Dwarves, Orcs
- **Variable Sensitivity:** Dragons, Demons

### Emergency Treatment Priorities
1. **Iron Sensitivity:** Elves, Fae
2. **High Dosage Requirements:** Dwarves, Giants, Orcs  
3. **Magical Interaction Risks:** Dragons, Demons, Angels
4. **Crossbreeding Complications:** All hybrid species

## 📖 Using This Archive

Each species entry follows a standardized format for quick reference:
- **Lifespan & Physical Characteristics**
- **Cardiovascular & Respiratory Systems**
- **Common Ailments & Vulnerabilities**
- **Magical Anomalies & Adaptations**
- **Healing Response Protocols**
- **Crossbreeding Medical Notes**
- **Known Allergies & Toxins**
- **Cultural Medical Practices**
- **Clinical Observations & Emergency Protocols**

---

*For emergency situations, refer to the individual species emergency protocols. When in doubt, begin with minimal magical intervention and observe patient response.*

<style>
.species-index {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.index-entry {
  border: 1px solid #e1e5e9;
  padding: 1.5rem;
  border-radius: 8px;
  background: #fff;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.index-entry h3 {
  margin-top: 0;
  color: #0366d6;
}

.index-entry h3 a {
  text-decoration: none;
  color: inherit;
}

.index-entry h3 a:hover {
  text-decoration: underline;
}

.read-more {
  display: inline-block;
  margin-top: 1rem;
  padding: 0.5rem 1rem;
  background: #f1f3f4;
  text-decoration: none;
  border-radius: 4px;
  font-size: 0.9rem;
}

.read-more:hover {
  background: #e1e5e9;
}
</style>
