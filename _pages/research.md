---
title: ""
permalink: /research/
---

<style>
/* Hide the auto page title rendered by the hero-page layout */
.k-page-title { display: none !important; }

/* Page spacing */
.research-wrap{
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 1rem;
}

/* Project blocks (fast + responsive) */
.proj{
  display: grid;
  grid-template-columns: minmax(260px, 380px) 1fr 44px;
  gap: 1.25rem;
  align-items: start;

  padding: 1.25rem 1.25rem;
  margin: 1.25rem 0;

  border: 1px solid rgba(255,255,255,.14);
  border-radius: 16px;
  background: rgba(0,0,0,.12);

  /* Performance: avoid heavy layout/paint cost until near viewport */
  content-visibility: auto;
  contain-intrinsic-size: 720px;
}

/* Image */
.proj-img{
  width: 100%;
  height: auto;
  display: block;
  border-radius: 12px;
  border: 1px solid rgba(255,255,255,.12);
  background: rgba(255,255,255,.04);
}

/* Text */
.proj-title{
  margin: 0 0 .35rem 0;
  font-size: 1.45rem;
  line-height: 1.2;
}
.proj-meta{
  margin: 0 0 .65rem 0;
  opacity: .85;
  font-size: .98rem;
}
.proj-desc{
  margin: 0 0 .65rem 0;
  opacity: .95;
}

/* Bullets */
.proj ul{
  margin: .65rem 0 0 1.1rem;
}
.proj li{
  margin: .35rem 0;
}

/* Link column (right side) */
.proj-links{
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: .6rem;
  padding-top: .2rem;
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

/* Make it mobile-friendly */
@media (max-width: 900px){
  .proj{
    grid-template-columns: 1fr;
  }
  .proj-links{
    flex-direction: row;
    justify-content: flex-start;
    padding-top: 0;
  }
}

/* Respect reduced motion */
@media (prefers-reduced-motion: reduce){
  .proj-link{ transition: none; }
}
</style>

<div class="research-wrap">

## Research

I build deployable computer vision and edge-to-cloud AI systems for real-world sensing—focused on robustness, scalability, and reliability in operational settings.

---

## Selected projects

<!--
IMPORTANT:
1) Put your images in: /assets/img/research/
2) Replace each GitHub URL: https://github.com/YOUR-ORG/YOUR-REPO
-->

<div class="proj">

  <div>
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
      End-to-end computer vision pipeline and interactive dashboards for mosquito surveillance: species, gonotrophy, larval attributes, and anatomy inference from heterogeneous imagery.
    </p>
    <ul>
      <li>Developed multi-task deep learning workflows across adult and larval stages for classification and biological inference.</li>
      <li>Evaluated multiple model families and established reproducible training/validation protocols for deployment-oriented performance.</li>
      <li>Integrated explainability outputs to support human verification and operational trust in high-impact decisions.</li>
      <li>Packaged results into accessible dashboards for field partners and applied use cases.</li>
    </ul>
  </div>

  <div class="proj-links">
    <a class="proj-link" href="https://github.com/YOUR-ORG/mosquitoai" target="_blank" rel="noopener" aria-label="GitHub repository">
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


<div class="proj">

  <div>
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
      A field-deployable sensing system that captures multi-focus imagery on-device and synchronizes data to the cloud for automated detection, analytics, and alerting.
    </p>
    <ul>
      <li>Designed an end-to-end pipeline from edge capture (multi-focus) to cloud storage, metadata logging, and model inference.</li>
      <li>Built automated workflows for extracting single-mosquito crops via localization and preparing training-ready datasets.</li>
      <li>Enabled scalable monitoring by standardizing capture formats, metadata schemas, and deployment-ready processing.</li>
      <li>Implemented robust evaluation to quantify performance under real-world conditions (clutter, occlusion, domain shift).</li>
    </ul>
  </div>

  <div class="proj-links">
    <a class="proj-link" href="https://github.com/YOUR-ORG/smart-mosquito-trap" target="_blank" rel="noopener" aria-label="GitHub repository">
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


<div class="proj">

  <div>
    <img class="proj-img"
         src="{{ '/assets/img/research/valvular-heartsound.webp' | relative_url }}"
         alt="Valvular disease classification from heartsound"
         loading="lazy"
         decoding="async">
  </div>

  <div>
    <h3 class="proj-title">Valvular Disease Classification from Heartsound Data</h3>
    <p class="proj-meta">Feb 2020 – Jul 2020 · Supervised by Dr. Taufiq Hasan · BUET</p>
    <p class="proj-desc">
      Computer-aided analysis of heartsound recordings for robust cardiac abnormality detection under noise and sensor variability.
    </p>
    <ul>
      <li>Developed preprocessing and feature engineering pipelines for heartsound signals under real-world noise.</li>
      <li>Trained deep classifiers for abnormality detection and benchmarked performance across multiple datasets.</li>
      <li>Focused on reliability in challenging conditions (additive noise, device variability, domain mismatch).</li>
      <li>Reported strong results with improvements in AUC and F1 aligned to clinical screening settings.</li>
    </ul>
  </div>

  <div class="proj-links">
    <a class="proj-link" href="https://github.com/YOUR-ORG/heartsound-valvular-classification" target="_blank" rel="noopener" aria-label="GitHub repository">
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


<div class="proj">

  <div>
    <img class="proj-img"
         src="{{ '/assets/img/research/hand-vein-authentication.webp' | relative_url }}"
         alt="Dynamic ROI hand vein authentication"
         loading="lazy"
         decoding="async">
  </div>

  <div>
    <h3 class="proj-title">Robust Human Authentication via Dynamic ROI from Hand Vein Images</h3>
    <p class="proj-meta">May 2019 – Dec 2019 · Supervised by Dr. Mohammed Imam-ul Hassan Bhuiyan · BUET</p>
    <p class="proj-desc">
      Vision-based biometric authentication using ROI extraction from dorsal/palm hand vein imagery with robustness to pose and acquisition variability.
    </p>
    <ul>
      <li>Implemented dynamic ROI extraction to reduce sensitivity to alignment, pose, and background variation.</li>
      <li>Trained deep models for identity verification and evaluated robustness across acquisition conditions.</li>
      <li>Built a streamlined pipeline that supports repeatable evaluation and practical system integration.</li>
      <li>Emphasized reliability and security considerations relevant to real deployment environments.</li>
    </ul>
  </div>

  <div class="proj-links">
    <a class="proj-link" href="https://github.com/YOUR-ORG/hand-vein-authentication" target="_blank" rel="noopener" aria-label="GitHub repository">
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

</div>
