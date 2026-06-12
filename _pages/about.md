---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
/* ── Palette & base ──────────────────────────────────────────── */
:root {
  --ink:    #1a1a1a;
  --body:   #3f3f46;
  --muted:  #9094a0;
  --accent: #3949ab;
  --line:   #ececf0;
  --subtle: #fafbfc;
}
.academic-home {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", sans-serif;
  color: var(--body);
  max-width: 820px;
  font-size: 16px;
  line-height: 1.75;
}
.academic-home a { color: var(--accent); text-decoration: none; }
.academic-home a:hover { text-decoration: underline; }

/* ── Section headers ─────────────────────────────────────────── */
.section-header { margin: 2.8em 0 1.2em 0; }
.section-header h2 {
  font-size: 0.74em;
  font-weight: 700;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--muted);
  margin: 0;
  padding-bottom: 0.7em;
  border: none;
  border-bottom: 1px solid var(--line);
}

/* ── Bio ─────────────────────────────────────────────────────── */
.bio-block {
  color: var(--body);
  padding: 0.4em 0 0.2em 0;
}
.bio-block strong { color: var(--ink); font-weight: 650; }

/* ── Research interests ──────────────────────────────────────── */
.tag-row { display: flex; flex-wrap: wrap; gap: 0.55em; margin-top: 0.2em; }
.tag {
  font-size: 0.84em;
  padding: 0.34em 0.9em;
  border: 1px solid var(--line);
  border-radius: 999px;
  color: var(--body);
  background: var(--subtle);
}

/* ── Publications ────────────────────────────────────────────── */
.pub-item { padding: 1.25em 0; border-top: 1px solid var(--line); }
.pub-item:first-child { border-top: none; padding-top: 0.4em; }
.pub-venue {
  font-size: 0.72em;
  font-weight: 700;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: var(--accent);
  margin-bottom: 0.25em;
}
.pub-title {
  font-size: 1em;
  font-weight: 650;
  color: var(--ink);
  line-height: 1.5;
  margin: 0 0 0.3em 0;
}
.pub-title a { color: inherit; }
.pub-title a:hover { color: var(--accent); }
.pub-authors { font-size: 0.9em; color: var(--body); margin-bottom: 0.1em; }
.pub-authors .me { font-weight: 700; color: var(--ink); }
.pub-note { font-size: 0.85em; color: var(--muted); margin-top: 0.35em; }
.pub-abstract-toggle {
  font-size: 0.82em;
  color: var(--accent);
  cursor: pointer;
  background: none;
  border: none;
  padding: 0;
  margin-top: 0.45em;
  font-family: inherit;
}
.pub-abstract-toggle:hover { text-decoration: underline; }
.pub-abstract {
  display: none;
  font-size: 0.88em;
  color: var(--body);
  line-height: 1.7;
  border-left: 2px solid var(--line);
  padding: 0.3em 0 0.3em 1em;
  margin: 0.6em 0 0.2em 0;
}
.pub-abstract.open { display: block; }
.pub-abstract strong { color: var(--ink); }
.pub-links { display: flex; flex-wrap: wrap; gap: 1em; margin-top: 0.55em; }
.pub-links a { font-size: 0.84em; font-weight: 600; }

/* ── Timeline (education + internships) ──────────────────────── */
.tl { margin-top: 0.4em; }
.tl-item { display: flex; gap: 1em; padding-bottom: 1.3em; }
.tl-item:last-child { padding-bottom: 0.2em; }
.tl-rail { display: flex; flex-direction: column; align-items: center; padding-top: 0.5em; }
.tl-dot {
  width: 8px; height: 8px; border-radius: 50%;
  background: var(--accent); flex-shrink: 0;
}
.tl-line { width: 1px; flex: 1; min-height: 26px; background: var(--line); margin-top: 6px; }
.tl-item:last-child .tl-line { display: none; }
.tl-body { flex: 1; }
.tl-period { font-size: 0.8em; color: var(--muted); }
.tl-role { font-size: 0.96em; font-weight: 650; color: var(--ink); margin: 0.05em 0; }
.tl-org { font-size: 0.88em; color: var(--body); }

/* ── Awards ──────────────────────────────────────────────────── */
.award-row {
  display: flex; align-items: baseline; gap: 1em;
  padding: 0.6em 0; border-top: 1px solid var(--line);
}
.award-row:first-child { border-top: none; }
.award-year { font-size: 0.82em; color: var(--muted); min-width: 38px; flex-shrink: 0; }
.award-name { font-size: 0.92em; color: var(--body); line-height: 1.5; }
.award-name .top { color: var(--accent); font-weight: 700; }

@media (max-width: 600px) {
  .academic-home { font-size: 15px; }
}
</style>

