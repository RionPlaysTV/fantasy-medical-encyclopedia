---
layout: default
title: "Species Index"
---

# 📚 Complete Species Index

Welcome to the comprehensive index of species documented in the Anatomica Fantastica archives. Each entry provides detailed medical, physiological, and cultural healing information essential for practitioners treating multispecies populations.

## 🧑‍⚕️ Core Humanoid Species

<div class="species-index">
  {% for species in site.species %}
    {% assign species_title = species.title | downcase %}
    {% unless species_title contains 'beastkin' or species_title contains 'dragon' or species_title contains 'troll' %}
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
    {% endunless %}
  {% endfor %}
</div>

## 🐾 Beastkin Species

*Therianthropic humanoids with animal characteristics and dual-nature physiology*

<div class="species-index">
  {% for species in site.species %}
    {% assign species_title = species.title | downcase %}
    {% if species_title contains 'beastkin' %}
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
    {% endif %}
  {% endfor %}
</div>

### Beastkin Subspecies by Type

<div class="quick-reference">
  <ul>
    <li><strong>🐱 Feline Beastkin:</strong> Cat-based subspecies with enhanced reflexes, night vision, and territorial behaviors</li>
    <li><strong>🐺 Canine Beastkin:</strong> Wolf and dog-based subspecies with pack dynamics and loyalty-based healing</li>
    <li><strong>🐻 Ursine Beastkin:</strong> Bear-based subspecies with seasonal hibernation and massive strength adaptations</li>
    <li><strong>🦅 Avian Beastkin:</strong> Bird-based subspecies with flight capabilities and altitude-specific physiology</li>
    <li><strong>🐍 Reptilian Beastkin:</strong> Reptile-based subspecies with temperature-dependent metabolism and regenerative healing</li>
  </ul>
</div>

## 🐲 Ancient Creatures & Monsters

*Powerful magical beings requiring specialized medical approaches*

<div class="species-index">
  {% for species in site.species %}
    {% assign species_title = species.title | downcase %}
    {% if species_title contains 'dragon' or species_title contains 'troll' %}
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
    {% endif %}
  {% endfor %}
</div>

## 🔍 Quick Medical Reference Guide

