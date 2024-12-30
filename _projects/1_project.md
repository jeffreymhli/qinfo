---
layout: page
title: project 1
description: with background image
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

<style>
/* --- CSS for Dropdown --- */

.course-block {
  margin-bottom: 2rem;
  border: 1px solid #ddd;
  padding: 1rem;
  border-radius: 4px;
}

/* Wrap the dropdown button */
.dropdown {
  position: relative;
  display: inline-block;
}

/* Style the dropdown button */
.dropbtn {
  background-color: #008c9e;
  color: white;
  padding: 10px 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
  border-radius: 4px;
}

/* Hover effect for the dropdown button */
.dropbtn:hover {
  background-color: #007480;
}

/* The dropdown content (hidden by default) */
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 200px;
  border: 1px solid #ddd;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
  z-index: 1;
  padding: 0.5rem 0;
}

/* Links inside the dropdown */
.dropdown-content a {
  color: #333;
  padding: 0.5rem 1rem;
  text-decoration: none;
  display: block;
}

/* Change color of dropdown links on hover */
.dropdown-content a:hover {
  background-color: #eee;
}

/* Show the dropdown menu on hover */
.dropdown:hover .dropdown-content {
  display: block;
}
</style>

<!-- Main Content: Example Course 1 -->
<h2>ESC194 – Calculus I</h2>
<div class="course-block">
  <p>
    A first-year calculus course covering typical content,
    including some real analysis and differential equations.
  </p>

  <div class="dropdown">
    <button class="dropbtn">Course Materials</button>
    <div class="dropdown-content">
      <a href="assets/pdf/AER210.pdf" target="_blank">
        Lecture Notes
      </a>
    </div>
  </div>
</div>

<!-- Repeat the above "course-block" section for additional courses -->
