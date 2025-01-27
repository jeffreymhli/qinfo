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

<a href="{{ site.baseurl }}/assets/pdf/Undergraduate_Physics.pdf" target="_blank">
UnderGraduate Physics
</a>

<a href="{{ site.baseurl }}/assets/pdf/Undergraduate_Math.pdf" target="_blank">
UnderGraduate Math
</a>



<!-- Main Content: Example Course 1 -->
<h2>AER210 – Fluid Mechanics</h2>
<div class="course-block">
  <p>
    A second-year Multi-variable Calculus course with Fluid mechanics on the second half.
  </p>

  <!-- Dropdown container -->
  <div class="dropdown">
    <!-- Button that triggers the dropdown -->
    <button onclick="toggleDropdown('myDropdown1')" class="dropbtn">
      Course Materials
    </button>

    <!-- Dropdown menu -->
    <div id="myDropdown1" class="dropdown-content">
      <a href="{{ site.baseurl }}/assets/pdf/AER210.pdf" target="_blank">
        Lecture Notes
      </a>
    </div>
  </div>
</div>


<!-- Main Content: Example Course 1 -->
<h2>Che260 - Heat Transfer and Thermodynamics</h2>
<div class="course-block">
  <p>
    A second-year Theomodynamics and Heat Transfer Course
  </p>

  <!-- Dropdown container -->
  <div class="dropdown">
    <!-- Button that triggers the dropdown -->
    <button onclick="toggleDropdown('myDropdown2')" class="dropbtn">
      Course Materials
    </button>

    <!-- Dropdown menu -->
    <div id="myDropdown2" class="dropdown-content">
      <a href="{{ site.baseurl }}/assets/pdf/CHE260.pdf" target="_blank">
        Lecture Notes
      </a>
    </div>
  </div>
</div>


<!-- Main Content: Example Course 1 -->
<h2>PHY365 - Quantum Information</h2>
<div class="course-block">
  <p>
    A Third Year introductory Course on Quantum Information
  </p>

  <!-- Dropdown container -->
  <div class="dropdown">
    <!-- Button that triggers the dropdown -->
    <button onclick="toggleDropdown('myDropdown3')" class="dropbtn">
      Course Materials
    </button>

    <!-- Dropdown menu -->
    <div id="myDropdown3" class="dropdown-content">
      <a href="{{ site.baseurl }}/assets/pdf/PHY365.pdf" target="_blank">
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