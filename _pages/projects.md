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
    <h2 class="section-title" style="font-weight: bold;">Academics and Coursework</h2>
    
    <h3 style="color: #666; font-size: 1.2rem; margin-bottom: 0.5rem; font-weight: 600;">Selected List of Courses Taken</h3>
    <p style="font-style: italic; color: #888; margin-bottom: 2rem;">All courses taken at the University of Michigan.</p>
    
    <div class="table-responsive">
      <table class="table table-bordered" style="line-height: 1.2;">
      <style>
        .table td, .table th {
          padding: 0.5rem !important;
          vertical-align: middle;
        }
      </style>
        <thead>
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
            <td>--</td>
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
    
    <!-- Course Projects Section -->
    <div style="margin-top: 3rem;">
      <h3 style="color: #666; font-size: 1.2rem; margin-bottom: 0.5rem; font-weight: 600;">Course Projects</h3>
      <p style="font-style: italic; color: #888; margin-bottom: 2rem;">Selected projects from academic coursework.</p>
      
      <div class="course-projects">
        <div class="course-project-item" style="margin-bottom: 1.5rem; padding: 1rem; border-left: 3px solid #ddd;">
          <div>
            <h4 style="margin-bottom: 0.5rem; font-weight: 600;"><a href="{{ '/assets/pdf/EECS_470_Final_Report.pdf' | relative_url }}" target="_blank" style="text-decoration:none; color:inherit;">A-SOUL: Advanced n-way Superscalar Out-of-order Unified Logic design</a></h4>
            <p style="color: #666; font-size: 0.9rem; margin-bottom: 0.75rem;">EECS 470 - Computer Architecture</p>
            <p style="margin-bottom: 0;">Brief description of the project and key achievements.</p>
            <img src="{{ '/assets/img/Project_Architecture.png' | relative_url }}" alt="project architecture" style="width:100%; max-width:460px; height:auto; object-fit:cover; border-radius:4px; margin-top:0.85rem;"/>
          </div>
        </div>
        
        <div class="course-project-item" style="margin-bottom: 1.5rem; padding: 1rem; border-left: 3px solid #ddd; display:flex; gap:1rem; align-items:flex-start;">
          <img src="{{ '/assets/img/Project_Architecture.png' | relative_url }}" alt="project architecture" style="width:180px; height:auto; object-fit:cover; border-radius:4px;"/>
          <div>
            <h4 style="margin-bottom: 0.5rem; font-weight: 600;"><a href="{{ '/assets/pdf/582_final_report.pdf' | relative_url }}" target="_blank" style="text-decoration:none; color:inherit;">WriteBoost RCU: an Enhanced RCU Library that provides an RCU-centric Update-side Synchronization Mechanism</a></h4>
            <p style="color: #666; font-size: 0.9rem; margin-bottom: 0.5rem;">CSE 582 - Advanced Operating Systems</p>
            <p style="margin-bottom: 0;">Brief description of the project and key achievements.</p>
          </div>
        </div>

      </div>
    </div>
  </div>
  
  <!-- Original Projects Section -->
  <!-- {% comment %}-->
  <div class="projects-section" style="margin-top: 3rem;">
    <h2 class="section-title">Projects</h2>
    
    <div class="projects">
    {% if site.enable_project_categories and page.display_categories %}
      {% for category in page.display_categories %}
      <a id="{{ category }}" href=".#{{ category }}">
        <h2 class="category">{{ category }}</h2>
      </a>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
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

    {% assign sorted_projects = site.projects | sort: "importance" %}

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
  <!-- {% endcomment %}-->
  
</div>
