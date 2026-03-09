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
/* ── Global ──────────────────────────────────────────────────── */
.academic-home {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  color: #222;
  max-width: 860px;
}

/* ── Section headers ─────────────────────────────────────────── */
.section-header {
  display: flex;
  align-items: center;
  gap: 0.55em;
  margin: 2.2em 0 1em 0;
}
.section-header h2 {
  font-size: 1.15em;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #1a1a2e;
  margin: 0;
  border: none;
  padding: 0;
}
.section-header .section-line {
  flex: 1;
  height: 2px;
  background: linear-gradient(to right, #3949ab, transparent);
  border-radius: 2px;
}

/* ── Bio ─────────────────────────────────────────────────────── */
.bio-block {
  font-size: 1em;
  line-height: 1.85;
  color: #333;
  padding: 0.2em 0 0.5em 0;
}
.bio-block a {
  color: #3949ab;
  text-decoration: none;
  border-bottom: 1px solid #c5cae9;
}
.bio-block a:hover {
  border-bottom-color: #3949ab;
}

/* ── Research Interests ──────────────────────────────────────── */
.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(190px, 1fr));
  gap: 0.75em;
  margin-top: 0.5em;
}
.research-item {
  display: flex;
  align-items: flex-start;
  gap: 0.6em;
  padding: 0.75em 1em;
  border: 1px solid #e3e8ef;
  border-radius: 8px;
  background: #fafbff;
  transition: box-shadow 0.18s, transform 0.18s;
}
.research-item:hover {
  box-shadow: 0 3px 12px rgba(57,73,171,0.12);
  transform: translateY(-2px);
}
.research-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #3949ab;
  margin-top: 0.42em;
  flex-shrink: 0;
}
.research-text {
  font-size: 0.88em;
  font-weight: 600;
  color: #1a1a2e;
  line-height: 1.4;
}
.research-sub {
  font-size: 0.76em;
  color: #777;
  font-weight: 400;
  margin-top: 0.15em;
}

/* ── Publications ────────────────────────────────────────────── */
.pub-list { margin-top: 0.5em; }

