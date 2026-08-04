---
layout: page
permalink: /publications/
title: Publications
#description: Publications
nav: true
nav_order: 2
hide_title: true
---

<div class="research">
  <style>
    /* Ensure proper dark mode support for section title */
    .research .section-title { 
      color: var(--global-text-color);
    }
  </style>
  <h2 class="section-title" style="font-weight: bold;">Publications</h2>

  <div class="pubs-placeholder">
    <ul class="pub-list">
      <li class="pub-item">
        <div class="pub-title">æSIP: µArch-aware ASIP-ISA Co-Design via Program Synthesis, Equality Saturation, and External Don’t Cares</div>
        <div class="pub-authors">Haoran Jin<sup>*</sup>, <strong>Jirong Yang</strong><sup>*</sup>, Barry Lyu, Ruijie Gao, Nathaniel Bleier <span style="font-size: 0.8rem; color: #888;">(<sup>*</sup>Equal contribution, alphabetical order)</span></div>
        <div class="pub-venue">ISCA 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2510.08873" style="text-decoration: none; color: inherit;">Mozart: A Chiplet Ecosystem-Accelerator Codesign Framework for Composable Bespoke Application Specific Integrated Circuits</a></div>
        <div class="pub-authors">Haoran Jin, <strong>Jirong Yang</strong>, Yunpeng Liu, Barry Lyu, Kangqi Zhang, Nathaniel Bleier</div>
        <div class="pub-venue">ArXiv preprint; Under Review at MICRO</div>
      </li>
      <li class="pub-item">
        <div class="pub-title">Scalable Hardware Pruning through Semiformal Verification and Microarchitecture Awareness</div>
        <div class="pub-authors">Please reach out to me if you are interested in reading the full paper or slides.</div>
        <div class="pub-venue">Second author; Under Review at ICCAD</div>
      </li>
      <li class="pub-item">
        <div class="pub-title">LiveOIBench: Can Large Language Models Outperform Human Contestants in Informatics Olympiads?</div>
        <div class="pub-authors">Kaijian Zou, Aaron Xiong, Yunxiang Zhang, Xinliang Frederick Zhang, Yueqi Ren, <strong>Jirong Yang</strong>, Ayoung Lee, Shitanshu Bhushan, Lu Wang</div>
        <div class="pub-venue">Under Review at ICML 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2511.00993" style="text-decoration: none; color: inherit;">Aligning LLM agents with human learning and adjustment behavior: a dual agent approach</a></div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin, Manzi Li, Linghao Wang, Zheng Zhu</div>
        <div class="pub-venue">Preprint; Major Revision, Transportation Research Part C: Emerging Technologies</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://www.sciencedirect.com/science/article/pii/S3050860625000018" style="text-decoration: none; color: inherit;">Toward llm-agent-based modeling of transportation systems: A conceptual framework</a></div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin</div>
        <div class="pub-venue">Artificial Intelligence for Transportation, 2025</div>
      </li>
    </ul>
  </div>

<style>
.pubs-placeholder {
  margin-top: 1rem;
  margin-bottom: 2rem;
  padding: 1rem;
  background: var(--global-bg-color);
  border-left: 3px solid var(--global-theme-color);
  border-radius: 4px;
  border: 1px solid var(--global-divider-color);
}

.pub-list {
  list-style: none;
  margin: 0;
  padding: 0;
}

.pub-item {
  margin-bottom: 1.5rem;
  padding-bottom: 1.5rem;
  border-bottom: 1px solid var(--global-divider-color);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  cursor: pointer;
}

.pub-item:hover {
  transform: scale(1.02);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.pub-item:last-child {
  border-bottom: none;
  margin-bottom: 0;
  padding-bottom: 0;
}

.pub-title {
  font-weight: 500;
  font-size: 1rem;
  color: var(--global-text-color);
  margin-bottom: 0.4rem;
  line-height: 1.4;
}

.pub-authors {
  font-size: 0.9rem;
  color: var(--global-text-color);
  opacity: 0.8;
  margin-bottom: 0.3rem;
}

.pub-authors strong {
  font-weight: 600;
}

.pub-venue {
  font-size: 0.85rem;
  color: var(--global-theme-color);
  font-style: italic;
}
</style>

</div>
