---
layout: home
author_profile: true
title: "Welcome"
header:
  overlay_color: "#0a0a1a"
  overlay_filter: "0.7"
  overlay_image: "/assets/images/blog-banner.jpg"
---

<style>
/* ═══════════════════════════════════════════════════════════════════════════
   TECHNO THEME - Cyberpunk Neon Aesthetic
   ═══════════════════════════════════════════════════════════════════════════ */

.techno-hero {
  text-align: center;
  padding: 3rem 1rem;
  background: linear-gradient(135deg, #0a0a1a 0%, #1a1a2e 50%, #16213e 100%);
  border-radius: 20px;
  margin-bottom: 2.5rem;
  position: relative;
  overflow: hidden;
  box-shadow: 0 0 40px rgba(0, 255, 255, 0.15), inset 0 0 60px rgba(138, 43, 226, 0.05);
}

.techno-hero::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 2px,
    rgba(0, 255, 255, 0.03) 2px,
    rgba(0, 255, 255, 0.03) 4px
  );
  animation: scan 8s linear infinite;
  pointer-events: none;
}

@keyframes scan {
  0% { transform: translateY(0); }
  100% { transform: translateY(50%); }
}

.techno-hero h1 {
  font-family: 'Orbitron', 'Segoe UI', sans-serif;
  font-size: 2.8rem;
  font-weight: 900;
  background: linear-gradient(90deg, #00ffff, #ff00ff, #00ffff);
  background-size: 200% auto;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  animation: gradient-shift 3s ease infinite;
  margin-bottom: 0.8rem;
  text-shadow: 0 0 30px rgba(0, 255, 255, 0.5);
  letter-spacing: 4px;
}

@keyframes gradient-shift {
  0%, 100% { background-position: 0% center; }
  50% { background-position: 200% center; }
}

.techno-hero p {
  font-size: 1.1rem;
  color: #a0e7e5;
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto;
  letter-spacing: 1px;
}

.techno-divider {
  height: 2px;
  background: linear-gradient(90deg, transparent, #00ffff, #ff00ff, #00ffff, transparent);
  margin: 2.5rem 0;
  border-radius: 2px;
  box-shadow: 0 0 15px rgba(0, 255, 255, 0.4);
}

/* Grid System */
.nav-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

/* Card Design */
.nav-card {
  background: linear-gradient(145deg, #12122a 0%, #1a1a3e 100%);
  border: 1px solid rgba(0, 255, 255, 0.2);
  border-radius: 16px;
  padding: 1.8rem;
  position: relative;
  overflow: hidden;
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
}

.nav-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: linear-gradient(90deg, #00ffff, #ff00ff);
  opacity: 0;
  transition: opacity 0.3s ease;
}

.nav-card:hover {
  transform: translateY(-8px) scale(1.02);
  border-color: rgba(0, 255, 255, 0.5);
  box-shadow: 0 15px 40px rgba(0, 255, 255, 0.2), 0 0 30px rgba(138, 43, 226, 0.15);
}

.nav-card:hover::before {
  opacity: 1;
}

.nav-card h3 {
  font-family: 'Orbitron', 'Segoe UI', sans-serif;
  font-size: 1.3rem;
  color: #00ffff;
  margin-bottom: 1rem;
  display: flex;
  align-items: center;
  gap: 10px;
  letter-spacing: 2px;
}

.nav-card .icon {
  font-size: 1.5rem;
  filter: drop-shadow(0 0 8px currentColor);
}

.nav-card ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.nav-card li {
  margin: 0.6rem 0;
  padding-left: 1.2rem;
  position: relative;
}

.nav-card li::before {
  content: '▸';
  position: absolute;
  left: 0;
  color: #ff00ff;
  font-size: 0.8rem;
  transition: transform 0.2s ease;
}

.nav-card li:hover::before {
  transform: translateX(4px);
  color: #00ffff;
}

.nav-card a {
  color: #e0e0ff;
  text-decoration: none;
  font-size: 0.95rem;
  transition: all 0.3s ease;
  border-bottom: 1px solid transparent;
}

.nav-card a:hover {
  color: #00ffff;
  border-bottom-color: #00ffff;
  text-shadow: 0 0 10px rgba(0, 255, 255, 0.5);
}

/* Subcategory styling */
.nav-card .subcategory {
  margin-left: 0.8rem;
  padding-left: 1rem;
  border-left: 2px solid rgba(138, 43, 226, 0.4);
  margin-top: 0.5rem;
}

.nav-card .subcategory-title {
  color: #b388ff;
  font-weight: 600;
  font-size: 0.9rem;
  margin-bottom: 0.4rem;
}

/* Footer */
.techno-footer {
  text-align: center;
  margin-top: 3rem;
  padding: 2rem;
  background: linear-gradient(135deg, #0a0a1a 0%, #1a1a2e 100%);
  border-radius: 16px;
  border: 1px solid rgba(0, 255, 255, 0.15);
}

.techno-footer a {
  color: #00ffff;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
}

.techno-footer a:hover {
  color: #ff00ff;
  text-shadow: 0 0 15px rgba(255, 0, 255, 0.6);
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .techno-hero h1 { font-size: 2rem; letter-spacing: 2px; }
  .nav-grid { grid-template-columns: 1fr; }
  .nav-card { padding: 1.4rem; }
}

/* Import Orbitron font */
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&display=swap');
</style>

<div class="techno-hero">
  <h1>⚡ ABHINAV'S HUB ⚡</h1>
  <p>Exploring the intersection of Technology, Strategy, Mathematics, Music, Travel & Craftsmanship</p>
</div>

<div class="techno-divider"></div>

<div class="nav-grid">

  <div class="nav-card">
    <h3><span class="icon">🎓</span> ACADEMICS</h3>
    <ul>
      <li><a href="/academics/genaiforundergrads.html">GenAI for Undergrads</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">💻</span> TECHNOLOGY</h3>
    <ul>
      <li><a href="/tech/index.md">Tech Home</a></li>
      <li><a href="/tech/ai.md">Artificial Intelligence</a></li>
      <li><a href="/tech/cloud.md">Cloud Computing</a></li>
      <li><a href="/tech/legacy-modernization.md">Legacy Modernization</a></li>
      <li><a href="/tech/nvidiahealthcareusecases.html">NVIDIA Healthcare Use Cases</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">📊</span> INDUSTRY</h3>
    <ul>
      <li><a href="/industry/aistrategy.html">AI Strategy</a></li>
      <li><a href="/industry/bigbill.html">A Tale of Two Healthcare Bills</a></li>
      <li><a href="/industry/obbbaimpact.html">One Big Beautiful Bill Impact</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">🎯</span> STRATEGY</h3>
    <ul>
      <li><a href="/strategy/abdmimmunization.html">ABDM Immunization</a></li>
      <li><a href="/strategy/largemodernization.html">Large Modernization</a></li>
      <li><a href="/strategy/progressiveengineering.html">Progressive Engineering</a></li>
      <li class="subcategory-title">Organization</li>
      <div class="subcategory">
        <li><a href="/strategy/Org/enterprise_ontology_graph.html">Enterprise Ontology Graph</a></li>
        <li><a href="/strategy/Org/org_strugture.html">Organization Structure</a></li>
      </div>
      <li class="subcategory-title">AI Workstation</li>
      <div class="subcategory">
        <li><a href="/strategy/AIWorkstation/budgetworkstation.html">Budget Analysis</a></li>
        <li><a href="/strategy/AIWorkstation/workstation-guide.html">Workstation Guide</a></li>
      </div>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">📝</span> CHEATSHEETS</h3>
    <ul>
      <li><a href="/cheatsheets/mlmodels.html">ML Models Reference</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">🧪</span> PROTOTYPES</h3>
    <ul>
      <li><a href="/prototypes/lab-admin-portal.html">Lab Admin Portal</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">🔬</span> SAMPLES</h3>
    <ul>
      <li><a href="/samples/agent.html">Agent Demo</a></li>
      <li><a href="/samples/spikes.html">Spikes</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">📖</span> STORIES</h3>
    <ul>
      <li><a href="/stories/theaibiryanifactory.html">The AI Biryani Factory</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">➕</span> MATHEMATICS</h3>
    <ul>
      <li><a href="/mathematics/index.md">Mathematics Home</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">🎵</span> MUSIC</h3>
    <ul>
      <li><a href="/music/index.md">Music Home</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">✈️</span> TRAVEL</h3>
    <ul>
      <li><a href="/travel/index.md">Travel Adventures</a></li>
    </ul>
  </div>

  <div class="nav-card">
    <h3><span class="icon">🪚</span> CARPENTRY</h3>
    <ul>
      <li><a href="/carpentry/index.md">Woodworking Projects</a></li>
    </ul>
  </div>

</div>

<div class="techno-divider"></div>

<div class="techno-footer">
  <p>🗺️ <a href="/sitemap.html">View Full Site Map</a></p>
</div>