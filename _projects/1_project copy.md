---
layout: page
title: project 3 with very long name
description: a project that redirects to another website
img: assets/img/7.jpg
redirect: https://unsplash.com
importance: 3
category: work
---

Some introductory text here.

<div class="dropdown">
    <button class="dropbtn">Menu</button>
    <div class="dropdown-content">
        <a href="assets\pdf\AER210.pdf" target="_blank">View PDF</a>
    </div>
</div>

<style>
    /* Basic styling for the dropdown menu */
    .dropdown {
        position: relative;
        display: inline-block;
    }

    .dropdown-content {
        display: none;
        position: absolute;
        background-color: #f9f9f9;
        min-width: 160px;
        box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
        z-index: 1;
    }

    .dropdown-content a {
        color: black;
        padding: 12px 16px;
        text-decoration: none;
        display: block;
    }

    .dropdown-content a:hover {
        background-color: #f1f1f1;
    }

    .dropdown:hover .dropdown-content {
        display: block;
    }

    .dropbtn {
        background-color: #4CAF50;
        color: white;
        padding: 16px;
        font-size: 16px;
        border: none;
        cursor: pointer;
    }
</style>

{% endraw %}