<script>
function toggleAbstract(btn) {
  var abs = btn.nextElementSibling;
  var open = abs.classList.toggle('open');
  btn.innerHTML = (open ? '▾' : '▸') + ' Abstract';
}
</script>

<div class="academic-home">

<!-- ═══════════════ BIO ═══════════════ -->
<div class="bio-block">
  I am <strong>Shida Wang (王世炟)</strong>, an M.S. student at the
  <a href="http://sds.ustc.edu.cn/main.htm" target="_blank">School of Artificial Intelligence and Data Science</a>,
  <a href="https://www.ustc.edu.cn/" target="_blank">University of Science and Technology of China (USTC)</a>,
  advised by <a href="http://staff.ustc.edu.cn/~linlixu/" target="_blank">Prof. Linli Xu</a>.
  My research spans <strong>Multimodal Large Language Models</strong>, <strong>Video Understanding</strong>,
  <strong>Token Compression</strong>, and <strong>LLM Security</strong>, with a focus on building efficient
  and trustworthy vision-language systems. Outside research, I enjoy basketball and R&amp;B music.
</div>

<!-- ═══════════════ RESEARCH INTERESTS ═══════════════ -->
<div class="section-header"><h2>Research Interests</h2></div>
<div class="tag-row">
  <span class="tag">Multimodal LLMs</span>
  <span class="tag">Video Understanding</span>
  <span class="tag">Token Compression</span>
  <span class="tag">Efficient Inference</span>
  <span class="tag">LLM Security</span>
</div>

<!-- ═══════════════ PUBLICATIONS ═══════════════ -->
<div class="section-header"><h2>Publications</h2></div>
<div class="pub-list">

  <!-- SCORE -->
  <div class="pub-item">
    <div class="pub-venue">arXiv 2026</div>
    <div class="pub-title">
      <a href="https://arxiv.org/abs/2603.26365" target="_blank">
        Dynamic Token Compression for Efficient Video Understanding through Reinforcement Learning
      </a>
    </div>
    <div class="pub-authors">
      <span class="me">Shida Wang*</span>, Yongxiang Hua*, Zhou Tao, Haoyu Cao, Linli Xu
      <span style="color:var(--muted);">(* equal contribution)</span>
    </div>
    <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
    <div class="pub-abstract">
      Multimodal Large Language Models have demonstrated remarkable capabilities in video understanding, yet face prohibitive computational costs and performance degradation from "context rot" due to massive visual token redundancy. Existing compression strategies typically rely on heuristics or fixed transformations that are often decoupled from the downstream task objectives. We propose <strong>SCORE</strong> (Surprise-augmented token COmpression via REinforcement learning), a unified framework that learns an adaptive token compression policy. SCORE introduces a lightweight policy network conditioned on a surprise-augmented state representation that incorporates inter-frame residuals to capture temporal dynamics and motion saliency, optimized via a group-wise reinforcement learning scheme with a split-advantage estimator and a static→real two-stage curriculum. SCORE achieves a <strong>16× prefill speedup</strong> while preserving <strong>99.5% of original performance</strong> at a 10% retention ratio.
    </div>
    <div class="pub-links">
      <a href="https://arxiv.org/abs/2603.26365" target="_blank">arXiv</a>
      <a href="https://arxiv.org/pdf/2603.26365" target="_blank">PDF</a>
    </div>
  </div>

  <!-- TableMix -->
  <div class="pub-item">
    <div class="pub-venue">CVPR 2026</div>
    <div class="pub-title">
      TableMix: Enhancing Multimodal Table Reasoning in MLLMs from a Data-Centric Perspective
    </div>
    <div class="pub-authors">
      Chaohu Liu, <span class="me">Shida Wang</span>, Yubo Wang, Linli Xu
    </div>
    <div class="pub-note">📌 Paper coming soon</div>
  </div>

  <!-- DiG -->
  <div class="pub-item">
    <div class="pub-venue">CVPR 2026</div>
    <div class="pub-title">
      <a href="https://arxiv.org/abs/2512.12633" target="_blank">
        DiG: Differential Grounding for Enhancing Fine-Grained Perception in Multimodal Large Language Model
      </a>
    </div>
    <div class="pub-authors">
      Zhou Tao*, <span class="me">Shida Wang*</span>, Yongxiang Hua, Haoyu Cao, Linli Xu
      <span style="color:var(--muted);">(* equal contribution)</span>
    </div>
    <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
    <div class="pub-abstract">
      Multimodal Large Language Models (MLLMs) have achieved impressive performance across vision-language tasks, yet their fine-grained visual perception and precise spatial reasoning remain limited. We introduce <strong>DiG (Differential Grounding)</strong>, a proxy task framework where MLLMs learn fine-grained perception by identifying and localizing <em>all</em> differences between similar image pairs, without prior knowledge of the number of differences. To support scalable training, we develop an automated 3D-rendering-based data generation pipeline and employ curriculum learning for stable optimization. DiG significantly improves performance on RefCOCO, RefCOCO+, RefCOCOg, and general multimodal perception benchmarks.
    </div>
    <div class="pub-links">
      <a href="https://arxiv.org/abs/2512.12633" target="_blank">arXiv</a>
      <a href="https://arxiv.org/pdf/2512.12633" target="_blank">PDF</a>
    </div>
  </div>

  <!-- FPEdit -->
  <div class="pub-item">
    <div class="pub-venue">arXiv 2025</div>
    <div class="pub-title">
      <a href="https://arxiv.org/abs/2508.02092" target="_blank">
        FPEdit: Robust LLM Fingerprinting through Localized Parameter Editing
      </a>
    </div>
    <div class="pub-authors">
      <span class="me">Shida Wang</span>, Chaohu Liu, Yubo Wang, Linli Xu
    </div>
    <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
    <div class="pub-abstract">
      We introduce <strong>FPEdit</strong>, a framework that leverages knowledge editing to inject semantically coherent natural language fingerprints through sparse, targeted modifications to model weights. Our Promote-Suppress Value Vector Optimization achieves 95–100% fingerprint retention under full-parameter fine-tuning and parameter-efficient adaptation, remaining robust under quantization, pruning, and stochastic decoding. FPEdit embeds 10 fingerprint pairs into LLaMA2-7B in under 2 minutes using less than 30 GB GPU memory.
    </div>
    <div class="pub-links">
      <a href="https://arxiv.org/abs/2508.02092" target="_blank">arXiv</a>
      <a href="https://arxiv.org/pdf/2508.02092" target="_blank">PDF</a>
    </div>
  </div>

