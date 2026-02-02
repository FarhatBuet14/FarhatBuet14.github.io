---
title: ""
permalink: /research/
---

<style>
/* Hide the auto title if your layout prints one */
.k-page-title { display: none !important; }

.research-wrap{
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 1rem;
}

/* One project card */
.proj{
  margin: 1.25rem 0;
  padding: 1.25rem;
  border-radius: 16px;
  border: 1px solid rgba(255,255,255,.14);
  background: rgba(0,0,0,.12);

  /* Performance: do less work until near viewport */
  content-visibility: auto;
  contain-intrinsic-size: 760px;
}

/* Top row: image + details (red box) */
.proj-top{
  display: grid;
  grid-template-columns: minmax(260px, 420px) 1fr 44px;
  gap: 1.25rem;
  align-items: center; /* key: vertically center image with the right text */
}

/* Image */
.proj-media{
  display: flex;
  align-items: center;   /* vertically center inside its column */
  justify-content: center; /* center horizontally within left column */
}

.proj-img{
  width: 100%;
  height: auto;
  max-height: 260px;  /* keeps it visually centered with the red area */
  object-fit: contain;
  display: block;
  border-radius: 12px;
  border: 1px solid rgba(255,255,255,.12);
  background: rgba(255,255,255,.04);
}

/* Right details text (red box content) */
.proj-title{
  margin: 0 0 .35rem 0;
  font-size: 1.5rem;
  line-height: 1.2;
}
.proj-meta{
  margin: 0 0 .75rem 0;
  opacity: .86;
  font-size: .98rem;
}
.proj-desc{
  margin: 0;
  opacity: .95;
  line-height: 1.55;
}

/* GitHub link column */
.proj-links{
  display: flex;
  align-items: flex-start;
  justify-content: center;
  padding-top: .1rem;
}

.proj-link{
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  border-radius: 10px;
  border: 1px solid rgba(255,255,255,.14);
  background: rgba(255,255,255,.06);
  text-decoration: none;
  transition: transform .12s ease, background .12s ease, border-color .12s ease;
}

.proj-link:hover{
  transform: translateY(-1px);
  background: rgba(255,255,255,.10);
  border-color: rgba(255,255,255,.22);
}

/* Bottom row: bullets span full width (blue box) */
.proj-bottom{
  margin-top: 1rem;
  padding-top: .75rem;
  border-top: 1px dashed rgba(255,255,255,.16);
}

.proj-bottom ul{
  margin: 0 0 0 1.1rem;
}

.proj-bottom li{
  margin: .45rem 0;
  line-height: 1.55;
}

/* Mobile */
@media (max-width: 900px){
  .proj-top{
    grid-template-columns: 1fr;
    align-items: start;
  }
  .proj-links{
    justify-content: flex-start;
  }
  .proj-img{
    max-height: 320px;
  }
}

/* Respect reduced motion */
@media (prefers-reduced-motion: reduce){
  .proj-link{ transition: none; }
}
</style>

<div class="research-wrap">

## Research

I build deployable computer vision and edge-to-cloud AI systems for real-world sensing, emphasizing robustness, scalability, and reliability. My work bridges model development and field deployment—designing end-to-end pipelines from data capture and processing to inference, monitoring, and human-in-the-loop validation.

---

## Selected projects

<!--
Put your images here (WebP):
assets/img/research/
- mosquitoai-dashboards.webp
- smart-trap-edge-to-cloud.webp
- valvular-heartsound.webp
- hand-vein-authentication.webp
-->

<!-- ================== PROJECT 1 ================== -->
<div class="proj">

  <div class="proj-top">

    <div class="proj-media">
      <img class="proj-img"
           src="{{ '/assets/img/research/mosquitoai-dashboards.webp' | relative_url }}"
           alt="MosquitoAI dashboards"
           loading="lazy"
           decoding="async">
    </div>

    <div>
      <h3 class="proj-title">MosquitoAI — AI Dashboards for Mosquito Biology & Species Inference</h3>
      <p class="proj-meta">Jan 2021 – Present · Supervised by Dr. Sriram Chellappan · University of South Florida</p>
      <p class="proj-desc">
        End-to-end computer vision pipeline and interactive dashboards for mosquito surveillance, supporting species and biological inference from heterogeneous imagery.
      </p>
    </div>

    <div class="proj-links">
      <a class="proj-link" href="https://github.com/FarhatBuet14/mosquitoAI" target="_blank" rel="noopener" aria-label="GitHub repository">
        <svg width="18" height="18" viewBox="0 0 16 16" fill="currentColor" aria-hidden="true">
          <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38
          0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52
          -.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64
          -.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18
          1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56
          .82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2
          0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
        </svg>
      </a>
    </div>

  </div>

  <div class="proj-bottom">
    <ul>
      <li>Developed multi-task deep learning workflows across adult and larval stages for classification and biological inference.</li>
      <li>Established reproducible training, validation, and benchmarking procedures to support deployment-oriented performance.</li>
      <li>Integrated explainability outputs to support human verification and operational trust.</li>
      <li>Packaged results into dashboards designed for field partners and applied surveillance workflows.</li>
    </ul>
  </div>

</div>

