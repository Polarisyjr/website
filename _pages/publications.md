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



  <h3 style="color: #666; font-size: 1.4rem; margin-bottom: 0.5rem; margin-top: 1rem; font-weight: 600;">Domain-Specific Hardware</h3>

  <h4 style="color: #888; font-style: italic; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Application-Specific Integrated Circuit (ASIC)</h4>
  <div class="expandable-content">
    <div class="content-preview">
      <p>Mozart introduces a chiplet ecosystem–accelerator co-design framework that constructs low-cost bespoke ASICs (BASICs) by leveraging operator-level disaggregation and composing accelerators from a reusable chiplet pool, thereby amortizing non-recurring engineering (NRE) costs while preserving high performance.</p>
    </div>
    <div class="content-full" style="display: none;">
      <p>
      During the first half of 2025, I co-developed <strong>Mozart</strong>, a cross-layer co-design framework that rethinks how modern AI accelerators are built. The project was motivated by a key challenge in AI hardware: traditional monolithic ASICs are efficient but expensive to customize, while general-purpose accelerators lack specialization. 
      </p>

      <p>
      To address this, we combined <em>operator-level disaggregation</em>—which maps each neural operator to its most suitable compute and memory subsystem—with <em>chiplet ecosystem co-design</em> that identifies a minimal, reusable pool of chiplets to amortize the non-recurring engineering (NRE) cost of custom silicon. This combination allows bespoke accelerators to achieve both architectural efficiency and economic scalability. 
      </p>

      <p>
      At its core, Mozart employs a hierarchical optimization framework integrating simulated annealing, genetic algorithms, convex-hull–based layer mapping, and constraint programming. Together, these layers co-optimize chiplet selection, tensor fusion, software mapping, and physical design validation under unified energy, latency, and cost objectives—bridging architectural insight with manufacturable, sustainable AI hardware design.
      </p>

      <p> Through this project, I gained a deep understanding of <em>dataflow accelerator</em> such as <strong>Eyeriss</strong> and <strong>Simba</strong>, as well as <em>mapping-space explorer</em> like <strong>Timeloop</strong> and <strong>Scale-sim</strong>. Working on Mozart allowed me to see how design space exploration (DSE) connects architectural abstraction, hardware constraints, and algorithmic optimization into a unified process. It trained me to reason about hardware not just in terms of microarchitecture, but as a multidimensional search problem—balancing performance, energy, and cost under real physical design limits. This experience laid the methodological foundation for my subsequent research in ISA-hardware co-design and domain-specific architecture exploration. </p>
    </div>
    <button class="toggle-btn" onclick="toggleContent(this)">Read More ▼</button>
  </div>

  <div class="pubs-placeholder">
    <h5>Publications</h5>
    <ul class="pub-list">
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2510.08873" style="text-decoration: none; color: inherit;">Mozart: A Chiplet Ecosystem-Accelerator Codesign Framework for Composable Bespoke Application Specific Integrated Circuits</a></div>
        <div class="pub-authors">Haoran Jin, <strong>Jirong Yang</strong>, Yunpeng Liu, Barry Lyu, Kangqi Zhang, Nathaniel Bleier</div>
        <div class="pub-venue">ArXiv preprint; Under Review at ASPLOS</div>
      </li>
    </ul>
  </div>

  <h4 style="color: #888; font-style: italic; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Application-Specific Instruction-set Processor (ASIP)</h4>

  <div class="expandable-content">
    <div class="content-preview">
      <p>
      This project is an ISA–hardware co-design framework that uses e-graph rewriting at the assembly level to derive minimal, application-specific ISA subsets and guide circuit pruning under ISA-aware formal constraints for efficient ASIP generation.
      </p>
    </div>
    <div class="content-full" style="display: none;">
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
    </div>
    <button class="toggle-btn" onclick="toggleContent(this)">Read More ▼</button>
  </div>

  <div class="pubs-placeholder">
    <h5>Publications</h5>
    <ul class="pub-list">
      <li class="pub-item">
        <div class="pub-title">æSIP: µArch-aware ASIP-ISA Co-Design via Program Synthesis, Equality Saturation, and External Don’t Cares</div>
        <div class="pub-authors">Please reach out to me if you are interested in reading the full paper or slides.</div>
        <div class="pub-venue">Co-first author; Under Review at ISCA</div>
      </li>
      <li class="pub-item">
        <div class="pub-title">Scalable Hardware Pruning through Semiformal Verification and Microarchitecture Awareness</div>
        <div class="pub-authors">Please reach out to me if you are interested in reading the full paper or slides.</div>
        <div class="pub-venue">Second author; Under Review at DAC</div>
      </li>
    </ul>
  </div>
  
  <h3 style="color: #666; font-size: 1.4rem; margin-bottom: 0.5rem; margin-top: 1rem; font-weight: 600;">Application</h3>

  <h4 style="color: #888; font-style: italic; font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Agent</h4>

  <div class="expandable-content">
    <div class="content-preview">
      <p>
      Beginning in 2024, I began exploring the potential of LLM agents in problem solving, deep semantic understanding over long contexts, and modeling human behavior within transportation systems. Over time, this exploration led me to shift my focus toward computer architecture.
      </p>
    </div>
    <div class="content-full" style="display: none;">
      <p>
      This is an era defined by artificial intelligence. With the rapid evolution of large language models (LLMs), the boundary between humans and intelligent agents is being continuously reshaped. The release of Stanford's Smallville (Generative Agents, 2023) sparked widespread discussion, drawing attention to LLM-based agents and their potential to reason, plan, and interact like humans. I was no exception.
      </p>

      <p>
      Beginning in 2024, I started exploring the potential of LLM agents—not only in problem solving, but also in deep semantic understanding over long contexts and in modeling human behavior within transportation systems.
      </p>
       
      <p>
      LLMs are transforming the world around us, quietly integrating into our everyday lives. In certain domains, they have already surpassed human performance, yet they still fall short of the ideal artificial general intelligence (AGI) we aspire to build. Motivated by this, I gradually shifted my focus toward computer architecture, aiming to contribute to the foundational infrastructure that empowers the next generation of AI. At the same time, I closely follow cutting-edge AI directions such as neuro-symbolic reasoning and embodied intelligence. 
      </p>

      <p>
      To me, the future of AI is not only about smarter algorithms, but also about efficient and sustainable systems that truly support them.
      </p>
    </div>
    <button class="toggle-btn" onclick="toggleContent(this)">Read More ▼</button>
  </div>

  <div class="pubs-placeholder">
    <h5>Publications</h5>
    <ul class="pub-list">
      <li class="pub-item">
        <div class="pub-title"><a href="https://www.sciencedirect.com/science/article/pii/S3050860625000018" style="text-decoration: none; color: inherit;">Toward llm-agent-based modeling of transportation systems: A conceptual framework</a></div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin</div>
        <div class="pub-venue">Artificial Intelligence for Transportation, 2025</div>
      </li>
      <li class="pub-item">
        <div class="pub-title"><a href="https://arxiv.org/abs/2511.00993" style="text-decoration: none; color: inherit;">Aligning LLM agents with human learning and adjustment behavior: a dual agent approach</a></div>
        <div class="pub-authors">Tianming Liu, <strong>Jirong Yang</strong>, Yafeng Yin, Manzi Li, Linghao Wang, Zheng Zhu</div>
        <div class="pub-venue"> Preprint; Submitted to Transportation Research Part C: Emerging Technologies, 2026</div>
      </li>
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

/* Expandable content styles */
.expandable-content {
  position: relative;
  margin-bottom: 1rem;
}

.expandable-content p {
  text-align: justify;
  text-justify: inter-word;
}

.toggle-btn {
  display: inline-block;
  margin-top: 0.5rem;
  padding: 0.4rem 1rem;
  background: transparent;
  color: #3999b6;
  border: 2px solid #3999b6;
  border-radius: 4px;
  cursor: pointer;
  font-size: 0.9rem;
  transition: all 0.3s ease;
}

.toggle-btn:hover {
  background: #3999b6;
  color: white;
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

</div>