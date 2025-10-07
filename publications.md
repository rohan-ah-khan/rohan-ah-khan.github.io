---
layout: default
title: Publications
permalink: /publications/
---

<div class="posts">
  <div class="post">
    <h1 class="post-title">Publications</h1>

    {% capture pubs %}
Below is a selection of research publications and scholarly works.  
(You can add more by editing this page or by creating posts under `_posts/` with `categories: [publication]`.)
    {% endcapture %}
    {{ pubs | markdownify }}

    <hr>

    <ul class="pub-list">
      <li>
        <strong>Predicting hydrocarbon presence in marine cold seep sediments using machine learning models trained with benthic bacterial 16S rRNA taxonomy</strong><br>
        <em>Marine Science Journal</em>, 2024.<br>
        <small>Developed ML models integrating 16S rRNA profiles and geochemical metadata to predict hydrocarbon seepage across marine sediments.</small>
      </li>

      <li>
        <strong>Identification of genetic subtypes in follicular lymphoma</strong><br>
        <em>Blood Cancer Journal</em>, 2024.<br>
        <small>Performed molecular clustering analysis of FL samples integrating methylation, transcriptomic, and mutational data to define novel subtypes.</small>
      </li>

      <li>
        <strong>Integration of gene mutations in risk prognostication for follicular lymphoma</strong><br>
        <em>Lancet Oncology</em>, 2015.<br>
        <small>Evaluated the prognostic value of seven key gene mutations (m7-FLIPI) in first-line immunochemotherapy-treated FL patients.</small>
      </li>
    </ul>
  </div>
</div>

<style>
.pub-list {
  list-style-type: none;
  padding-left: 0;
  margin-top: 1.5rem;
}
.pub-list li {
  margin-bottom: 1.5rem;
  line-height: 1.6;
}
.pub-list strong {
  font-size: 1.05rem;
}
.pub-list em {
  color: #666;
}
.pub-list small {
  display: block;
  color: #555;
}
</style>
