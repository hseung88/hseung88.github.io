---
layout: page
title: "CV"
permalink: /cv/
---

<style>
.page-title { display: none; }
</style>

<style>
:root {
  --accent-color: #0056a4;
  --accent-soft: #f4f7fb;
  --text-color: #222222;
  --muted-color: #666666;
}

.cv-container {
  max-width: 760px;
  margin: 0 auto;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  color: var(--text-color);
  line-height: 1.6;
  font-size: 16px;
}

.cv-section {
  margin-top: 2.5rem;
  padding: 1.5rem 1.75rem;
  border-radius: 12px;
  background-color: var(--accent-soft);
}

.cv-section h2 {
  margin-top: 0;
  margin-bottom: 1rem;
  font-size: 1.1rem;
  font-weight: 600;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  color: var(--accent-color);
}

.cv-button {
  display: inline-block;
  padding: 0.45rem 1.1rem;
  border-radius: 999px;
  font-size: 0.85rem;
  text-decoration: none;
  border: 1px solid var(--accent-color);
  color: #ffffff;
  background-color: var(--accent-color);
  font-weight: 500;
  margin-bottom: 1rem;
}

.cv-button-outline {
  background-color: transparent;
  color: var(--accent-color);
}

.cv-button:hover {
  opacity: 0.9;
}

.cv-embed {
  margin-top: 1rem;
  width: 100%;
  border: none;
  border-radius: 8px;
}
</style>

<div class="cv-container">

  <div class="cv-section">
    <h2>Curriculum Vitae</h2>

    <a class="cv-button-outline"
       href="{{ '/assets/cv/Academic_CV_Hyunseok_Seung.pdf' | relative_url }}"
       target="_blank"
       download="Hyunseok_Seung_CV">
      Download CV (PDF)
    </a>

    <embed class="cv-embed"
           src="{{ '/assets/cv/Academic_CV_Hyunseok_Seung.pdf' | relative_url }}"
           type="application/pdf"
           height="1000px" />
  </div>

</div>