<!-- ================== PROJECT 2 ================== -->
<div class="proj">

  <div class="proj-top">

    <div class="proj-media">
      <img class="proj-img"
           src="{{ '/assets/img/research/smart-trap-edge-to-cloud.webp' | relative_url }}"
           alt="Edge-to-cloud smart mosquito trap"
           loading="lazy"
           decoding="async">
    </div>

    <div>
      <h3 class="proj-title">Edge-to-Cloud Smart Mosquito Trap for Automated Vector Monitoring</h3>
      <p class="proj-meta">Apr 2023 – Present · Supervised by Dr. Sriram Chellappan · University of South Florida</p>
      <p class="proj-desc">
        Field-deployable sensing system that captures multi-focus imagery on-device and synchronizes data to the cloud for automated detection, analytics, and alerting.
      </p>
    </div>

    <div class="proj-links">
      <a class="proj-link" href="https://github.com/FarhatBuet14/Smart-AI-Mosquito-Trap" target="_blank" rel="noopener" aria-label="GitHub repository">
        <svg width="18" height="18" viewBox="0 0 16 16" fill="currentColor" aria-hidden="true">
          <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38
          0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52
          -.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64
          -.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18
          1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56
          .82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2
          0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
        </svg>
      </a>
    </div>

  </div>

  <div class="proj-bottom">
    <ul>
      <li>Designed an end-to-end pipeline from edge capture (multi-focus) to cloud storage, metadata logging, and model inference.</li>
      <li>Built automated workflows for extracting single-mosquito crops via localization and preparing training-ready datasets.</li>
      <li>Enabled scalable monitoring through standardized capture formats, metadata schemas, and deployment-ready processing.</li>
      <li>Implemented robust evaluation to quantify performance under real-world conditions (clutter, occlusion, domain shift).</li>
    </ul>
  </div>

</div>

<!-- ================== PROJECT 3 ================== -->
<div class="proj">

  <div class="proj-top">

    <div class="proj-media">
      <img class="proj-img"
           src="{{ '/assets/img/research/valvular-heartsound.webp' | relative_url }}"
           alt="Valvular disease classification from heartsound data"
           loading="lazy"
           decoding="async">
    </div>

    <div>
      <h3 class="proj-title">Valvular Disease Classification from Heartsound Data</h3>
      <p class="proj-meta">Feb 2020 – Jul 2020 · Supervised by Dr. Taufiq Hasan · Bangladesh University of Engineering and Technology</p>
      <p class="proj-desc">
        Computer-aided analysis of heartsound recordings for reliable cardiac abnormality detection under noise and sensor variability.
      </p>
    </div>

    <div class="proj-links">
      <a class="proj-link" href="https://github.com/FarhatBuet14/CepsNET" target="_blank" rel="noopener" aria-label="GitHub repository">
        <svg width="18" height="18" viewBox="0 0 16 16" fill="currentColor" aria-hidden="true">
          <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38
          0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52
          -.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64
          -.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18
          1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56
          .82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2
          0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
        </svg>
      </a>
    </div>

  </div>

  <div class="proj-bottom">
    <ul>
      <li>Developed preprocessing and feature pipelines for heartsound signals under real-world noise and acquisition variation.</li>
      <li>Trained and benchmarked deep classifiers for abnormality detection across multiple datasets.</li>
      <li>Focused on reliability in challenging conditions (additive noise, device variability, domain mismatch).</li>
      <li>Reported strong screening-aligned performance with improvements in discrimination metrics.</li>
    </ul>
  </div>

</div>

<!-- ================== PROJECT 4 ================== -->
<div class="proj">

  <div class="proj-top">

    <div class="proj-media">
      <img class="proj-img"
           src="{{ '/assets/img/research/hand-vein-authentication.webp' | relative_url }}"
           alt="Dynamic ROI hand vein authentication"
           loading="lazy"
           decoding="async">
    </div>

    <div>
      <h3 class="proj-title">Robust Human Authentication via Dynamic ROI from Hand Vein Images</h3>
      <p class="proj-meta">May 2019 – Dec 2019 · Supervised by Dr. Mohammed Imam-ul Hassan Bhuiyan · Bangladesh University of Engineering and Technology</p>
      <p class="proj-desc">
        Vision-based biometric authentication using dynamic ROI extraction from dorsal/palm hand vein imagery with robustness to pose and acquisition variability.
      </p>
    </div>

    <div class="proj-links">
      <a class="proj-link" href="https://github.com/FarhatBuet14/VeinNET" target="_blank" rel="noopener" aria-label="GitHub repository">
        <svg width="18" height="18" viewBox="0 0 16 16" fill="currentColor" aria-hidden="true">
          <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38
          0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52
          -.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64
          -.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18
          1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56
          .82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2
          0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
        </svg>
      </a>
    </div>

  </div>

  <div class="proj-bottom">
    <ul>
      <li>Implemented dynamic ROI extraction to reduce sensitivity to alignment, pose, and background variation.</li>
      <li>Trained deep models for identity verification and evaluated robustness across acquisition conditions.</li>
      <li>Built a streamlined pipeline suitable for integration into practical authentication workflows.</li>
      <li>Emphasized reliability and security considerations relevant to real deployment environments.</li>
    </ul>
  </div>

</div>

</div>
