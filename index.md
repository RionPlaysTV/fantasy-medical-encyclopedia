---
layout: default
---

<div class="home">
  <h1 class="page-heading">{{ site.title }}</h1>
  
  <div class="hero-section">
    <h2>🏥 Welcome to the Multispecies Medical Archive</h2>
    <p>A comprehensive medical encyclopedia documenting the anatomical, physiological, and magical healing properties of fantasy species across the multiverse.</p>
  </div>

  <div class="featured-species">
    <h3>📚 Browse by Species</h3>
    <div class="species-grid">
      {% for species in site.species %}
        <div class="species-card">
          <h4><a href="{{ species.url | relative_url }}">{{ species.title }}</a></h4>
          <p>{{ species.excerpt | strip_html | truncatewords: 15 }}</p>
        </div>
      {% endfor %}
    </div>
  </div>

  <div class="quick-reference">
    <h3>🔬 Quick Reference</h3>
    <ul>
      <li><a href="{{ '/species/' | relative_url }}">Complete Species Index</a></li>
      <li><a href="{{ '/about/' | relative_url }}">About This Archive</a></li>
    </ul>
  </div>
</div>

<style>
.hero-section {
  background: #f8f9fa;
  padding: 2rem;
  border-radius: 8px;
  margin: 2rem 0;
  text-align: center;
}

.species-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1rem;
  margin: 1rem 0;
}

.species-card {
  border: 1px solid #ddd;
  padding: 1rem;
  border-radius: 6px;
  background: #fff;
}

.species-card h4 {
  margin-top: 0;
}

.quick-reference ul {
  list-style-type: none;
  padding: 0;
}

.quick-reference li {
  margin: 0.5rem 0;
  padding: 0.5rem;
  background: #f1f3f4;
  border-radius: 4px;
}
</style>
