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
        <div class="pub-title"><a href="https://www.sciencedirect.com/science/article/pii/S0968090X26003062" style="text-decoration: none; color: inherit;">Aligning LLM Agents with Human Learning and Adjustment Behavior: A Dual Agent Approach</a></div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin, Manzi Li, Linghao Wang, Zheng Zhu</div>
        <div class="pub-venue">Transportation Research Part C: Emerging Technologies, vol. 191, 105818, 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2510.08873" style="text-decoration: none; color: inherit;">Fengshui: Composable Chiplet Ecosystems &amp; Fine-Grained Neural Network Accelerators Codesign</a></div>
        <div class="pub-authors">Haoran Jin, <strong>Jirong Yang</strong>, Yunpeng Liu, Barry Lyu, Kangqi Zhang, Nathaniel Bleier</div>
        <div class="pub-venue">59th IEEE/ACM International Symposium on Microarchitecture (MICRO), 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2604.13523" style="text-decoration: none; color: inherit;">TensorLift: Automatic Extraction of Tensor-Level ISA Semantics from Accelerator RTL via MLIR Semantic Lifting</a></div>
        <div class="pub-authors">Ruijie Gao, Haoran Jin, <strong>Jirong Yang</strong>, Nathaniel Bleier</div>
        <div class="pub-venue">45th IEEE/ACM International Conference on Computer-Aided Design (ICCAD), 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2606.05405" style="text-decoration: none; color: inherit;">Agents’ Last Exam</a></div>
        <div class="pub-authors">Yiyou Sun, Xinyang Han, Weichen Zhang, &hellip;, <strong>Jirong Yang</strong>, &hellip;, Dawn Song <span style="font-size: 0.8rem; color: #888;">(520 authors)</span></div>
        <div class="pub-venue">arXiv preprint arXiv:2606.05405, 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://crucible.eecs.umich.edu/data/papers/paper-24-%C3%A6sip-%CE%BCarch-aware-asip-isa-co-design-via-program-s.pdf" style="text-decoration: none; color: inherit;">æSIP: µArch-aware ASIP-ISA Co-Design via Program Synthesis, Equality Saturation, and External Don’t Cares</a></div>
        <div class="pub-authors">Haoran Jin<sup>*</sup>, <strong>Jirong Yang</strong><sup>*</sup>, Barry Lyu, Ruijie Gao, Nathaniel Bleier <span style="font-size: 0.8rem; color: #888;">(<sup>*</sup>Equal contribution, alphabetical order)</span></div>
        <div class="pub-venue">ACM/IEEE 53rd Annual International Symposium on Computer Architecture (ISCA), 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2510.09595" style="text-decoration: none; color: inherit;">LiveOIBench: Can Large Language Models Outperform Human Contestants in Informatics Olympiads?</a></div>
        <div class="pub-authors">Kaijian Zou, Aaron Xiong, Yunxiang Zhang, Xinliang Frederick Zhang, Yueqi Ren, <strong>Jirong Yang</strong>, Ayoung Lee, Shitanshu Bhushan, Lu Wang</div>
        <div class="pub-venue">43rd International Conference on Machine Learning (ICML), 2026</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://www.sciencedirect.com/science/article/pii/S3050860625000018" style="text-decoration: none; color: inherit;">Toward LLM-Agent-Based Modeling of Transportation Systems: A Conceptual Framework</a></div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin</div>
        <div class="pub-venue">Artificial Intelligence for Transportation, vol. 1, 100001, 2025</div>
      </li>
      <li class="pub-item">
        <div class="pub-title">LLM-ABM for Transportation: Assessing the Potential of LLM Agents in System Analysis</div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin</div>
        <div class="pub-venue">AI for Urban Planning Workshop @ AAAI, 2025</div>
      </li>
      <!-- <li class="pub-item">
        <div class="pub-title">Scalable Hardware Pruning through Semiformal Verification and Microarchitecture Awareness</div>
        <div class="pub-authors">Please reach out to me if you are interested in reading the full paper or slides.</div>
        <div class="pub-venue">Second author; Under review</div>
      </li> -->
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
