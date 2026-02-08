---
title: ""
permalink: /press/
layout: hero-page
---

<style>
/* =========================
   Press page styles (scoped)
   Only applies inside #press-page
   ========================= */

#press-page { max-width: 1100px; margin: 0 auto; }

#press-page .press-grid{
  display:grid;
  grid-template-columns: repeat(2, minmax(0,1fr));
  gap: 18px;
  margin: 14px 0 26px 0;
}
@media (max-width: 900px){
  #press-page .press-grid{ grid-template-columns: 1fr; }
}

/* Card */
#press-page .press-card{
  display:flex;
  gap:16px;
  padding:16px;
  border-radius:16px;
  text-decoration:none !important;

  border: 1px solid rgba(255,255,255,0.10);
  background: rgba(0,0,0,0.28);

  transition: transform .14s ease, border-color .14s ease;

  /* Performance */
  content-visibility: auto;
  contain-intrinsic-size: 260px;
}

#press-page .press-card:hover{
  transform: translateY(-2px);
  border-color: rgba(255,255,255,0.22);
}

/* Ensure ONLY the title is blue; everything else is white/neutral */
#press-page .press-card,
#press-page .press-card *{
  color: rgba(255,255,255,0.92) !important;
}

#press-page .press-title{
  color: #77b8ff !important;     /* blue only for title */
  font-weight: 800;
  font-size: 1.05rem;
  line-height: 1.25;
  margin: 0 0 8px 0;
}
#press-page .press-card:hover .press-title{
  text-decoration: underline;
}

/* Kicker + description */
#press-page .press-kicker{
  font-size: 0.85rem;
  opacity: 0.78;
  margin-bottom: 6px;
}
#press-page .press-desc{
  opacity: 0.92;
  line-height: 1.55;
  margin: 0;
}

/* Thumb for video cards */
#press-page .press-thumb{
  width: 220px;
  max-width: 40%;
  border-radius: 12px;
  object-fit: cover;
  flex: 0 0 auto;
}
@media (max-width: 900px){
  #press-page .press-thumb{ width: 160px; }
}

/* Footer links row */
#press-page .press-links{
  display:flex;
  align-items:center;
  gap:10px;
  margin-top: 10px;
  opacity: 0.95;
}
#press-page .press-favicon img{
  width:18px;
  height:18px;
  border-radius:4px;
}
#press-page .press-link{
  font-weight: 700;
  text-decoration: underline;
}

/* Optional: tighten headings a bit */
#press-page h2{
  font-weight: 900;
  letter-spacing: 0.01em;
}
#press-page hr{
  border: 0;
  border-top: 1px solid rgba(255,255,255,0.18);
  margin: 16px 0 18px;
}
</style>

<div id="press-page">

## Press

Selected media coverage and features of my research on deployable AI systems for mosquito surveillance, smart trapping, and citizen-science–powered detection.

---

## Featured

<div class="press-grid">

  <a class="press-card press-card--video" href="https://www.youtube.com/watch?v=998C99xx0J8" target="_blank" rel="noopener">
    <img class="press-thumb" loading="lazy" decoding="async"
      src="https://i.ytimg.com/vi/998C99xx0J8/hqdefault.jpg"
      alt="USF Boundless Bulls — Farhat Azam">
    <div class="press-meta">
      <div class="press-kicker">Video • USF “Boundless Bulls”</div>
      <div class="press-title">Farhat Azam is using artificial intelligence to help fight mosquito-borne illnesses</div>
      <p class="press-desc">A profile feature on the motivation and impact behind my work on AI-enabled mosquito surveillance and smart trapping.</p>
      <div class="press-links"><span class="press-link">Watch</span></div>
    </div>
  </a>

  <a class="press-card" href="https://www.usf.edu/news/2025/how-a-usf-students-personal-battle-with-dengue-helped-develop-mosquito-fighting-ai.aspx" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Article • USF News (Jul 28, 2025)</div>
      <div class="press-title">How a USF student's personal battle with dengue helped develop mosquito-fighting AI</div>
      <p class="press-desc">USF News story highlighting the real-world motivation, technical direction, and public-health goals of my research.</p>
      <div class="press-links">
        <span class="press-favicon">
          <img loading="lazy" decoding="async" alt="USF"
               src="https://www.google.com/s2/favicons?domain=usf.edu&sz=64">
        </span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

</div>

---

## 2025