.pub-card {
  display: flex;
  gap: 1.2em;
  padding: 1.2em 1.4em;
  margin-bottom: 1.2em;
  border: 1px solid #e3e8ef;
  border-radius: 10px;
  background: #fff;
  box-shadow: 0 2px 8px rgba(0,0,0,0.04);
  transition: box-shadow 0.2s ease, transform 0.2s ease;
}
.pub-card:hover {
  box-shadow: 0 4px 18px rgba(0,0,0,0.10);
  transform: translateY(-2px);
}
.pub-venue-badge {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  min-width: 60px;
  padding-top: 0.15em;
}
.pub-venue-label {
  font-size: 0.70em;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  padding: 0.28em 0.55em;
  border-radius: 5px;
  text-align: center;
  line-height: 1.3;
  white-space: nowrap;
}
.venue-cvpr  { background: #1565c0; color: #fff; }
.venue-arxiv { background: #b71c1c; color: #fff; }
.pub-year {
  font-size: 0.76em;
  color: #999;
  margin-top: 0.4em;
  font-weight: 500;
}
.pub-content { flex: 1; min-width: 0; }
.pub-title {
  font-size: 0.98em;
  font-weight: 700;
  color: #1a1a2e;
  margin: 0 0 0.3em 0;
  line-height: 1.45;
}
.pub-title a {
  color: inherit;
  text-decoration: none;
}
.pub-title a:hover { color: #1565c0; text-decoration: underline; }
.pub-authors {
  font-size: 0.85em;
  color: #555;
  margin-bottom: 0.25em;
  line-height: 1.5;
}
.pub-authors .me { font-weight: 700; color: #1a1a2e; }
.pub-venue-line {
  font-size: 0.84em;
  color: #666;
  font-style: italic;
  margin-bottom: 0.5em;
}
.pub-topics {
  display: flex;
  flex-wrap: wrap;
  gap: 0.3em;
  margin-bottom: 0.55em;
}
.pub-tag {
  font-size: 0.72em;
  padding: 0.16em 0.55em;
  border-radius: 20px;
  background: #f0f4ff;
  color: #3949ab;
  border: 1px solid #c5cae9;
  font-weight: 500;
}
.pub-abstract-toggle {
  font-size: 0.80em;
  color: #1565c0;
  cursor: pointer;
  user-select: none;
  display: inline-flex;
  align-items: center;
  gap: 0.3em;
  margin-bottom: 0.35em;
  background: none;
  border: none;
  padding: 0;
  font-family: inherit;
}
.pub-abstract-toggle:hover { text-decoration: underline; }
.pub-abstract {
  display: none;
  font-size: 0.83em;
  color: #555;
  line-height: 1.65;
  background: #f8f9fb;
  border-left: 3px solid #1565c0;
  padding: 0.65em 0.85em;
  border-radius: 0 5px 5px 0;
  margin: 0.35em 0 0.5em 0;
}
.pub-abstract.open { display: block; }
.pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.45em;
  margin-top: 0.5em;
}
.pub-btn {
  font-size: 0.77em;
  padding: 0.25em 0.7em;
  border-radius: 5px;
  text-decoration: none !important;
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  gap: 0.28em;
  transition: background 0.15s, color 0.15s;
}
.pub-btn-arxiv { background:#fce4ec; color:#c62828; border:1px solid #ef9a9a; }
.pub-btn-arxiv:hover { background:#c62828; color:#fff; }
.pub-btn-pdf   { background:#e8f5e9; color:#2e7d32; border:1px solid #a5d6a7; }
.pub-btn-pdf:hover   { background:#2e7d32; color:#fff; }

/* ── Education timeline ──────────────────────────────────────── */
.edu-timeline { margin-top: 0.5em; padding-left: 0.2em; }
.edu-item {
  display: flex;
  gap: 1.1em;
  margin-bottom: 1.1em;
  align-items: flex-start;
}
.edu-dot-col {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 0.35em;
}
.edu-dot {
  width: 11px;
  height: 11px;
  border-radius: 50%;
  background: #3949ab;
  border: 2px solid #fff;
  box-shadow: 0 0 0 2px #3949ab;
  flex-shrink: 0;
}
.edu-line {
  width: 2px;
  flex: 1;
  min-height: 28px;
  background: linear-gradient(to bottom, #c5cae9, transparent);
  margin-top: 4px;
}
.edu-item:last-child .edu-line { display: none; }
.edu-body { flex: 1; padding-bottom: 0.2em; }
.edu-period {
  font-size: 0.78em;
  color: #888;
  font-weight: 500;
  margin-bottom: 0.18em;
}
.edu-degree {
  font-size: 0.95em;
  font-weight: 700;
  color: #1a1a2e;
  margin-bottom: 0.1em;
}
.edu-school {
  font-size: 0.85em;
  color: #555;
}
.edu-school a { color: #3949ab; text-decoration: none; border-bottom: 1px solid #c5cae9; }
.edu-school a:hover { border-bottom-color: #3949ab; }

/* ── Awards ──────────────────────────────────────────────────── */
.awards-list { margin-top: 0.5em; }
.award-item {
  display: flex;
  align-items: baseline;
  gap: 0.8em;
  padding: 0.55em 0.9em;
  margin-bottom: 0.45em;
  border-radius: 7px;
  background: #fafbff;
  border-left: 3px solid #3949ab;
  font-size: 0.9em;
}
.award-item.highlight {
  background: #fffde7;
  border-left-color: #f9a825;
}
.award-year {
  font-size: 0.78em;
  color: #888;
  font-weight: 600;
  min-width: 34px;
}
.award-name { color: #333; line-height: 1.4; }
.award-badge {
  font-size: 0.72em;
  font-weight: 700;
  background: #f9a825;
  color: #fff;
  padding: 0.1em 0.45em;
  border-radius: 4px;
  margin-left: 0.3em;
  white-space: nowrap;
}

/* ── Misc ────────────────────────────────────────────────────── */
@media (max-width: 600px) {
  .research-grid { grid-template-columns: 1fr 1fr; }
  .pub-card { flex-direction: column; gap: 0.6em; }
  .pub-venue-badge { flex-direction: row; gap: 0.6em; align-items: center; }
}
</style>

<script>
function toggleAbstract(btn) {
  var abs = btn.nextElementSibling;
  if (abs.classList.contains('open')) {
    abs.classList.remove('open');
    btn.innerHTML = '▸ Abstract';
  } else {
    abs.classList.add('open');
    btn.innerHTML = '▾ Abstract';
  }
}
</script>

<div class="academic-home">

<!-- ═══════════════════════════════════════════════════════
     BIO
════════════════════════════════════════════════════════ -->
<div class="bio-block">
  I am <strong>Shida Wang (王世炟)</strong>, an M.S. student at the
  <a href="http://sds.ustc.edu.cn/main.htm" target="_blank">School of Artificial Intelligence and Data Science</a>,
  <a href="https://www.ustc.edu.cn/" target="_blank">University of Science and Technology of China (USTC)</a>,
  advised by <a href="http://staff.ustc.edu.cn/~linlixu/" target="_blank">Prof. Linli Xu</a>.
  My research spans <strong>Multimodal Large Language Models</strong>, <strong>Video Understanding</strong>,
  <strong>Token Compression</strong>, and <strong>LLM Security</strong>.
  I am broadly interested in building efficient and trustworthy vision-language systems.
  Outside research, I enjoy basketball and R&amp;B music.
</div>

<!-- ═══════════════════════════════════════════════════════
     RESEARCH INTERESTS
════════════════════════════════════════════════════════ -->
<div class="section-header">
  <h2>Research Interests</h2>
  <div class="section-line"></div>
</div>

<div class="research-grid">
  <div class="research-item">
    <div class="research-dot"></div>
    <div>
      <div class="research-text">Multimodal LLMs</div>
      <div class="research-sub">Fine-grained perception &amp; visual grounding</div>
    </div>
  </div>
  <div class="research-item">
    <div class="research-dot"></div>
    <div>
      <div class="research-text">Video Understanding</div>
      <div class="research-sub">Temporal reasoning &amp; video-language models</div>
    </div>
  </div>
  <div class="research-item">
    <div class="research-dot"></div>
    <div>
      <div class="research-text">Token Compression</div>
      <div class="research-sub">Efficient inference for vision-language models</div>
    </div>
  </div>
  <div class="research-item">
    <div class="research-dot"></div>
    <div>
      <div class="research-text">LLM Security</div>
      <div class="research-sub">Model fingerprinting &amp; IP protection</div>
    </div>
  </div>
</div>

<!-- ═══════════════════════════════════════════════════════
     PUBLICATIONS
════════════════════════════════════════════════════════ -->
<div class="section-header">
  <h2>Publications</h2>
  <div class="section-line"></div>
</div>

<div class="pub-list">

  <!-- DTC -->
  <div class="pub-card">
    <div class="pub-venue-badge">
      <span class="pub-venue-label venue-arxiv">arXiv</span>
      <span class="pub-year">2025</span>
    </div>
    <div class="pub-content">
      <div class="pub-title">
        Dynamic Token Compression for Efficient Video Understanding through Reinforcement Learning
      </div>
      <div class="pub-authors">
        <span class="me">Shida Wang*</span>,&nbsp;Yongxiang Hua*,&nbsp;Zhou Tao,&nbsp;Haoyu Cao,&nbsp;Linli Xu
        <span style="font-size:0.84em;color:#999;">&nbsp;(* equal contribution)</span>
      </div>
      <div class="pub-venue-line">Preprint, 2025</div>
      <div class="pub-topics">
        <span class="pub-tag">Video Understanding</span>
        <span class="pub-tag">Token Compression</span>
        <span class="pub-tag">Reinforcement Learning</span>
        <span class="pub-tag">Efficient Inference</span>
      </div>
      <div style="font-size:0.82em;color:#999;font-style:italic;margin-top:0.3em;">📌 Paper coming soon</div>
    </div>
  </div>

  <!-- TableMix -->
  <div class="pub-card">
    <div class="pub-venue-badge">
      <span class="pub-venue-label venue-cvpr">CVPR<br>2026</span>
      <span class="pub-year">2025</span>
    </div>
    <div class="pub-content">
      <div class="pub-title">
        TableMix: Enhancing Multimodal Table Reasoning in MLLMs from a Data-Centric Perspective
      </div>
      <div class="pub-authors">
        Chaohu Liu,&nbsp;<span class="me">Shida Wang</span>,&nbsp;Yubo Wang,&nbsp;Linli Xu
      </div>
      <div class="pub-venue-line">IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026</div>
      <div class="pub-topics">
        <span class="pub-tag">Multimodal LLM</span>
        <span class="pub-tag">Table Reasoning</span>
        <span class="pub-tag">Data-Centric AI</span>
      </div>
      <div style="font-size:0.82em;color:#999;font-style:italic;margin-top:0.3em;">📌 Paper coming soon</div>
    </div>
  </div>

  <!-- DiG -->
  <div class="pub-card">
    <div class="pub-venue-badge">
      <span class="pub-venue-label venue-cvpr">CVPR<br>2026</span>
      <span class="pub-year">2025</span>
    </div>
    <div class="pub-content">
      <div class="pub-title">
        <a href="https://arxiv.org/abs/2512.12633" target="_blank">
          DiG: Differential Grounding for Enhancing Fine-Grained Perception in Multimodal Large Language Model
        </a>
      </div>
      <div class="pub-authors">
        Zhou Tao*,&nbsp;<span class="me">Shida Wang*</span>,&nbsp;Yongxiang Hua,&nbsp;Haoyu Cao,&nbsp;Linli Xu
        <span style="font-size:0.84em;color:#999;">&nbsp;(* equal contribution)</span>
      </div>
      <div class="pub-venue-line">IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026</div>
      <div class="pub-topics">
        <span class="pub-tag">Multimodal LLM</span>
        <span class="pub-tag">Visual Grounding</span>
        <span class="pub-tag">Fine-Grained Perception</span>
      </div>
      <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
      <div class="pub-abstract">
        Multimodal Large Language Models (MLLMs) have achieved impressive performance across various vision-language tasks, yet their fine-grained visual perception and precise spatial reasoning capabilities remain limited. This work introduces <strong>DiG (Differential Grounding)</strong>, a novel proxy task framework where MLLMs learn fine-grained perception by identifying and localizing <em>all</em> differences between similar image pairs, without prior knowledge of the number of differences. To support scalable training, we develop an automated 3D-rendering-based data generation pipeline and employ curriculum learning for stable optimization. DiG significantly improves model performance on RefCOCO, RefCOCO+, RefCOCOg, and general multimodal perception benchmarks.
      </div>
      <div class="pub-links">
        <a class="pub-btn pub-btn-arxiv" href="https://arxiv.org/abs/2512.12633" target="_blank">📄 arXiv</a>
        <a class="pub-btn pub-btn-pdf"   href="https://arxiv.org/pdf/2512.12633"  target="_blank">📑 PDF</a>
      </div>
    </div>
  </div>

  <!-- FPEdit -->
  <div class="pub-card">
    <div class="pub-venue-badge">
      <span class="pub-venue-label venue-arxiv">arXiv</span>
      <span class="pub-year">2025</span>
    </div>
    <div class="pub-content">
      <div class="pub-title">
        <a href="https://arxiv.org/abs/2508.02092" target="_blank">
          FPEdit: Robust LLM Fingerprinting through Localized Parameter Editing
        </a>
      </div>
      <div class="pub-authors">
        <span class="me">Shida Wang</span>,&nbsp;Chaohu Liu,&nbsp;Yubo Wang,&nbsp;Linli Xu
      </div>
      <div class="pub-venue-line">arXiv preprint arXiv:2508.02092, 2025</div>
      <div class="pub-topics">
        <span class="pub-tag">LLM Security</span>
        <span class="pub-tag">Model Fingerprinting</span>
        <span class="pub-tag">Knowledge Editing</span>
      </div>
      <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
      <div class="pub-abstract">
        We introduce <strong>FPEdit</strong>, a novel framework that leverages knowledge editing to inject semantically coherent natural language fingerprints through sparse, targeted modifications to model weights. Our Promote-Suppress Value Vector Optimization achieves 95–100% fingerprint retention under full-parameter fine-tuning and parameter-efficient adaptation, remaining robust under quantization, pruning, and stochastic decoding. FPEdit embeds 10 fingerprint pairs into LLaMA2-7B in under 2 minutes using less than 30 GB GPU memory.
      </div>
      <div class="pub-links">
        <a class="pub-btn pub-btn-arxiv" href="https://arxiv.org/abs/2508.02092" target="_blank">📄 arXiv</a>
        <a class="pub-btn pub-btn-pdf"   href="https://arxiv.org/pdf/2508.02092"  target="_blank">📑 PDF</a>
      </div>
    </div>
  </div>

</div>

<!-- ═══════════════════════════════════════════════════════
     EDUCATION
════════════════════════════════════════════════════════ -->
<div class="section-header">
  <h2>Education</h2>
  <div class="section-line"></div>
</div>

<div class="edu-timeline">

  <div class="edu-item">
    <div class="edu-dot-col">
      <div class="edu-dot"></div>
      <div class="edu-line"></div>
    </div>
    <div class="edu-body">
      <div class="edu-period">Sept. 2024 – Present</div>
      <div class="edu-degree">M.S. in Artificial Intelligence</div>
      <div class="edu-school">
        <a href="https://www.ustc.edu.cn/" target="_blank">University of Science and Technology of China (USTC)</a>
        &nbsp;·&nbsp; School of Artificial Intelligence and Data Science, Hefei, China
      </div>
    </div>
  </div>

  <div class="edu-item">
    <div class="edu-dot-col">
      <div class="edu-dot"></div>
      <div class="edu-line"></div>
    </div>
    <div class="edu-body">
      <div class="edu-period">Sept. 2021 – July 2024</div>
      <div class="edu-degree">B.S. in Big Data</div>
      <div class="edu-school">
        <a href="https://www.ustc.edu.cn/" target="_blank">University of Science and Technology of China (USTC)</a>
        &nbsp;·&nbsp; School of Big Data, Hefei, China
      </div>
    </div>
  </div>

  <div class="edu-item">
    <div class="edu-dot-col">
      <div class="edu-dot"></div>
    </div>
    <div class="edu-body">
      <div class="edu-period">Sept. 2020 – July 2021</div>
      <div class="edu-degree">B.S. in Management (transferred)</div>
      <div class="edu-school">
        <a href="https://www.ustc.edu.cn/" target="_blank">University of Science and Technology of China (USTC)</a>
        &nbsp;·&nbsp; School of Management, Hefei, China
      </div>
    </div>
  </div>



</div>

<!-- ═══════════════════════════════════════════════════════
     HONORS & AWARDS
════════════════════════════════════════════════════════ -->
<div class="section-header">
  <h2>Honors &amp; Awards</h2>
  <div class="section-line"></div>
</div>

<div class="awards-list">
  <div class="award-item highlight">
    <span class="award-year">2023</span>
    <span class="award-name">China Petroleum Scholarship <span class="award-badge">Top 1</span></span>
  </div>
  <div class="award-item">
    <span class="award-year">2023</span>
    <span class="award-name">Soong Ching Ling Future Scholarship</span>
  </div>
  <div class="award-item">
    <span class="award-year">2022</span>
    <span class="award-name">Third Prize, Contemporary Undergraduate Mathematical Contest in Modeling, Anhui Province</span>
  </div>
  <div class="award-item">
    <span class="award-year">2019</span>
    <span class="award-name">First Prize, National High School Mathematics Competition, Jilin Province</span>
  </div>
  <div class="award-item">
    <span class="award-year">2019</span>
    <span class="award-name">Second Prize, National High School Physics Competition, Jilin Province</span>
  </div>
  <div class="award-item">
    <span class="award-year">2019</span>
    <span class="award-name">Second Prize, China Chemistry Olympiad (Preliminary Round), Jilin Province</span>
  </div>
</div>

</div>
