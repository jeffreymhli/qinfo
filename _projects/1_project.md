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
/* --- CSS for Dropdown (Click-to-open version) --- */

/* Course block container */
.course-block {
  margin-bottom: 2rem;
  border: 1px solid #ddd;
  padding: 1rem;
  border-radius: 4px;
}

/* Wrap the dropdown button and content */
.dropdown {
  position: relative;
  display: inline-block;
}

/* Style the button that toggles the dropdown */
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

/* The dropdown content is hidden by default; toggled via JavaScript */
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

/* Show the dropdown when toggled */
.show {
  display: block;
}
</style>

<!-- Main Content: Example Course 1 -->
<h2>AER210 – Fluid Mechanics</h2>
<div class="course-block">
  <p>
    A second-year Multi-variable Calculus course with Fluid mechanics on the second half.
  </p>

  <!-- Dropdown container -->
  <div class="dropdown">
    <!-- Button that triggers the dropdown -->
    <button onclick="toggleDropdown('myDropdown')" class="dropbtn">
      Course Materials
    </button>

    <!-- Dropdown menu -->
    <div id="myDropdown" class="dropdown-content">
      <a href="assets/AER210.pdf" target="_blank">
        Lecture Notes
      </a>
    </div>
  </div>
</div>

<!-- Repeat the above block for additional courses, 
     giving each dropdown-content a unique ID, e.g. myDropdown2, myDropdown3, etc. -->

<script>
/**
 * Toggle the dropdown menu for a given ID.
 * @param {string} dropdownID - The ID of the dropdown-content div
 */
function toggleDropdown(dropdownID) {
  document.getElementById(dropdownID).classList.toggle("show");
}

/**
 * Close the dropdown if the user clicks outside of it.
 */
window.onclick = function(event) {
  // If the click is NOT on a dropbtn, close all dropdowns
  if (!event.target.matches('.dropbtn')) {
    var dropdowns = document.getElementsByClassName("dropdown-content");
    for (var i = 0; i < dropdowns.length; i++) {
      var openDropdown = dropdowns[i];
      if (openDropdown.classList.contains('show')) {
        openDropdown.classList.remove('show');
      }
    }
  }
}
</script>