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
    <style>
      /* Force section title to be black on Academics page */
      .academics .section-title { color: #000 !important; }
    </style>
    <h2 class="section-title" style="font-weight: bold;">Academics and Coursework</h2>
    
    <h3 style="color: #666; font-size: 1.4rem; margin-bottom: 0.5rem; margin-top: 1rem; font-weight: 600;">Selected List of Courses Taken</h3>
    <p style="font-style: italic; color: #888; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">All courses taken at the University of Michigan.</p>
    
    <div class="table-responsive">
      <table class="table table-bordered course-table" style="line-height: 1.2;">
      <style>
        .table td, .table th {
          padding: 0.5rem !important;
          vertical-align: middle;
        }
        /* Slightly bolder text for coursework table cells */
        .course-table td { font-weight: 400; }
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
    <div style="margin-top: 1rem;">
      <h3 style="color: #666; font-size: 1.4rem; margin-bottom: 0.5rem; font-weight: 600;">Course Projects</h3>
      <p style="font-style: italic; color: #888; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Selected projects from academic coursework.</p>
      <style>
        /* Make course project titles visibly link-styled (blue + underline on hover) */
        .course-project-item h4 a { color: #3999b6; text-decoration: none; }
        .course-project-item h4 a:hover,
        .course-project-item h4 a:focus { text-decoration: underline; color: #0a58ca; }
      </style>
      
      <div class="course-projects">
        <div class="course-project-item" style="margin-bottom: 1.5rem; padding: 1rem; border-left: 3px solid #ddd;">
          <div>
            <h4 style="margin-bottom: 0.5rem; font-weight: 600;"><a href="{{ '/assets/pdf/EECS_470_Final_Report.pdf' | relative_url }}" target="_blank">A-SOUL: Advanced n-way Superscalar Out-of-order Unified Logic design</a></h4>
            <p style="color: #666; font-size: 0.9rem; margin-bottom: 0.85rem;">EECS 470 - Computer Architecture</p>
            <img class="course-project-img zoomable" src="{{ '/assets/img/Project_Architecture.png' | relative_url }}" alt="project architecture" style="width:100%; max-width:960px; height:auto; object-fit:cover; border-radius:6px; margin:0 0 0.95rem 0; cursor:zoom-in;"/>
            <div class="expandable-content">
              <div class="content-preview">
                <div class="course-project-desc" style="text-align: justify; text-justify: inter-word;">
                  <p style="margin: 0 0 0.95rem 0;">A-SOUL is a fully functional out-of-order RISC-V CPU inspired by the MIPS R10K microarchitecture, featuring a unified RTL-level microarchitecture and a highly modular pipeline design. The project implements n-way superscalar execution, register renaming, speculative load scheduling, precise states, and early branch resolution within a synthesizable SystemVerilog framework.</p>
                </div>
              </div>
              <div class="content-full" style="display: none;">
                <div class="course-project-desc" style="text-align: justify; text-justify: inter-word;">
                  <p style="margin: 0 0 0.95rem 0;">A-SOUL is a fully functional out-of-order RISC-V CPU inspired by the MIPS R10K microarchitecture, featuring a unified RTL-level microarchitecture and a highly modular pipeline design. The project implements n-way superscalar execution, register renaming, speculative load scheduling, precise states, and early branch resolution within a synthesizable SystemVerilog framework.</p>

                  <p style="margin: 0 0 0.95rem 0;">The processor pipeline supports instruction-level parallelism with a multi-issue dispatch stage, a Reservation Station and Reorder Buffer, and a Load-Store Queue (LSQ) capable of byte-level forwarding and non-blocking memory access through an MSHR-based D-Cache. The instruction side incorporates GShare and Tournament branch predictors, return address stack, and a configurable adaptive instruction prefetcher with victim cache for reducing i-cache misses.</p>

                  <p style="margin: 0 0 0.95rem 0;">To improve performance, we designed a speculative LSQ that issues loads before dependent stores are fully resolved, reducing pipeline stalls caused by load/store dependency chains. This optimization alone improved CPI by 0.15 (≈ 8.1%) and eliminated 21 % of issue-stage stalls, bringing the overall average CPI down to ~1.7 at a 7.7 ns clock period after timing closure.</p>

                  <p style="margin: 0;">Beyond RTL design, the project features a robust testing and profiling infrastructure. We developed a top-down, counter-based performance simulator and an automated experiment pipeline for architectural design-space exploration. The framework systematically sweeps key microarchitectural parameters, collects CPI, occupancy, and stall breakdowns, and generates detailed visualizations for bottleneck identification and performance analysis. These tools enabled iterative optimization of critical paths (e.g., ROB/RS sizing, pipeline partitioning) and empirical validation across 20+ C benchmarks against a verified in-order golden model.</p>
                </div>
              </div>
              <button class="toggle-btn" onclick="toggleContent(this)">Read More ▼</button>
            </div>
          </div>
        </div>
        
        <div class="course-project-item" style="margin-bottom: 1.5rem; padding: 1rem; border-left: 3px solid #ddd; display:flex; gap:1rem; align-items:flex-start;">
          <div>
            <h4 style="margin-bottom: 0.5rem; font-weight: 600;"><a href="{{ '/assets/pdf/582_final_report.pdf' | relative_url }}" target="_blank">WriteBoost RCU: an Enhanced RCU Library that provides an RCU-centric Update-side Synchronization Mechanism</a></h4>
            <p style="color: #666; font-size: 0.9rem; margin-bottom: 0.5rem;">CSE 582 - Advanced Operating Systems</p>
            <div class="expandable-content">
              <div class="content-preview">
                <div class="course-project-desc" style="text-align: justify; text-justify: inter-word;">
                  <p style="margin: 0 0 0.95rem 0;">WriteBoost RCU extends the classic Read-Copy-Update (RCU) synchronization mechanism by integrating update-side coordination into the library, eliminating the need for external locks. Compared to liburcu and Folly RCU, it maintains RCU's wait-free reads while simplifying writer logic and improving throughput in balanced workloads.</p>
                </div>
              </div>
              <div class="content-full" style="display: none;">
                <div class="course-project-desc" style="text-align: justify; text-justify: inter-word;">
                  <p style="margin: 0 0 0.95rem 0;">WriteBoost RCU extends the classic Read-Copy-Update (RCU) synchronization mechanism by integrating update-side coordination into the library, eliminating the need for external locks. Compared to liburcu and Folly RCU, it maintains RCU's wait-free reads while simplifying writer logic and improving throughput in balanced workloads.</p>

                  <p style="margin: 0 0 0.95rem 0;">The design introduces a single updater/reclaimer model, batch update processing, and an object pool for memory reuse—together removing retirement-list contention and amortizing copy costs. An epoch-based reader–reclaimer synchronization scheme ensures safe reclamation with amortized O(1) complexity and zero reader contention.</p>

                  <p style="margin: 0;">Evaluated against existing RCU and mutex-based mechanisms, WriteBoost RCU achieved 3.49 B reads/s and 35 M writes/s (8 thread), outperforming Folly RCU by ~1.8× on reads and maintaining competitive write performance. The project demonstrates that RCU can scale effectively beyond read-heavy workloads, combining high programmability with robust multi-core efficiency.</p>
                </div>
              </div>
              <button class="toggle-btn" onclick="toggleContent(this)">Read More ▼</button>
            </div>
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

<!-- Image Lightbox (inline for this page) -->
<style>
  .lightbox-backdrop {position:fixed; inset:0; background:rgba(0,0,0,.65); display:none; align-items:center; justify-content:center; z-index:9999; padding:2rem;}
  .lightbox-backdrop.active {display:flex;}
  .lightbox-content {max-width: min(90vw,1200px); max-height: 90vh; position:relative;}
  .lightbox-content img {width:100%; height:auto; border-radius:6px; box-shadow:0 6px 24px -4px rgba(0,0,0,.4);}   
  .lightbox-close {position:absolute; top:-14px; right:-14px; background:#fff; border-radius:50%; width:34px; height:34px; border:1px solid #ccc; display:flex; align-items:center; justify-content:center; cursor:pointer; font-size:20px; font-weight:600; line-height:1;}
  .lightbox-close:hover {background:#f2f2f2;}
  @media (max-width: 600px){ .lightbox-content {padding:0;}} 
</style>
<div id="lightboxBackdrop" class="lightbox-backdrop" aria-modal="true" role="dialog">
  <div class="lightbox-content">
    <button class="lightbox-close" aria-label="Close" title="Close">×</button>
    <img id="lightboxImage" alt="Expanded project image" />
  </div>
</div>
<script>
(function(){
  const imgs = document.querySelectorAll('.zoomable');
  const backdrop = document.getElementById('lightboxBackdrop');
  const outImg = document.getElementById('lightboxImage');
  const closeBtn = backdrop.querySelector('.lightbox-close');
  function open(src, alt){
    outImg.src = src; outImg.alt = alt || 'project image';
    backdrop.classList.add('active');
    document.body.style.overflow='hidden';
  }
  function close(){
    backdrop.classList.remove('active');
    document.body.style.overflow='';
  }
  imgs.forEach(img=>{
    img.addEventListener('click', ()=> open(img.src, img.alt));
    img.addEventListener('keydown', e=>{ if(e.key==='Enter') open(img.src, img.alt); });
    img.setAttribute('tabindex','0');
    img.setAttribute('role','button');
    img.setAttribute('aria-label','Open image in larger view');
  });
  backdrop.addEventListener('click', e=>{ if(e.target===backdrop) close(); });
  closeBtn.addEventListener('click', close);
  document.addEventListener('keydown', e=>{ if(e.key==='Escape' && backdrop.classList.contains('active')) close(); });
})();
</script>

<!-- Expandable Content Styles and Script -->
<style>
.expandable-content {
  position: relative;
  margin-bottom: 1rem;
}

.toggle-btn {
  display: inline-block;
  margin-top: 0.5rem;
  padding: 0.4rem 1rem;
  background: var(--global-theme-color);
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 0.9rem;
  transition: all 0.3s ease;
}

.toggle-btn:hover {
  opacity: 0.85;
  transform: translateY(-1px);
}

.toggle-btn:active {
  transform: translateY(0);
}
</style>

<script>
function toggleContent(button) {
  const container = button.parentElement;
  const preview = container.querySelector('.content-preview');
  const full = container.querySelector('.content-full');
  
  if (full.style.display === 'none') {
    preview.style.display = 'none';
    full.style.display = 'block';
    button.textContent = 'Show Less ▲';
  } else {
    preview.style.display = 'block';
    full.style.display = 'none';
    button.textContent = 'Read More ▼';
  }
}
</script>
