---
layout: page
title: Code
nav: true
nav_order: 3
---

<div class="posts">
  <div class="post">

    <p>Here are some of the repositories and projects I have worked on, spanning genomics pipelines, machine learning, and web development.</p>

    <ul class="repo-list">
      <li>
        <strong><a href="https://github.com/rohan-ah-khan/16S-Taxonomy-Assignment" target="_blank" rel="noopener">16S-Taxonomy-Assignment</a></strong><br>
        Workflow for processing and taxonomically assigning 16S rRNA gene sequences using Dada2 and SILVA databases.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/16s-ASV-Metadata-ML-Prediction" target="_blank" rel="noopener">16s-ASV-Metadata-ML-Prediction</a></strong><br>
        Machine learning models built in R (H2O AutoML, GBM) to predict environmental metadata associated with 16S ASV abundance data.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/rohan-ah-khan.github.io" target="_blank" rel="noopener">rohan-ah-khan.github.io</a></strong><br>
        My personal website and portfolio, built using Jekyll and the Hyde theme, showcasing my work and research.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/Synthetic-Promoter-Prediction" target="_blank" rel="noopener">Synthetic-Promoter-Prediction</a></strong><br>
        TensorFlow-based deep learning model for predicting promoter strength from synthetic DNA sequences, integrating CNN layers with sequence embedding features.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/RNAseq-Snakemake-Pipeline" target="_blank" rel="noopener">RNAseq-Snakemake-Pipeline</a></strong><br>
        Built a reproducible RNA-seq analysis pipeline using Snakemake with HISAT2, HTSeq, and edgeR to identify drug responses in muscle cell lines.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/Docker-Pipeline-Demo" target="_blank" rel="noopener">Docker-Pipeline-Demo</a></strong><br>
        Minimal Docker prototype used to test and containerize bioinformatics workflows before deployment in large-scale HPC environments.
      </li>
    </ul>
  </div>
</div>

<style>
.repo-list { list-style: none; padding-left: 0; margin-top: 1rem; }
.repo-list li { margin-bottom: 1.5rem; line-height: 1.6; }
.repo-list strong a { text-decoration: none; }
.repo-list strong a:hover { text-decoration: underline; }
</style>
