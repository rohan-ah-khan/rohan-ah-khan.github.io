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
        <strong><a href="https://github.com/ccmbioinfo/ccm_benchmate" target="_blank" rel="noopener">CCM-Benchmate</a></strong><br>
        Worked on creating a Container Runner module for CCM Benchmate to execute Docker/Singularity commands without CLI. Benchmate is a modular Python toolkit that integrates biological data from APIs, literature, sequences, structures, variants, genomes, and containerized pipelines into a unified, queryable knowledge base for computational biology.
      </li>

      <li>
        <strong><a href="https://github.com/ccmbioinfo/crg2-pacbio" target="_blank" rel="noopener">crg2-pacbio</a></strong><br>
        Worked on creating a QC module for crg2-pacbio to collect and consolidate various allignment and variant quality control metrics into a single report. crg2-pacbio is a long-read variant annotation pipeline.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-uhn/pipeline-suite" target="_blank" rel="noopener">Targeted-Seq-Pipeline</a></strong><br>
        Developed an end-to-end targeted-seq pipeline for translational research in follicular lymphoma. The pipeline processes raw reads, and uses consensus SNV and CNV caliing to generate variant calls for targeted-seq data.
      </li>
      
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
        TensorFlow and Keras based model for predicting promoters (e.g., TATA box) from synthetic DNA sequences.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/RNAseq-Pipeline" target="_blank" rel="noopener">RNAseq-Pipeline</a></strong><br>
        Built a reproducible RNA-seq analysis pipeline with HISAT2, HTSeq, and edgeR to identify drug responses in muscle cell lines. Repo has demo example with publically avaiable Yeast data.
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
