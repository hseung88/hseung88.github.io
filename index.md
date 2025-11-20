---
layout: page
permalink: /
---

<style>
:root {
  --accent-color: #0056a4;
  --accent-soft: #f4f7fb;
  --text-color: #222222;
  --muted-color: #666666;
}

.page-about {
  max-width: 760px;
  margin: 0 auto;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  color: var(--text-color);
  line-height: 1.6;
  font-size: 16px;
}

.page-about-header {
  text-align: center;
  margin-bottom: 2.5rem;
}

.page-about-header img {
  width: 240px;
  border-radius: 50%;
  box-shadow: 0 10px 30px rgba(0,0,0,0.08);
}

.page-about-header h1 {
  margin-top: 1.25rem;
  margin-bottom: 0.25rem;
  font-size: 1.9rem;
  letter-spacing: 0.03em;
}

.page-about-header .subtitle {
  font-size: 0.95rem;
  color: var(--muted-color);
}

.page-about p {
  margin: 0.75rem 0;
}

.page-section {
  margin-top: 2.5rem;
  padding: 1.5rem 1.75rem;
  border-radius: 12px;
  background-color: var(--accent-soft);
}

.page-section h2 {
  margin-top: 0;
  margin-bottom: 0.75rem;
  font-size: 1.1rem;
  font-weight: 600;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  color: var(--accent-color);
}

.page-about a {
  color: var(--accent-color);
  text-decoration: none;
  border-bottom: 1px solid rgba(0,86,164,0.2);
}

.page-about a:hover {
  border-bottom-color: rgba(0,86,164,0.6);
}

.page-section ul {
  list-style: none;
  padding-left: 0;
  margin: 0.25rem 0 0;
}

.page-section li {
  margin-bottom: 0.4rem;
}

.news-date {
  font-weight: 600;
  font-feature-settings: "tnum" 1;
  margin-right: 0.5rem;
}

.news-item-title {
  font-weight: 500;
}

.contact-list li {
  margin-bottom: 0.3rem;
}

@media (max-width: 600px) {
  .page-about {
    padding: 0 0.5rem;
  }

  .page-about-header img {
    width: 200px;
  }
}
</style>

<div class="page-about">

  <div class="page-about-header">
    <img src="assets/images/Profile.jpg" alt="Hyunseok Seung">
    <h1>Hyunseok Seung</h1>
    <div class="subtitle">
      Postdoctoral Researcher · University of Wisconsin–Madison<br>
      <span style="color: var(--muted-color);">hseung2 at wisc dot edu</span>
    </div>
  </div>

  <p>
    I am a Postdoctoral Researcher in the Department of Statistics at the
    <a href="https://stat.wisc.edu/">University of Wisconsin–Madison</a>, working with
    Professor <a href="https://sites.google.com/view/katzfuss/home?authuser=0">Matthias Katzfuss</a>.
  </p>

  <p>
    I received my Ph.D. in Statistics from the
    <a href="https://stat.uga.edu/">University of Georgia</a> in 2025, co-advised by Professors
    <a href="https://ppmlguy.github.io/">Jaewoo Lee</a> and
    <a href="https://yuan-ke.github.io/">Yuan Ke</a>. Before that, I completed my M.A. and B.A.
    in Applied Statistics at
    <a href="https://devcms.yonsei.ac.kr/stat_en/index.do">Yonsei University</a>.
  </p>

  <p>
    My research focuses on 
    <span style="color: var(--accent-color); font-weight: 600;">deep learning optimization</span>
    and 
    <span style="color: var(--accent-color); font-weight: 600;">Bayesian optimization</span>,
    with an emphasis on curvature-aware gradient methods.
  </p>


  <div class="page-section">
    <h2>News 📰</h2>
    <ul>
      <li>
        <span class="news-date">11/2025</span>
        <span class="news-item-title">
          <em>Low-Rank Curvature for Zeroth-Order Optimization in LLM Fine-Tuning</em>
        </span>
        accepted to AAAI 2026.
        Preprint:
        <a href="https://arxiv.org/abs/2511.07971" target="_blank">arXiv</a>
      </li>
      <li>
        <span class="news-date">10/2025</span>
        <span class="news-item-title">
          <em>MAC: An Efficient Gradient Preconditioning using Mean Activation Approximated Curvature</em>
        </span>
        accepted to ICDM 2025.
        Preprint:
        <a href="https://arxiv.org/abs/2506.08464" target="_blank">arXiv</a>
      </li>
      <li>
        <span class="news-date">08/2025</span>
        Joined the Katzfuss group as a postdoctoral researcher.
      </li>
    </ul>
  </div>

</div>
