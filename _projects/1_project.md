---
layout: page
title: University Notes
description: This page includes all the university notes for specific courses. It may not be entirely complete or correct.
img: assets/img/uoft.png
importance: 1
category: work
related_publications: true
---

<style>
  /* Term Headers (e.g. Year 1) */
  .term-header {
    font-size: 1.5rem;
    font-weight: 600;
    color: #333;
    margin-top: 3rem;
    margin-bottom: 1.5rem;
    padding-left: 15px;
    border-left: 4px solid #0056b3; /* The blue accent line */
  }

  /* Course Container */
  .course-block {
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 1px dashed #eee; /* Subtle separator */
  }

  /* Course Title Row */
  .course-title {
    font-size: 1.1rem;
    font-weight: bold;
    margin-bottom: 0.5rem;
  }

  .course-code {
    color: #0056b3; /* Academic Blue */
    margin-right: 8px;
  }

  /* Course Description */
  .course-desc {
    font-size: 0.95rem;
    color: #666;
    margin-bottom: 0.8rem;
    line-height: 1.5;
  }

  /* Resource Links Container */
  .resource-list {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }

  /* The Link "Buttons" */
  .resource-tag {
    background-color: #f4f4f9;
    color: #0056b3 !important; /* Force color to match theme */
    padding: 4px 10px;
    border-radius: 4px;
    font-size: 0.85rem;
    text-decoration: none;
    transition: background-color 0.2s ease;
    border: 1px solid #e0e0e0;
  }

  .resource-tag:hover {
    background-color: #e2e2ff;
    text-decoration: none;
  }
</style>

<div class="term-header">General Resources</div>

<div class="course-block">
  <div class="course-title">
    <span class="course-code">PHY-GEN</span> Undergraduate Physics
  </div>
  <div class="course-desc">
    General notes covering the undergraduate physics curriculum.
  </div>
  <div class="resource-list">
    <a href="{{ site.baseurl }}/assets/pdf/Undergraduate_Physics.pdf" target="_blank" class="resource-tag">Full Notes</a>
    </div>
</div>

<div class="course-block">
  <div class="course-title">
    <span class="course-code">MAT-GEN</span> Undergraduate Math
  </div>
  <div class="course-desc">
    Comprehensive mathematics notes.
  </div>
  <div class="resource-list">
    <a href="{{ site.baseurl }}/assets/pdf/Undergraduate_Math.pdf" target="_blank" class="resource-tag">Full Notes</a>
  </div>
</div>

<div class="term-header">Specialized Topics</div>

<div class="course-block">
  <div class="course-title">
    <span class="course-code">PHY350</span> Electromagnetism
  </div>
  <div class="course-desc">
    Advanced EM theory, Maxwell's equations, and waves.
  </div>
  <div class="resource-list">
    <a href="{{ site.baseurl }}/assets/pdf/E_M.pdf" target="_blank" class="resource-tag">Lecture Notes</a>
  </div>
</div>

<div class="course-block">
  <div class="course-title">
    <span class="course-code">PHY400</span> Quantum Topics
  </div>
  <div class="course-desc">
    Coverage of Quantum Optics and Quantum Information theory.
  </div>
  <div class="resource-list">
    <a href="{{ site.baseurl }}/assets/pdf/Quantum_Optics.pdf" target="_blank" class="resource-tag">Quantum Optics</a>
    <a href="{{ site.baseurl }}/assets/pdf/Quantum_Information.pdf" target="_blank" class="resource-tag">Quantum Information</a>
  </div>
</div>