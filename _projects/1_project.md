---
layout: page
title: University Notes
description: This page includes all the university notes for specific courses.
img: assets/img/uoft.png
importance: 1
category: work
related_publications: true
---

<style>
  /* --- YOUR ORIGINAL STYLES --- */
  .term-header {
    font-size: 1.5rem;
    font-weight: 600;
    color: #333;
    margin-top: 3rem;
    margin-bottom: 1.5rem;
    padding-left: 15px;
    border-left: 4px solid #0056b3;
  }

  .course-block {
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 1px dashed #eee;
  }

  .course-title {
    font-size: 1.1rem;
    font-weight: bold;
    margin-bottom: 0.5rem;
  }

  .course-code {
    color: #0056b3;
    margin-right: 8px;
    text-transform: uppercase;
  }

  .course-desc {
    font-size: 0.95rem;
    color: #666;
    margin-bottom: 0.8rem;
    line-height: 1.5;
  }

  .resource-list {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }

  .resource-tag {
    background-color: #f4f4f9;
    color: #0056b3 !important;
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

{% assign library_files = site.static_files | where_exp: "file", "file.path contains 'assets/pdf/library'" %}

{% assign categories = "" | split: "" %}
{% for file in library_files %}
    {% assign parts = file.path | split: '/' %}
    {% if parts.size > 4 %}
        {% assign cat = parts[4] %}
        {% unless categories contains cat %}
            {% assign categories = categories | push: cat %}
        {% endunless %}
    {% endif %}
{% endfor %}

{% assign sorted_categories = categories | sort %}

<div class="notes-container">
    
    {% for category in sorted_categories %}
        
        {% assign display_header = category | replace: "year", "Year " | replace: "_", " " | capitalize %}
        <div class="term-header">{{ display_header }}</div>

        {% for file in library_files %}
            {% if file.path contains category %}
                
                {% assign filename = file.path | split: '/' | last %}
                {% assign course_name = filename | replace: ".pdf", "" | upcase %}
                
                {% if filename contains ".pdf" %}
                    <div class="course-block">
                        <div class="course-title">
                            <span class="course-code">{{ course_name }}</span>
                            </div>
                        
                        <div class="course-desc">
                            University notes for {{ course_name }}. 
                            (Automatically synced from Overleaf).
                        </div>
                        
                        <div class="resource-list">
                            <a href="{{ site.baseurl }}{{ file.path }}" target="_blank" class="resource-tag">
                                Download PDF
                            </a>
                        </div>
                    </div>
                {% endif %}
            {% endif %}
        {% endfor %}

    {% endfor %}

    {% if library_files.size == 0 %}
        <div style="padding: 20px; text-align: center; color: #666;">
            <p>No notes found yet. Upload a PDF to your <b>university-notes</b> GitHub repo to see it appear here!</p>
        </div>
    {% endif %}

</div>