<div class="press-grid">

  <a class="press-card" href="https://www.eurekalert.org/news-releases/1103336" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Press release • EurekAlert (Oct 28, 2025)</div>
      <div class="press-title">USF study: AI and citizen science reveal potential first detection of invasive malaria mosquito in Madagascar</div>
      <p class="press-desc">Coverage of our work showing how AI + citizen-science imagery can accelerate detection of invasive malaria vectors.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="EurekAlert" src="https://www.google.com/s2/favicons?domain=eurekalert.org&sz=64"></span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

  <a class="press-card" href="https://phys.org/news/2025-10-ai-citizen-science-reveal-potential.html" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Article • Phys.org (Oct 28, 2025)</div>
      <div class="press-title">AI and citizen science reveal potential first detection of invasive malaria mosquito in Madagascar</div>
      <p class="press-desc">An overview of how smartphone imagery and trained models can support early-warning surveillance.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="Phys.org" src="https://www.google.com/s2/favicons?domain=phys.org&sz=64"></span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

  <a class="press-card" href="https://www.miragenews.com/ai-citizen-science-detect-invasive-malaria-1559231/" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Media pickup • Mirage News (Oct 29, 2025)</div>
      <div class="press-title">AI, Citizen Science Detect Invasive Malaria Mosquito</div>
      <p class="press-desc">International pickup emphasizing the public-health relevance of rapid, scalable, image-based vector surveillance.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="Mirage News" src="https://www.google.com/s2/favicons?domain=miragenews.com&sz=64"></span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

  <a class="press-card" href="https://bioengineer.org/ai-and-citizen-science-team-up-to-spot-potential-first-invasive-malaria-mosquito-in-madagascar-finds-usf-study/" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Media pickup • Bioengineer.org (Oct 28, 2025)</div>
      <div class="press-title">AI and Citizen Science Team Up to Spot Potential First Invasive Malaria Mosquito in Madagascar</div>
      <p class="press-desc">Summary coverage highlighting a citizen science + AI workflow and its role in scaling detection globally.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="Bioengineer" src="https://www.google.com/s2/favicons?domain=bioengineer.org&sz=64"></span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

  <a class="press-card press-card--video" href="https://www.youtube.com/watch?v=xwTDBe2VI34" target="_blank" rel="noopener">
    <img class="press-thumb" loading="lazy" decoding="async"
      src="https://i.ytimg.com/vi/xwTDBe2VI34/hqdefault.jpg"
      alt="Video coverage">
    <div class="press-meta">
      <div class="press-kicker">Video • Feature</div>
      <div class="press-title">Scientists use AI in the fight against mosquito-borne diseases</div>
      <p class="press-desc">Video coverage of AI-enabled smart trapping and its role in improving speed and precision of vector monitoring.</p>
      <div class="press-links"><span class="press-link">Watch</span></div>
    </div>
  </a>

</div>

---

## 2024

<div class="press-grid">

  <a class="press-card" href="https://baynews9.com/fl/tampa/news/2024/06/18/usf-mosquito-smart-trap" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Local news • Spectrum Bay News 9 (Jun 18, 2024)</div>
      <div class="press-title">USF researchers develop mosquito “smart trap” to help fight malaria</div>
      <p class="press-desc">Coverage highlighting the motivation, concept, and public-health direction of the smart mosquito trap effort.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="Bay News 9" src="https://www.google.com/s2/favicons?domain=baynews9.com&sz=64"></span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

  <a class="press-card" href="https://www.usf.edu/news/2024/usf-using-ai-to-help-combat-malaria-in-africa.aspx" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Article • USF News (Jun 6, 2024)</div>
      <div class="press-title">USF using AI to help combat malaria in Africa</div>
      <p class="press-desc">USF News overview of AI-driven mosquito surveillance and the broader research direction supporting malaria monitoring.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="USF" src="https://www.google.com/s2/favicons?domain=usf.edu&sz=64"></span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

  <a class="press-card" href="https://www.tampabay28.com/news/region-hillsborough/usf-researchers-use-ai-to-track-mosquito-borne-illness" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Local news • Tampa Bay 28</div>
      <div class="press-title">USF researchers use AI to track mosquito-borne illness</div>
      <p class="press-desc">Local coverage of AI-enabled vector monitoring and the value of automated identification for public-health response.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="Tampa Bay 28" src="https://www.google.com/s2/favicons?domain=tampabay28.com&sz=64"></span>
        <span class="press-link">Read</span>
      </div>
    </div>
  </a>

</div>

---

## Social

<div class="press-grid">
  <a class="press-card" href="https://www.facebook.com/reel/1666291457348510" target="_blank" rel="noopener">
    <div class="press-meta">
      <div class="press-kicker">Social • Facebook Reel</div>
      <div class="press-title">Research feature clip</div>
      <p class="press-desc">Short-form clip highlighting the smart mosquito trap and AI-based detection workflow.</p>
      <div class="press-links">
        <span class="press-favicon"><img loading="lazy" decoding="async" alt="Facebook" src="https://www.google.com/s2/favicons?domain=facebook.com&sz=64"></span>
        <span class="press-link">Open</span>
      </div>
    </div>
  </a>
</div>

</div>
