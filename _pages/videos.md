---
title: ""
permalink: /videos/
layout: hero-page
---

<style>
/* Layout */
.v-wrap{ max-width: 1100px; margin: 0 auto; padding: 0 1rem; }
.v-wrap h2{ margin: 0 0 .35rem 0; }
.v-wrap p.lead{ margin: 0 0 1rem 0; opacity: .95; line-height: 1.6; }

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

/* Thumbnail -> becomes iframe on click */
.v-thumb{
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 9;
  background: rgba(255,255,255,.06);
  display: grid;
  place-items: center;
  cursor: pointer;
}
.v-thumb[data-yt]{
  background-size: cover;
  background-position: center;
}

.v-play{
  width: 64px; height: 64px;
  border-radius: 999px;
  border: 1px solid rgba(255,255,255,.25);
  background: rgba(0,0,0,.35);
  display: grid;
  place-items: center;
  backdrop-filter: blur(6px);
}
.v-play svg{ width: 22px; height: 22px; transform: translateX(1px); }

/* Text */
.v-body{ padding: .95rem 1rem 1rem; }
.v-title{ font-weight: 800; line-height: 1.25; margin: 0 0 .25rem 0; }
.v-meta{ opacity: .86; font-size: .95rem; margin: 0 0 .6rem 0; }
.v-caption{ opacity: .95; line-height: 1.55; margin: 0; }

/* Mobile */
@media (max-width: 980px){ .v-grid{ grid-template-columns: repeat(2, minmax(0, 1fr)); } }
@media (max-width: 640px){ .v-grid{ grid-template-columns: 1fr; } }
</style>

<div class="v-wrap">

<!-- <h2>Videos</h2>
<p class="lead">
A curated set of research demos and project clips, plus a few travel moments—because I like exploring the world the same way I like exploring ideas.
</p>

--- -->

<h2>Projects & Research</h2>
<p class="lead">
Hardware/software demos, algorithm visualizations, and project prototypes from my engineering and research journey.
</p>

<div class="v-grid">

  <!-- Research / Projects -->
  <div class="v-card">
    <div class="v-thumb" data-yt="yvbThD835m0" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Heart Rate Monitoring with Emotion Detection using PPG &amp; GSR Sensors</div>
      <div class="v-meta">Sensing + signal processing • Prototype</div>
      <p class="v-caption">A wearable/portable sensing concept combining physiological signals to estimate heart rate and track emotion-related changes.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="GEpUhzFNl2w" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">PathFinder</div>
      <div class="v-meta">Robotics / navigation • Project demo</div>
      <p class="v-caption">A navigation-oriented prototype demonstrating planning and movement through an environment.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="SeunymHm4Ak" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Rescue BOT</div>
      <div class="v-meta">Robotics • Project prototype</div>
      <p class="v-caption">A robotics concept demo focused on assistive/rescue-style operation and control.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="XR9IUkZXSQk" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Plotting Electric Field Lines</div>
      <div class="v-meta">Numerical methods • Visualization</div>
      <p class="v-caption">A computational visualization project demonstrating field-line plotting for physics/electromagnetics concepts.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="qB2WqiHOQ8I" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Project Demo (Research / Engineering)</div>
      <div class="v-meta">Demo • Project clip</div>
      <p class="v-caption">A short project demonstration highlighting implementation details and results in a practical setup.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="Em0mEWKRr2I" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Four Wheeled Car Controlled by Hand Gesture</div>
      <div class="v-meta">Embedded systems • Control</div>
      <p class="v-caption">A gesture-controlled vehicle prototype demonstrating real-time sensing and control for motion commands.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="ywfBh0ipygg" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Project Demo (Research / Engineering)</div>
      <div class="v-meta">Demo • Project clip</div>
      <p class="v-caption">A project video showing a working system and key outputs from the implementation.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="0xPcVjBJbuc" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Vein Pattern Extraction from Gray Scaled Images</div>
      <div class="v-meta">Computer vision • Biometrics</div>
      <p class="v-caption">A vision pipeline for extracting vein patterns from imaging data, supporting authentication/biometric analysis.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="ptiaPZuCs8E" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Project Demo (Research / Engineering)</div>
      <div class="v-meta">Demo • Project clip</div>
      <p class="v-caption">A concise demo focused on implementation and outcomes, presented as a standalone project clip.</p>
    </div>
  </div>

</div>

---

<h2>Travel &amp; Life</h2>
<p class="lead">
Driving, nature, and places that feel like a reset—small moments that keep me grounded and curious.
</p>

<div class="v-grid">

  <!-- Travel -->
  <div class="v-card">
    <div class="v-thumb" data-yt="I4vOSdM8Y6o" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Smoky Mountains Road Trip (Summer 2023)</div>
      <div class="v-meta">Road trip • Nature</div>
      <p class="v-caption">My first planned road trip from Florida to the Smoky Mountains—an unforgettable, scenic adventure.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="dvGYAPHfppQ" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Drive with the song I love</div>
      <div class="v-meta">Road trip • Music + scenery</div>
      <p class="v-caption">A peaceful drive with a soundtrack I love—one of those “just keep going” moments.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="xxfXd-v3oOg" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Beautiful Drive through Sedona Mountains (Evening)</div>
      <div class="v-meta">Sedona • Scenic drive</div>
      <p class="v-caption">Evening light, mountains, and a quiet road—Sedona at its best.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="jXUvunDZ9X0" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Serene Waves at Fort De Soto Beach</div>
      <div class="v-meta">Florida • Beach</div>
      <p class="v-caption">A calming ocean moment—just waves, wind, and a mental reset.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="Ivyfxc5qF_c" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Magical View of the Utah Mountains from Utah Lake</div>
      <div class="v-meta">Utah • Nature</div>
      <p class="v-caption">Mountain reflections and open skies—one of those views that slows time down.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="Ob6HZ8SdBdk" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Travel Moment</div>
      <div class="v-meta">Travel • Short clip</div>
      <p class="v-caption">A quick travel clip from the road—capturing the mood more than the destination.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="SU99eVQviUs" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Travel Moment</div>
      <div class="v-meta">Travel • Short clip</div>
      <p class="v-caption">Another small adventure—driving, exploring, and collecting memories.</p>
    </div>
  </div>

  <div class="v-card">
    <div class="v-thumb" data-yt="FQLCfLEtnx4" role="button" aria-label="Play video"></div>
    <div class="v-body">
      <div class="v-title">Sylhet Tour Memories</div>
      <div class="v-meta">Memories • Travel</div>
      <p class="v-caption">A nostalgic travel memory—just laughter and the kind of joy that stays with you.</p>
    </div>
  </div>

</div>

</div>

<script>
/* Lightweight YouTube embeds:
   - Load only thumbnail while scrolling
   - Replace with iframe only on click
*/
(function(){
  const thumbs = document.querySelectorAll('.v-thumb[data-yt]');
  thumbs.forEach(el => {
    const id = el.getAttribute('data-yt');
    el.style.backgroundImage = `url(https://i.ytimg.com/vi/${id}/hqdefault.jpg)`;
    el.innerHTML = '<div class="v-play" aria-hidden="true">' +
      '<svg viewBox="0 0 24 24" fill="currentColor"><path d="M8 5v14l11-7z"/></svg>' +
    '</div>';

    el.addEventListener('click', () => {
      const iframe = document.createElement('iframe');
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
      el.style.cursor = 'auto';
      el.appendChild(iframe);
    }, { once: true });
  });
})();
</script>
