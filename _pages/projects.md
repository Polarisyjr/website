---
layout: page
title: Academics
permalink: /academics/
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
hide_title: true
---

<!-- pages/projects.md -->
<div class="academics">
  
  <div class="coursework-section">
    <h2 class="section-title">Academics and Coursework</h2>
    
    <h3 style="color: #666; font-size: 1.2rem; margin-bottom: 0.5rem;">Selected List of Courses Taken</h3>
    <p style="font-style: italic; color: #888; margin-bottom: 2rem;">All courses taken at the University of Michigan.</p>
    
    <div class="table-responsive">
      <table class="table table-bordered">
        <thead style="background-color: #f8e8e8;">
          <tr>
            <th style="font-weight: bold;">Course Number</th>
            <th style="font-weight: bold;">Course Title</th>
            <th style="font-weight: bold;">Grade</th>
            <th style="font-weight: bold;">Semester Taken</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>EECS 443</td>
            <td>Honors Thesis</td>
            <td>Present</td>
            <td>Fall 2025</td>
          </tr>
          <tr>
            <td>EECS 570</td>
            <td>Parallel Computer Architecture</td>
            <td>A</td>
            <td>Winter 2025</td>
          </tr>
          <tr>
            <td>EECS 573</td>
            <td>Microarchitecture</td>
            <td>A</td>
            <td>Winter 2025</td>
          </tr>
          <tr>
            <td>STATS 526</td>
            <td>Discrete Stochastic Processes</td>
            <td>A-</td>
            <td>Winter 2025</td>
          </tr>
          <tr>
            <td>EECS 470</td>
            <td>Computer Architecture</td>
            <td>A</td>
            <td>Fall 2024</td>
          </tr>
          <tr>
            <td>CSE 582</td>
            <td>Advanced Operating Systems</td>
            <td>A-</td>
            <td>Fall 2024</td>
          </tr>
          <tr>
            <td>DATASCI 451</td>
            <td>Bayesian Data Analysis</td>
            <td>A</td>
            <td>Fall 2024</td>
          </tr>
          <tr>
            <td>EECS 545</td>
            <td>Advanced Machine Learning</td>
            <td>A</td>
            <td>Winter 2024</td>
          </tr>
          <tr>
            <td>ROB 599</td>
            <td>Deep Learning for Robot Perception</td>
            <td>A</td>
            <td>Winter 2024</td>
          </tr>
          <tr>
            <td>EECS 442</td>
            <td>Computer Vision</td>
            <td>A</td>
            <td>Winter 2024</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
  
  <!-- Original Projects Section -->
  <div class="projects-section" style="margin-top: 3rem;">
    <h2 class="section-title">Projects</h2>
    
    <div class="projects">
    {% if site.enable_project_categories and page.display_categories %}
      <!-- Display categorized projects -->
      {% for category in page.display_categories %}
      <a id="{{ category }}" href=".#{{ category }}">
        <h2 class="category">{{ category }}</h2>
      </a>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <!-- Generate cards for each project -->
      {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-1 row-cols-md-2">
        {% for project in sorted_projects %}
          {% include projects_horizontal.liquid %}
        {% endfor %}
        </div>
      </div>
      {% else %}
      <div class="row row-cols-1 row-cols-md-3">
        {% for project in sorted_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
      {% endif %}
      {% endfor %}

    {% else %}

    <!-- Display projects without categories -->

    {% assign sorted_projects = site.projects | sort: "importance" %}

      <!-- Generate cards for each project -->

    {% if page.horizontal %}

      <div class="container">
        <div class="row row-cols-1 row-cols-md-2">
        {% for project in sorted_projects %}
          {% include projects_horizontal.liquid %}
        {% endfor %}
        </div>
      </div>
      {% else %}
      <div class="row row-cols-1 row-cols-md-3">
        {% for project in sorted_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
      {% endif %}
    {% endif %}
    </div>
  </div>
  
</div>
