---
layout: page
permalink: /talks/
title: Talks
nav: true
nav_order: 3
---

<style>
  .talks-page {
    --talks-border: var(--site-accent-soft-border, #d4e1ea);
    --talks-muted: var(--global-text-color-light, #626970);
    color: var(--global-text-color, #212529);
  }

  .talks-page .talks-intro {
    margin: -0.25rem 0 1.8rem;
    color: var(--talks-muted);
    font-size: 0.96rem;
    line-height: 1.6;
  }

  .talks-page .talks-section {
    margin: 0 0 2rem;
    padding: clamp(1.35rem, 3vw, 2rem);
    border: 1px solid var(--talks-border);
    border-radius: 0.9rem;
    background: var(--global-card-bg-color, #fff);
  }

  .talks-page .talks-section-header {
    margin: 0;
    padding: 0 0 1rem;
    border-bottom: 1px solid var(--global-divider-color, #e2e5e8);
  }

  .talks-page .talks-section-header h2 {
    margin: 0;
    color: var(--global-text-color, #212529);
    font-size: clamp(1.35rem, 2.5vw, 1.75rem);
    font-weight: 600;
    line-height: 1.25;
    letter-spacing: -0.015em;
  }

  .talks-page .talks-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .talks-page .talks-item {
    display: grid;
    grid-template-columns: 4.5rem minmax(0, 1fr);
    gap: 1.4rem;
    margin: 0;
    padding: 1.45rem 0;
    border-bottom: 1px solid var(--global-divider-color, #e2e5e8);
  }

  .talks-page .talks-item:last-child {
    padding-bottom: 0;
    border-bottom: 0;
  }

  .talks-page .talks-date {
    display: flex;
    flex-direction: column;
    gap: 0.22rem;
    padding-top: 0.1rem;
    font-variant-numeric: tabular-nums;
  }

  .talks-page .talks-year {
    color: var(--site-accent-color, #1f4e79);
    font-size: 1.12rem;
    font-weight: 650;
    line-height: 1.25;
  }

  .talks-page .talks-month {
    color: var(--talks-muted);
    font-size: 0.73rem;
    line-height: 1.3;
    letter-spacing: 0.065em;
    text-transform: uppercase;
  }

  .talks-page .talks-details {
    min-width: 0;
  }

  .talks-page .talks-title {
    margin: 0 0 0.45rem;
    color: var(--global-text-color, #212529);
    font-size: 1.03rem;
    font-weight: 600;
    line-height: 1.45;
    letter-spacing: -0.01em;
    overflow-wrap: break-word;
  }

  .talks-page .talks-venue {
    margin: 0;
    color: var(--global-text-color, #212529);
    font-size: 0.87rem;
    line-height: 1.5;
  }

  .talks-page .talks-location {
    margin: 0.2rem 0 0;
    color: var(--talks-muted);
    font-size: 0.8rem;
    line-height: 1.45;
  }

  .talks-page .talks-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 0.75rem;
  }

  .talks-page .talks-links a {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    min-height: 2rem;
    padding: 0.28rem 0.65rem;
    border: 1px solid var(--talks-border);
    border-radius: 0.3rem;
    background: var(--global-card-bg-color, #fff);
    color: var(--site-accent-color, #1f4e79);
    font-size: 0.76rem;
    font-weight: 600;
    line-height: 1.3;
    text-decoration: none;
  }

  .talks-page .talks-links a:hover {
    border-color: var(--site-accent-color, #1f4e79);
    background: var(--site-accent-soft-bg, #eef4f8);
    color: var(--site-accent-hover-color, #163a5a);
    text-decoration: none;
  }

  .talks-page .talks-links a:focus-visible {
    outline: 2px solid var(--site-accent-color, #1f4e79);
    outline-offset: 3px;
  }

  @media (max-width: 575.98px) {
    .talks-page .talks-intro {
      margin-bottom: 1.4rem;
      font-size: 0.9rem;
    }

    .talks-page .talks-section {
      padding: 1.1rem;
      border-radius: 0.75rem;
    }

    .talks-page .talks-item {
      grid-template-columns: minmax(0, 1fr);
      gap: 0.6rem;
      padding-top: 1.25rem;
      padding-bottom: 1.25rem;
    }

    .talks-page .talks-date {
      flex-direction: row;
      align-items: baseline;
      gap: 0.5rem;
      padding: 0;
    }

    .talks-page .talks-year {
      font-size: 0.86rem;
    }

    .talks-page .talks-month {
      font-size: 0.69rem;
    }

    .talks-page .talks-title {
      font-size: 0.97rem;
    }

    .talks-page .talks-links a {
      min-height: 2.75rem;
    }
  }
</style>

<div class="talks-page">

  <section class="talks-section" aria-labelledby="oral-presentations">
    <header class="talks-section-header">
      <h2 id="oral-presentations">Oral presentations</h2>
    </header>

    <ul class="talks-list">
      <li class="talks-item">
        <time class="talks-date" datetime="2026-08">
          <span class="talks-year">2026</span>
          <span class="talks-month">August</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">Scalable Derivative Gaussian Processes via Exact Gradient Reduction</h3>
          <p class="talks-venue">Institute for Foundations of Data Science (IFDS) Research Expo</p>
          <p class="talks-location">Madison, WI</p>
        </div>
      </li>

      <li class="talks-item">
        <time class="talks-date" datetime="2025-11">
          <span class="talks-year">2025</span>
          <span class="talks-month">November</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">An Efficient Gradient Preconditioning using Mean Activation Approximated Curvature</h3>
          <p class="talks-venue">IEEE International Conference on Data Mining (ICDM)</p>
          <p class="talks-location">Washington, DC</p>
        </div>
      </li>

      <li class="talks-item">
        <time class="talks-date" datetime="2024-12">
          <span class="talks-year">2024</span>
          <span class="talks-month">December</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">A Scalable Preconditioned Gradient Descent using Nystrom Approximation</h3>
          <p class="talks-venue">IEEE International Conference on Big Data</p>
          <p class="talks-location">Washington, DC</p>
        </div>
      </li>

      <li class="talks-item">
        <time class="talks-date" datetime="2018-05">
          <span class="talks-year">2018</span>
          <span class="talks-month">May</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">Modified Likelihood Ratio Tests for Extreme Value Distributions</h3>
          <p class="talks-venue">Korean Data and Information Science Society (KDISS)</p>
          <p class="talks-location">Pukyong University · Busan, South Korea</p>
        </div>
      </li>
    </ul>
  </section>

  <section class="talks-section" aria-labelledby="poster-presentations">
    <header class="talks-section-header">
      <h2 id="poster-presentations">Posters</h2>
    </header>

    <ul class="talks-list">
      <li class="talks-item">
        <time class="talks-date" datetime="2026-01">
          <span class="talks-year">2026</span>
          <span class="talks-month">January</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">Low-Rank Curvature for Zeroth-Order Optimization in LLM Fine-Tuning</h3>
          <p class="talks-venue">AAAI Conference on Artificial Intelligence</p>
          <p class="talks-location">Singapore</p>
        </div>
      </li>

      <li class="talks-item">
        <time class="talks-date" datetime="2025-04">
          <span class="talks-year">2025</span>
          <span class="talks-month">April</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">A Scalable Preconditioned Gradient Descent using Nystrom Approximation</h3>
          <p class="talks-venue">AI Research Day, Institute for Artificial Intelligence</p>
          <p class="talks-location">Athens, GA</p>
        </div>
      </li>

      <li class="talks-item">
        <time class="talks-date" datetime="2024-04">
          <span class="talks-year">2024</span>
          <span class="talks-month">April</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">An Adaptive Method Stabilizing Activations for Enhanced Generalization</h3>
          <p class="talks-venue">AI Research Day, Institute for Artificial Intelligence</p>
          <p class="talks-location">Athens, GA</p>
        </div>
      </li>

      <li class="talks-item">
        <time class="talks-date" datetime="2018-05">
          <span class="talks-year">2018</span>
          <span class="talks-month">May</span>
        </time>
        <div class="talks-details">
          <h3 class="talks-title">Modified Likelihood Ratio Tests for Extreme Value Distributions</h3>
          <p class="talks-venue">Korean Statistical Society (KSS)</p>
          <p class="talks-location">Pusan National University · Busan, South Korea</p>
        </div>
      </li>
    </ul>
  </section>
</div>
