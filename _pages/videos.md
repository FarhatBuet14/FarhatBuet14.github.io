---
title: "Videos"
permalink: /videos/
---

<style>
/* Page container */
.v-wrap{
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 1rem;
}

/* Headings */
.v-wrap h2{
  margin: 0 0 .35rem 0;
}
.v-wrap p.lead{
  margin: 0 0 1rem 0;
  opacity: .95;
  line-height: 1.6;
}

/* Grid */
.v-grid{
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.1rem;
  margin: 1rem 0 2rem;
}

/* Card */
.v-card{
  border: 1px solid rgba(255,255,255,.14);
  border-radius: 16px;
  background: rgba(0,0,0,.12);
  overflow: hidden;

  /* Performance */
  content-visibility: auto;
  contain-intrinsic-size: 420px;
}

/* Video preview area */
.v-thumb{
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 9;
  background: rgba(255,255,255,.06);
  display: grid;
  place-items: center;
  cursor: pointer;
}

/* Thumbnail image as background */
.v-thumb[data-yt]{
  background-size: cover;
  background-position: center;
}

/* Play button */
.v-play{
  width: 64px;
  height: 64px;
  border-radius: 999px;
  border: 1px solid rgba(255,255,255,.25);
  background: rgba(0,0,0,.35);
  display: grid;
  place-items: center;
  backdrop-filter: blur(6px);
}
.v-play svg{
  width: 22px;
  height: 22px;
  transform: translateX(1px);
}

/* Caption */
.v-body{
  padding: .95rem 1rem 1rem;
}
.v-title{
  font-weight: 800;
  line-height: 1.25;
  margin: 0 0 .25rem 0;
}
.v-meta{
  opacity: .86;
  font-size: .95rem;
  margin: 0 0 .6rem 0;
}
.v-caption{
  opacity: .95;
  line-height: 1.55;
  margin: 0;
}

/* Mobile */
@media (max-width: 980px){
  .v-grid{ grid-template-columns: repeat(2, minmax(0, 1fr)); }
}
@media (max-width: 640px){
  .v-grid{ grid-template-columns: 1fr; }
}

/* Reduced motion */
@media (prefers-reduced-motion: reduce){
  .v-thumb{ transition: none; }
}
</style>

<div class="v-wrap">

<h2>Videos</h2>
<p class="lead">
A curated set of videos covering my research projects and a few personal travel moments—because I like exploring the world the same way I like exploring ideas.
</p>

---

<h2>Projects & Research</h2>
<p class="lead">Demos, talks, and media clips related to my work in computer vision and edge-to-cloud AI systems.</p>

<div class="v-grid">

  <!-- Example: you can keep this one (it’s public and already available) -->
  <div class="v-card">
    <div class="v-thumb" data-yt="998C99xx0J8" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Boundless Bulls — AI for Mosquito Surveillance (Interview)</div>
      <div class="v-meta">Media clip • Project spotlight</div>
      <p class="v-caption">A short feature on using AI to support mosquito monitoring and public-health surveillance.</p>
    </div>
  </div>

  <!-- Replace VIDEO_ID_xxx with your real YouTube video IDs -->
  <div class="v-card">
    <div class="v-thumb" data-yt="yvbThD835m0" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">MosquitoAI — Project Demo</div>
      <div class="v-meta">Demo • Year</div>
      <p class="v-caption">Short walkthrough of the pipeline, outputs, and how the system supports monitoring workflows.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="GEpUhzFNl2w" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Edge-to-Cloud Smart Trap — System Overview</div>
      <div class="v-meta">Demo • Year</div>
      <p class="v-caption">Edge capture + cloud processing overview, showing the end-to-end flow from device to analytics.</p>
    </div>
  </div>

</div>

---

<h2>Travel & Life</h2>
<p class="lead">Travel clips—driving, nature, rain, and small moments that remind me life is an adventure.</p>

<div class="v-grid">

  <div class="v-card">
    <div class="v-thumb" data-yt="VIDEO_ID_TRAVEL_1" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Solo drive & exploring new places</div>
      <div class="v-meta">Travel • Year</div>
      <p class="v-caption">A quiet reminder that showing up for yourself is also progress.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="VIDEO_ID_TRAVEL_2" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Rain, roads, and calm</div>
      <div class="v-meta">Travel • Year</div>
      <p class="v-caption">The kind of weather that makes everything feel slower—in a good way.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="VIDEO_ID_TRAVEL_3" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Nature reset: beach / mountain moments</div>
      <div class="v-meta">Travel • Year</div>
      <p class="v-caption">Clips from nature that keep me grounded and curious.</p>
    </div>
  </div>

</div>

</div>

<script>
/*
  Lightweight YouTube: show thumbnail first, load iframe only on click.
  This keeps scrolling fast on desktop + mobile.
*/
(function(){
  const thumbs = document.querySelectorAll('.v-thumb[data-yt]');
  thumbs.forEach(el => {
    const id = el.getAttribute('data-yt');
    if (!id || id.startsWith('VIDEO_ID_')) {
      // Still render a neutral background for placeholders
      el.style.background = 'rgba(255,255,255,.06)';
      el.innerHTML = '<div class="v-play" aria-hidden="true">' +
        '<svg viewBox="0 0 24 24" fill="currentColor"><path d="M8 5v14l11-7z"/></svg>' +
      '</div>';
      return;
    }

    // Set thumbnail background
    el.style.backgroundImage = `url(https://i.ytimg.com/vi/${id}/hqdefault.jpg)`;
    el.innerHTML = '<div class="v-play" aria-hidden="true">' +
      '<svg viewBox="0 0 24 24" fill="currentColor"><path d="M8 5v14l11-7z"/></svg>' +
    '</div>';

    // Click -> replace with iframe
    el.addEventListener('click', () => {
      const iframe = document.createElement('iframe');
      iframe.width = "560";
      iframe.height = "315";
      iframe.style.width = "100%";
      iframe.style.height = "100%";
      iframe.style.border = "0";
      iframe.setAttribute('allowfullscreen', '');
      iframe.setAttribute('loading', 'lazy');
      iframe.setAttribute('referrerpolicy', 'strict-origin-when-cross-origin');
      iframe.setAttribute('allow', 'accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share');
      iframe.src = `https://www.youtube-nocookie.com/embed/${id}?autoplay=1&rel=0`;

      el.innerHTML = '';
      el.style.backgroundImage = 'none';
      el.appendChild(iframe);
      el.style.cursor = 'auto';
    }, { once: true });
  });
})();
</script>
