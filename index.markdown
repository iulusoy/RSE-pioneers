---
layout: splash
permalink: /
header:
  overlay_color: "#0d2476ff"
  overlay_image: /assets/images/header-bg.jpg
  overlay_filter: 0.3
  actions:
    - label: "<i class='fas fa-play'></i> Listen to Interviews"
      url: "https://www.buzzsprout.com/2531619/episodes/17727894"
excerpt: >
  How did the first RSEs advance science, and what factors determined success, adoption and impact of research software? These are central questions that RSE pioneers addresses.
feature_row:
  - image_path: /assets/images/dieter.jpg
    alt: "Hans-Dieter Meyer"
    title: "Featured Interview: Hans-Dieter Meyer"
    excerpt: "Quantum dynamics researcher and developer of the Heidelberg MCTDH software package."
    url: "/interview/2025/08/25/Hans-Dieter-Meyer.html"
    btn_class: "btn--primary"
    btn_label: "Read Interview"
  - image_path: /assets/images/soundbyte-image.png
    alt: "Audio Highlights"
    title: "Audio Highlights"
    excerpt: "Listen to key moments from our interviews with RSE pioneers."
    url: "/audio/"
    btn_class: "btn--primary"
    btn_label: "Listen Now"
  - image_path: /assets/images/RSE-pioneer.png
    alt: "About the Project"
    title: "About RSE Pioneers"
    excerpt: "Learn more about the RSE pioneers project."
    url: "/about/"
    btn_class: "btn--primary"
    btn_label: "Learn More"
---

<style>
/* Make feature row items same size */
.feature__wrapper {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  align-items: stretch;
}

.feature__item {
  flex: 1 1 300px;
  max-width: 33.333%;
  display: flex;
  flex-direction: column;
}

.feature__item .archive__item {
  display: flex;
  flex-direction: column;
  height: 100%;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  overflow: hidden;
  transition: box-shadow 0.3s ease;
}

.feature__item .archive__item:hover {
  box-shadow: 0 4px 15px rgba(13, 36, 118, 0.2);
}

.feature__item .archive__item-teaser {
  height: 200px;
  overflow: hidden;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #f8f9fa;
}

.feature__item .archive__item-teaser img {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
  display: block;
}

.feature__item .archive__item-body {
  flex: 1;
  display: flex;
  flex-direction: column;
  padding: 1rem;
  min-height: 150px;
}

.feature__item .archive__item-title {
  margin-bottom: 0.5rem;
  font-size: 1.1em;
  font-weight: bold;
  min-height: 2.5em;
}

.feature__item .archive__item-excerpt {
  flex: 1;
  margin-bottom: 1rem;
  line-height: 1.5;
  min-height: 4em;
}

.btn--primary {
  background-color: #0d2476ff !important;
  border-color: #0d2476ff !important;
  color: #fff !important;
  margin-top: auto;
  align-self: flex-start;
}

.btn--primary:hover {
  background-color: #092155 !important;
  border-color: #092155 !important;
}

@media (max-width: 768px) {
  .feature__item {
    max-width: 100%;
    flex: 1 1 100%;
  }
}

/* Remove horizontal line after feature row */
.feature__wrapper + *,
.feature__wrapper + * h2 {
  border-top: none !important;
  margin-top: 2rem !important;
  padding-top: 0 !important;
}

.feature__wrapper::after,
.feature__wrapper::before {
  display: none !important;
  content: none !important;
}

.feature__item .archive__item {
  display: flex;
  flex-direction: column;
  height: 100%;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  overflow: hidden;
  transition: box-shadow 0.3s ease;
  border-bottom: 1px solid #e0e0e0 !important;
}

/* Remove any hr elements or borders that might appear */
hr,
.page hr,
.initial-content hr {
  display: none !important;
  border: none !important;
  height: 0 !important;
}

/* Remove bottom border from feature wrapper */
.feature__wrapper {
  border-bottom: none !important;
  margin-bottom: 0 !important;
}
</style>

{% include feature_row %}

## About the Project

The RSE Pioneers project is created and maintained by researchers at the Scientific Software Center, Heidelberg University. We document the stories and contributions of early research software engineers.

**Contact:** For questions about the project or to suggest interview subjects, please reach out via [GitHub](https://github.com/iulusoy/RSE-pioneers/issues).