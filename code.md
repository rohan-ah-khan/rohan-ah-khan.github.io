---
layout: page
title: Code
nav: true
nav_order: 3
---

<div class="posts">
  <div class="post">

    <p>Here are some of the repositories and projects I have worked on, spanning genomics pipelines, machine learning, and toolkit development.</p>

    <ul class="repo-list">
      <li>
        <strong><a href="https://github.com/ccmbioinfo/ccm_benchmate" target="_blank" rel="noopener">CCM-Benchmate</a></strong><br>
        Developed a Container Runner module for CCM Benchmate to execute Docker and Singularity workflows without direct CLI interaction. Also contributed to building a containerized deployment (<a href="https://hub.docker.com/r/rohanahkhan/ccm-benchmate" target="_blank" rel="noopener">Docker Hub</a>) integrating Benchmate with PostgreSQL, enabling use in HPC environments. Currently working on database-backed systems for storing and querying biological data, including natural language–based retrieval.
      </li>

      <li>
        <strong><a href="https://github.com/ccmbioinfo/CPHI-DRAGEN-anno" target="_blank" rel="noopener">CPHI-DRAGEN-anno</a></strong><br>
        Contributed to development of a Snakemake-based annotation pipeline for DRAGEN VCFs, supporting standardized and reproducible variant annotation workflows for large-scale genomics projects.
      </li>

      <li>
        <strong><a href="https://github.com/ccmbioinfo/crg2/tree/malkin/GRCm38" target="_blank" rel="noopener">Mouse-WES-Pipeline</a></strong><br>
        Contributed to a mouse whole-exome sequencing pipeline, processing data from raw reads through alignment, variant calling, and filtering to generate high-confidence germline and somatic VCFs.
      </li>
      
      <li>
        <strong><a href="https://github.com/rohan-uhn/pipeline-suite" target="_blank" rel="noopener">Targeted-Seq-Pipeline</a></strong><br>
        Developed an end-to-end targeted sequencing pipeline for translational cancer genomics, integrating consensus SNV and CNV calling for tumor-only data.
      </li>
      
      <li>
        <strong><a href="https://github.com/rohan-ah-khan/16S-Taxonomy-Assignment" target="_blank" rel="noopener">16S-Taxonomy-Assignment</a></strong><br>
        Workflow for processing and taxonomically assigning 16S rRNA gene sequences using DADA2 and SILVA databases.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/16s-ASV-Metadata-ML-Prediction" target="_blank" rel="noopener">16s-ASV-Metadata-ML-Prediction</a></strong><br>
        Machine learning models built in R (H2O AutoML, GBM) to predict environmental metadata associated with 16S ASV abundance data.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/Synthetic-Promoter-Prediction" target="_blank" rel="noopener">Synthetic-Promoter-Prediction</a></strong><br>
        TensorFlow and Keras-based model for predicting promoter regions (e.g., TATA box) from synthetic DNA sequences.
      </li>

      <li>
        <strong><a href="https://github.com/rohan-ah-khan/RNAseq-Pipeline" target="_blank" rel="noopener">RNAseq-Pipeline</a></strong><br>
        Built a reproducible RNA-seq analysis pipeline using HISAT2, HTSeq, and edgeR to identify transcriptional responses. Includes a demo with publicly available yeast data.
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
