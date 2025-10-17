---
layout: page
permalink: /publications/
title: Research
#description: Research experience and publications
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
  <h2 class="section-title" style="font-weight: bold;">Experience and Publications</h2>



  <h3 style="color: #666; font-size: 1.4rem; margin-bottom: 0.5rem; margin-top: 1rem; font-weight: 600;">Domain-Specific Platform</h3>

  <h4 style="color: #888; font-style: italic; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Application-Specific Integrated Circuit (ASIC)</h4>

  <p>针对特定工作负载的专用集成电路设计，聚焦算子映射、存储层次优化与片上互连；在能效/性能/面积权衡下进行体系结构协同优化。</p>

  <div class="pubs-placeholder">
    <h5>Publications</h5>
    <ul class="pub-list">
      <li class="pub-item">
        <div class="pub-title">Mozart: A Chiplet Ecosystem-Accelerator Codesign Framework for Composable Bespoke Application Specific Integrated Circuits</div>
        <div class="pub-authors">Haoran Jin, <strong>Jirong Yang</strong>, Yunpeng Liu, Barry Lyu, Kangqi Zhang, Nathaniel Bleier</div>
        <div class="pub-venue">Preprint, Submitted to ASPLOS 2026</div>
      </li>
    </ul>
  </div>

  <h4 style="color: #888; font-style: italic; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Application-Specific Instruction-set Processor (ASIP)</h4>

  <p>
  Since the summer, I have been working with Prof. Nathaniel Bleier and Ph.D. student Haoran Jin on formal verification methods for external don't-cares. We soon realized that this domain is already quite mature, leaving limited space for new contributions. Around that time, I was introduced to e-graphs and Prof. Bleier's prior work on Property-Driven Automatic Transformation (PDAT), which ultimately inspired my honors thesis project.
  </p>

  <p>
  My honors thesis aims to achieve application-specific ISA subset customization through assembly-level rewriting, followed by constraint-driven hardware trimming under ISA-aware synthesis. The project adopts an ISA–hardware co-design methodology, representing the first attempt to apply e-graphs directly at the assembly level.
  </p>

  <p>
  Building on PDAT's property-driven foundation, we integrated induction-based signal correspondence to prune irrelevant or unreachable circuits. This enhancement delivers over 100× faster runtime while maintaining—or even improving—the result quality compared to the original PDAT framework.
  </p>

  <p>
  Importantly, the system is designed as a general co-design framework, rather than a fixed ASIP generator for a single workload. Once an ISA subset is derived for Application A, the same subset can be used to rewrite and deploy Application B, effectively amortizing the non-recurring engineering (NRE) cost. The framework enables designers to explore Pareto-optimal ISA subsets across performance, power, and area, supporting scalable and workload-aware hardware customization.
  </p>

  <p>
  This project deepened my understanding of traditional computer architecture while revealing that cross-layer co-design principles—often emphasized in modern AI infrastructure—can also advance conventional architectures. It has encouraged me to think about systems holistically, recognizing how interactions across abstraction layers shape performance, scalability, and efficiency.
  </p>

  <div class="pubs-placeholder">
    <h5>Publications</h5>
    <ul class="pub-list">
      <li class="pub-item">
        <div class="pub-title">æSIP: From Equality to Efficiency — ISA-ASIP Co-Design via Equality Saturation</div>
        <div class="pub-authors">Haoran Jin*, <strong>Jirong Yang*</strong>, Ruijie Gao, Nathaniel Bleier <em>(* Equal contribution; authors listed alphabetically.)</em></div>
        <div class="pub-venue">Ongoing Honor Thesis, to be submitted</div>
      </li>
    </ul>
  </div>
  
  <h3 style="color: #666; font-size: 1.4rem; margin-bottom: 0.5rem; margin-top: 1rem; font-weight: 600;">Application</h3>

  <h4 style="color: #888; font-style: italic; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Agent</h4>

  <p>面向复杂环境的智能体系统研究，包括多智能体协作、强化学习与任务/资源调度；关注可泛化的策略学习与可解释的决策流程。</p>

  <div class="pubs-placeholder">
    <h5>Publications</h5>
    <ul class="pub-list">
      <li class="pub-item">
        <div class="pub-title">Toward llm-agent-based modeling of transportation systems: A conceptual framework</div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin</div>
        <div class="pub-venue">Artificial Intelligence for Transportation, 2025</div>
      </li>
      <!-- <li class="pub-item">
        <div class="pub-title">Aligning LLM with human learning and adjustment behavior: a dual agent approach</div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin, Manzi Li, Linghao Wang, Zheng Zhu</div>
        <div class="pub-venue">Submitted to Transportation Research Part C: Emerging Technologies, 2026</div>
      </li> -->
      <li class="pub-item">
        <div class="pub-title">LiveOIBench: Can Large Language Models Outperform Human Contestants in Informatics Olympiads?</div>
        <div class="pub-authors">Kaijian Zou, Aaron Xiong, Yunxiang Zhang, Xinliang Frederick Zhang, Yueqi Ren, <strong>Jirong Yang</strong>, Ayoung Lee, Shitanshu Bhushan, Lu Wang</div>
        <div class="pub-venue">Submitted to ICLR 2026</div>
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

.pubs-placeholder h5 {
  margin: 0 0 1rem 0;
  font-size: 0.95rem;
  color: var(--global-text-color);
  font-weight: 600;
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