<div class="quick-reference">
  <h4>By Lifespan Categories</h4>
  <ul>
    <li><strong>Short-lived (Under 100 years):</strong> Humans, Orcs, Most Beastkin (60-120 years)</li>
    <li><strong>Medium-lived (100-500 years):</strong> Dwarves, Avian Beastkin (80-150 years), Trolls (200-400 years)</li>
    <li><strong>Long-lived (500+ years):</strong> Elves, Reptilian Beastkin (150-300 years)</li>
    <li><strong>Ancient (1000+ years):</strong> Dragons (1000-5000 years)</li>
    <li><strong>Immortal:</strong> Fae, Dragons (conditional immortality)</li>
  </ul>

  <h4>By Magical Sensitivity</h4>
  <ul>
    <li><strong>Reality-Altering:</strong> Dragons, Fae</li>
    <li><strong>High Sensitivity:</strong> Elves, Fae, Avian Beastkin</li>
    <li><strong>Moderate Sensitivity:</strong> Humans, Most Beastkin</li>
    <li><strong>Low Sensitivity:</strong> Dwarves, Orcs</li>
    <li><strong>Magical Resistance:</strong> Trolls (regeneration-based), Dragons (ancient immunity)</li>
  </ul>

  <h4>Special Physiological Considerations</h4>
  <ul>
    <li><strong>Temperature-Dependent:</strong> Reptilian Beastkin (require 75-80°F), Ice Trolls (cold-adapted)</li>
    <li><strong>Transformation Capable:</strong> All Beastkin subspecies, some advanced magical humanoids</li>
    <li><strong>Regenerative:</strong> Trolls (advanced), Reptilian Beastkin (limited), Dragons (magical)</li>
    <li><strong>Pack/Social Dependent:</strong> Canine Beastkin, some Troll subspecies</li>
    <li><strong>Seasonal Cycles:</strong> Ursine Beastkin (hibernation), Avian Beastkin (migration), Forest Trolls</li>
  </ul>

  <h4>Critical Vulnerabilities</h4>
  <ul>
    <li><strong>Fire Vulnerability:</strong> ALL Troll subspecies (permanent damage), Avian Beastkin (panic response)</li>
    <li><strong>Iron Sensitivity:</strong> Elves, Fae - Remove all iron instruments immediately</li>
    <li><strong>Cold Vulnerability:</strong> Reptilian Beastkin (hypothermia risk below 60°F)</li>
    <li><strong>Toxic Substances:</strong> Chocolate (Canine/Feline Beastkin), Valerian (Feline)</li>
    <li><strong>Magical Disruption:</strong> Beastkin transformation states, Dragon magical fields</li>
  </ul>

  <h4>Dosage Adjustments Required</h4>
  <ul>
    <li><strong>Massive Increase (500-1000x):</strong> Dragons</li>
    <li><strong>High Increase (200-300%):</strong> Avian Beastkin, Large Troll subspecies</li>
    <li><strong>Moderate Increase (150-200%):</strong> Orcs, Most Beastkin, Mountain Trolls</li>
    <li><strong>Standard Increase (125-150%):</strong> Dwarves</li>
    <li><strong>Temperature Dependent:</strong> Reptilian Beastkin (varies with body temperature)</li>
  </ul>

  <h4>Emergency Treatment Priorities</h4>
  <ul>
    <li><strong>🔥 FIRE PROTOCOLS:</strong> Immediate suppression for ALL Troll patients - fire damage is permanent</li>
    <li><strong>🌡️ TEMPERATURE CRITICAL:</strong> Maintain 75-80°F for Reptilian Beastkin - hypothermia is lethal</li>
    <li><strong>⚡ TRANSFORMATION EMERGENCY:</strong> Clear 10-foot radius around transforming Beastkin - never restrain</li>
    <li><strong>🐉 DRAGON APPROACH:</strong> Diplomatic contact before medical intervention - hostile dragons are unsurvivable</li>
    <li><strong>🧲 IRON REMOVAL:</strong> Elves, Fae - Remove all iron instruments immediately</li>
    <li><strong>🏥 PACK SEPARATION:</strong> Canidae Beastkin in crisis without pack presence - allow pack members</li>
    <li><strong>💊 TOXIC SUBSTANCES:</strong> Chocolate/Grapes (Canidae), Chocolate/Valerian (Felidae) - potentially fatal</li>
    <li><strong>🔮 MAGICAL CONSENT:</strong> Dragons, Fae, Advanced Beastkin - Obtain explicit consent before magical healing</li>
  </ul>
</div>

<div class="medical-alert critical">
  <strong>🚨 Emergency Protocol:</strong> When treating unknown or hybrid species, begin with minimal magical intervention and observe patient response. ALWAYS inquire about subspecies heritage, transformation status, pack bonds, territorial concerns, and known allergies before treatment. Fire suppression equipment should be available for all large creature treatment.
</div>

<div class="medical-alert warning">
  <strong>⚠️ Beastkin Transformation Protocol:</strong> If patient begins involuntary transformation during treatment:
  <br>1. Clear 10-foot minimum radius immediately
  <br>2. Speak in calm, low tones - avoid sudden movements  
  <br>3. Allow transformation to complete naturally
  <br>4. Reassess patient needs after transformation stabilizes
  <br>5. NEVER attempt to restrain or reverse active transformation
</div>

---

## 📋 Classification System Notes

**Threat Levels:**
- **Peaceful:** Generally non-aggressive, standard medical protocols
- **Territorial:** Aggressive when territory threatened, approach with cultural sensitivity
- **Dangerous:** Requires specialized safety protocols and expert handlers
- **Extremely Dangerous:** Life-threatening risk to medical staff, emergency protocols only

**Subspecies Notation:**
- Individual Beastkin subspecies pages contain detailed transformation protocols
- Troll subspecies vary significantly in territorial and environmental needs
- Dragon chromatic vs. metallic classifications affect treatment approach
- Hybrid species require consultation with multiple species protocols

*For detailed emergency protocols, transformation management, and species-specific treatment guidelines, refer to individual species medical profiles. When treating ancient creatures or unknown subspecies, consult the Transcendental Medical College emergency consultation service.*

**Archive Status:** Currently documenting 15+ species with 5+ Beastkin subspecies. Research ongoing for additional monster species including Griffins, Phoenixes, Unicorns, and planar entities.
