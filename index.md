---
layout: default
---

<div class="home">
  <div class="hero-section">
    <h2>🏥 Welcome to the Multispecies Medical Archive</h2>
    <p>A comprehensive medical encyclopedia documenting the anatomical, physiological, and magical healing properties of fantasy species across the multiverse. This archive serves as an essential reference for healers, physicians, researchers, and anyone involved in multispecies medical care.</p>
  </div>

  <div class="featured-species">
    <h3>📚 Featured Species Documentation</h3>
    <div class="species-grid">
      {% for species in site.species %}
        <div class="species-card">
          <h4><a href="{{ species.url | relative_url }}">{{ species.title }}</a></h4>
          {% if species.lifespan %}
            <div class="species-meta">
              🧬 <strong>Lifespan:</strong> {{ species.lifespan }}
            </div>
          {% endif %}
          <p>{{ species.excerpt | strip_html | truncatewords: 20 }}</p>
          <a href="{{ species.url | relative_url }}" class="read-more">View Medical Profile →</a>
        </div>
      {% endfor %}
    </div>
  </div>

  <div class="quick-reference">
    <h3>🔬 Quick Reference</h3>
    <ul>
      <li><strong>Species Count:</strong> {{ site.species.size }} documented species</li>
      <li><strong>Medical Standards:</strong> Transcendental Medical College approved</li>
      <li><strong>Emergency Protocols:</strong> Included in all species entries</li>
      <li><strong>Cultural Practices:</strong> Respectfully documented healing traditions</li>
    </ul>
  </div>

  <div class="medical-alert warning">
    <strong>⚠️ Medical Disclaimer:</strong> This archive is intended for educational and reference purposes. Always consult with qualified healers for actual treatment. Consider individual patient variations and respect cultural medical preferences.
  </div>
</div>
