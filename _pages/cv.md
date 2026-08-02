---
layout: page
title: CV
permalink: /cv/
nav: true
nav_order: 5
---

<style>
  .cv-pdf-actions {
    display: flex;
    align-items: center;
    gap: 0.65rem;
    margin: 0 0 1rem;
  }

  .cv-pdf-open {
    display: inline-flex;
    align-items: center;
    gap: 0.45rem;
    padding: 0.45rem 0.8rem;
    border: 1px solid var(--site-accent-color);
    border-radius: 0.3rem;
    color: var(--site-accent-color) !important;
    font-size: 0.88rem;
    font-weight: 600;
    line-height: 1.2;
    text-decoration: none !important;
  }

  .cv-pdf-open:hover,
  .cv-pdf-open:focus {
    background: var(--site-accent-color);
    color: #ffffff !important;
  }

  .cv-pdf-frame {
    display: block;
    box-sizing: border-box;
    width: 100%;
    max-width: 100%;
    height: 1100px;
    border: 1px solid var(--global-divider-color);
    border-radius: 4px;
  }

  .cv-mobile-panel {
    display: none;
  }

  @media (max-width: 767.98px) {
    .cv-pdf-frame {
      display: none;
    }

    .cv-pdf-actions {
      display: none;
    }

    .cv-mobile-panel {
      display: block;
      box-sizing: border-box;
      width: 100%;
      margin-top: 1rem;
      padding: 1.2rem;
      border: 1px solid var(--global-divider-color);
      border-radius: 0.6rem;
      text-align: center;
    }

    .cv-mobile-panel p {
      margin: 0 0 1rem;
      font-size: 0.92rem;
      line-height: 1.5;
    }

    .cv-mobile-panel .cv-pdf-open {
      justify-content: center;
      width: 100%;
    }
  }
</style>

{% assign cv_pdf = '/assets/pdf/CurriculumVitae_HyunseokSeung.pdf' | relative_url %}

<div class="cv-pdf-actions">
  <a
    class="cv-pdf-open"
    href="{{ cv_pdf }}"
    target="_blank"
    rel="noopener noreferrer"
  >
    <i class="fa-solid fa-file-pdf"></i>
    Open CV as PDF
  </a>
</div>

<iframe
  class="cv-pdf-frame"
  src="{{ cv_pdf }}"
  title="Hyunseok Seung Curriculum Vitae"
>
</iframe>

<div class="cv-mobile-panel">
  <p>
    Open the CV in your browser’s PDF viewer for a properly scaled,
    scrollable mobile version.
  </p>

  <a
    class="cv-pdf-open"
    href="{{ cv_pdf }}"
    target="_blank"
    rel="noopener noreferrer"
  >
    <i class="fa-solid fa-file-pdf"></i>
    Open CV PDF
  </a>
</div>