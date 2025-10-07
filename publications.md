---
layout: default
title: About
permalink: /
---

<div class="posts">
  <div class="post">
    <h1 class="post-title">About</h1>

    <div class="about-wrap">
      <img class="about-photo" src="{{ '/public/img/rohan.png' | relative_url }}" alt="Rohan Khan headshot">

      {% capture about_md %}
**Core Skills:**  
Bioinformatics · Medical Genomics · Cancer Genomics · Whole-Genome Sequencing (WGS) · Targeted NGS · Variant Calling (SNVs, CNVs, SVs) · Mutational Profiling & Burden · Copy Number & Ploidy Analysis · RNA-seq · Machine Learning · Statistical Genetics · R (tidyverse, phyloseq, ggplot) · Python · Perl · Git · High-Performance Computing (SLURM/Linux) · HMM-based Annotation
      {% endcapture %}
      {{ about_md | markdownify }}
    </div>
  </div>
</div>

<style>

.about-wrap {
  position: relative;
}
.about-photo {
  width: 160px;
  height: 160px;
  object-fit: cover;
  border-radius: 9999px; 
  float: right;
  margin: 0 0 1rem 1.25rem; 
  border: 3px solid rgba(0,0,0,0.06);
}
@media (max-width: 640px) {
  .about-photo { float: none; display: block; margin: 0 auto 1rem auto; }
}
</style>