</div>

<!-- ═══════════════ EXPERIENCE / EDUCATION ═══════════════ -->
<div class="section-header"><h2>Internships</h2></div>
<div class="tl">
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">June 2026 – Present</div>
      <div class="tl-role">dots · Ace Top Intern</div>
      <div class="tl-org">Xiaohongshu (RED) · Shanghai, China</div>
    </div>
  </div>
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">Oct. 2025 – May 2026</div>
      <div class="tl-role">Research Intern</div>
      <div class="tl-org">Tencent Youtu Lab · Hefei, China</div>
    </div>
  </div>
</div>

<div class="section-header"><h2>Education</h2></div>
<div class="tl">
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">Sept. 2024 – Present</div>
      <div class="tl-role">M.S. in Artificial Intelligence</div>
      <div class="tl-org">
        <a href="https://www.ustc.edu.cn/" target="_blank">USTC</a> · School of Artificial Intelligence and Data Science, Hefei
      </div>
    </div>
  </div>
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">Sept. 2021 – July 2024</div>
      <div class="tl-role">B.S. in Artificial Intelligence</div>
      <div class="tl-org">
        <a href="https://www.ustc.edu.cn/" target="_blank">USTC</a> · School of Artificial Intelligence and Data Science, Hefei
      </div>
    </div>
  </div>
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">Sept. 2020 – July 2021</div>
      <div class="tl-role">B.S. in Management (transferred)</div>
      <div class="tl-org">
        <a href="https://www.ustc.edu.cn/" target="_blank">USTC</a> · School of Management, Hefei
      </div>
    </div>
  </div>
</div>

<!-- ═══════════════ HONORS & AWARDS ═══════════════ -->
<div class="section-header"><h2>Honors &amp; Awards</h2></div>
<div class="awards">
  <div class="award-row">
    <span class="award-year">2023</span>
    <span class="award-name">China Petroleum Scholarship <span class="top">· Top 1</span></span>
  </div>
  <div class="award-row">
    <span class="award-year">2023</span>
    <span class="award-name">Soong Ching Ling Future Scholarship</span>
  </div>
  <div class="award-row">
    <span class="award-year">2022</span>
    <span class="award-name">Third Prize, Contemporary Undergraduate Mathematical Contest in Modeling, Anhui Province</span>
  </div>
  <div class="award-row">
    <span class="award-year">2019</span>
    <span class="award-name">First Prize, National High School Mathematics Competition, Jilin Province</span>
  </div>
  <div class="award-row">
    <span class="award-year">2019</span>
    <span class="award-name">Second Prize, National High School Physics Competition, Jilin Province</span>
  </div>
  <div class="award-row">
    <span class="award-year">2019</span>
    <span class="award-name">Second Prize, China Chemistry Olympiad (Preliminary Round), Jilin Province</span>
  </div>
</div>

</div>
