---
layout: page
title: Academics
permalink: /academics/
description: Academic coursework and project portfolio.
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="academics">
  
  <div class="coursework-section">
    <h2 class="section-title" style="color: #B31B1B; margin-bottom: 1rem;">Academics and Coursework</h2>
    
    <h3 style="color: #666; font-size: 1.2rem; margin-bottom: 0.5rem;">Selected List of Courses Taken</h3>
    <p style="font-style: italic; color: #888; margin-bottom: 2rem;">All courses taken at the University of Michigan.</p>
    
    <div class="table-responsive">
      <table class="table table-bordered">
        <thead style="background-color: #f8e8e8;">
          <tr>
            <th style="font-weight: bold;">Course Number</th>
            <th style="font-weight: bold;">Course Title</th>
            <th style="font-weight: bold;">Instructor</th>
            <th style="font-weight: bold;">Semester Taken</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>EECS 481</td>
            <td>Software Engineering</td>
            <td>Xinyu Wang</td>
            <td>Winter 2024</td>
          </tr>
          <tr>
            <td>MATH 561</td>
            <td>Linear Programming</td>
            <td>Ruiwei Jiang</td>
            <td>Winter 2024</td>
          </tr>
          <tr>
            <td>EECS 573</td>
            <td>Microarchitecture</td>
            <td>Todd Austin</td>
            <td>Fall 2023</td>
          </tr>
          <tr>
            <td>EECS 583</td>
            <td>Advanced Compiler Construction</td>
            <td>Scott Mahlke</td>
            <td>Fall 2023</td>
          </tr>
          <tr>
            <td>CEE 552</td>
            <td>Travel Analysis and Forecasting</td>
            <td>Atiyya Shaw</td>
            <td>Fall 2023</td>
          </tr>
          <tr>
            <td>EECS 470</td>
            <td>Computer Architecture</td>
            <td>Jonathan Beaumont</td>
            <td>Winter 2023</td>
          </tr>
          <tr>
            <td>EECS 442</td>
            <td>Computer Vision</td>
            <td>Andrew Owens</td>
            <td>Fall 2022</td>
          </tr>
          <tr>
            <td>CEE 551</td>
            <td>Traffic Science</td>
            <td>Henry Liu</td>
            <td>Fall 2022</td>
          </tr>
          <tr>
            <td>EECS 388</td>
            <td>Introduction to Computer Security</td>
            <td>Peter Honeyman</td>
            <td>Winter 2022</td>
          </tr>
          <tr>
            <td>CEE 450</td>
            <td>Introduction to Transportation Engineering</td>
            <td>Henry Liu</td>
            <td>Winter 2022</td>
          </tr>
          <tr>
            <td>CEE 375</td>
            <td>Sensors and Circuits</td>
            <td>Jeff Scruggs</td>
            <td>Winter 2022</td>
          </tr>
          <tr>
            <td>ENGR 255</td>
            <td><a href="#" style="color: #007acc;">Introductory Multidisciplinary Engineering Project</a></td>
            <td>Ivo Dinov</td>
            <td>Winter 2021</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
  
  <!-- Original Projects Section -->
  <div class="projects-section" style="margin-top: 3rem;">
    <h2 class="section-title" style="color: #B31B1B; margin-bottom: 1rem;">Projects</h2>
    
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
