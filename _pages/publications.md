---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
/* ─── Publication Card Styles ─────────────────────────────────────── */
.pub-list {
  margin-top: 1.5em;
}

.pub-card {
  display: flex;
  gap: 1.4em;
  padding: 1.4em 1.6em;
  margin-bottom: 1.6em;
  border: 1px solid #e3e8ef;
  border-radius: 10px;
  background: #fff;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  transition: box-shadow 0.2s ease, transform 0.2s ease;
  position: relative;
}

.pub-card:hover {
  box-shadow: 0 4px 18px rgba(0,0,0,0.10);
  transform: translateY(-2px);
}

/* venue badge on left */
.pub-venue-badge {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  min-width: 64px;
  padding-top: 0.2em;
}

.pub-venue-label {
  font-size: 0.72em;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  padding: 0.28em 0.6em;
  border-radius: 5px;
  text-align: center;
  line-height: 1.3;
  white-space: nowrap;
}

.venue-cvpr {
  background: #1565c0;
  color: #fff;
}

.venue-arxiv {
  background: #b71c1c;
  color: #fff;
}

.pub-year {
  font-size: 0.78em;
  color: #888;
  margin-top: 0.45em;
  font-weight: 500;
}

/* right content */
.pub-content {
  flex: 1;
  min-width: 0;
}

.pub-title {
  font-size: 1.05em;
  font-weight: 700;
  color: #1a1a2e;
  margin: 0 0 0.35em 0;
  line-height: 1.4;
}

.pub-title a {
  color: inherit;
  text-decoration: none;
}

.pub-title a:hover {
  color: #1565c0;
  text-decoration: underline;
}

.pub-authors {
  font-size: 0.88em;
  color: #444;
  margin-bottom: 0.3em;
  line-height: 1.5;
}

.pub-authors .me {
  font-weight: 700;
  color: #1a1a2e;
}

.pub-venue-line {
  font-size: 0.88em;
  color: #555;
  font-style: italic;
  margin-bottom: 0.55em;
}

.pub-topics {
  margin-bottom: 0.65em;
  display: flex;
  flex-wrap: wrap;
  gap: 0.35em;
}

.pub-tag {
  font-size: 0.74em;
  padding: 0.18em 0.6em;
  border-radius: 20px;
  background: #f0f4ff;
  color: #3949ab;
  border: 1px solid #c5cae9;
  font-weight: 500;
}

/* abstract toggle */
.pub-abstract-toggle {
  font-size: 0.82em;
  color: #1565c0;
  cursor: pointer;
  user-select: none;
  display: inline-flex;
  align-items: center;
  gap: 0.3em;
  margin-bottom: 0.4em;
  background: none;
  border: none;
  padding: 0;
  font-family: inherit;
}

.pub-abstract-toggle:hover {
  text-decoration: underline;
}

.pub-abstract {
  display: none;
  font-size: 0.85em;
  color: #555;
  line-height: 1.65;
  background: #f8f9fb;
  border-left: 3px solid #1565c0;
  padding: 0.7em 0.9em;
  border-radius: 0 5px 5px 0;
  margin: 0.4em 0 0.6em 0;
}

.pub-abstract.open {
  display: block;
}

/* links */
.pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5em;
  margin-top: 0.55em;
}

.pub-btn {
  font-size: 0.79em;
  padding: 0.28em 0.75em;
  border-radius: 5px;
  text-decoration: none !important;
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  gap: 0.3em;
  transition: background 0.15s, color 0.15s;
}

.pub-btn-arxiv {
  background: #fce4ec;
  color: #c62828;
  border: 1px solid #ef9a9a;
}

.pub-btn-arxiv:hover {
  background: #c62828;
  color: #fff;
}

.pub-btn-pdf {
  background: #e8f5e9;
  color: #2e7d32;
  border: 1px solid #a5d6a7;
}

.pub-btn-pdf:hover {
  background: #2e7d32;
  color: #fff;
}

/* section header */
.pub-section-title {
  font-size: 1.05em;
  font-weight: 700;
  color: #666;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  border-bottom: 2px solid #e0e0e0;
  padding-bottom: 0.4em;
  margin: 2em 0 1em 0;
}

@media (max-width: 600px) {
  .pub-card { flex-direction: column; gap: 0.7em; }
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

<div class="pub-list">

<div class="pub-section-title">2025 – 2026</div>

<!-- ── DiG ──────────────────────────────────────────── -->
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
      <span style="font-size:0.85em;color:#888;"> &nbsp;(* equal contribution)</span>
    </div>
    <div class="pub-venue-line">
      IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026
    </div>
    <div class="pub-topics">
      <span class="pub-tag">Multimodal LLM</span>
      <span class="pub-tag">Visual Grounding</span>
      <span class="pub-tag">Fine-Grained Perception</span>
      <span class="pub-tag">Computer Vision</span>
    </div>
    <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
    <div class="pub-abstract">
      Multimodal Large Language Models (MLLMs) have achieved impressive performance across various vision-language tasks, yet their fine-grained visual perception and precise spatial reasoning capabilities remain limited. This work introduces <strong>DiG (Differential Grounding)</strong>, a novel proxy task framework where MLLMs learn fine-grained perception by identifying and localizing <em>all</em> differences between similar image pairs, without prior knowledge of the number of differences. To support scalable training, we develop an automated 3D-rendering-based data generation pipeline that produces high-quality paired images with fully controllable differences. Curriculum learning progressively increases complexity from single to multiple differences for stable optimization. Extensive experiments demonstrate that DiG significantly improves model performance across diverse visual perception benchmarks, with learned skills effectively transferring to RefCOCO, RefCOCO+, RefCOCOg, and general multimodal perception benchmarks.
    </div>
    <div class="pub-links">
      <a class="pub-btn pub-btn-arxiv" href="https://arxiv.org/abs/2512.12633" target="_blank">
        📄 arXiv
      </a>
      <a class="pub-btn pub-btn-pdf" href="https://arxiv.org/pdf/2512.12633" target="_blank">
        📑 PDF
      </a>
    </div>
  </div>
</div>

<!-- ── FPEdit ─────────────────────────────────────────── -->
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
    <div class="pub-venue-line">
      arXiv preprint arXiv:2508.02092, 2025
    </div>
    <div class="pub-topics">
      <span class="pub-tag">LLM Security</span>
      <span class="pub-tag">Model Fingerprinting</span>
      <span class="pub-tag">Knowledge Editing</span>
      <span class="pub-tag">Model Protection</span>
    </div>
    <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
    <div class="pub-abstract">
      Large language models represent significant investments in computation, data, and engineering expertise, making them extraordinarily valuable intellectual assets. Nevertheless, these AI assets remain vulnerable to unauthorized redistribution and commercial exploitation through fine-tuning or black-box deployment. We introduce <strong>FPEdit</strong>, a novel framework that leverages knowledge editing to inject semantically coherent natural language fingerprints through sparse, targeted modifications to model weights. Our approach introduces <strong>Promote-Suppress Value Vector Optimization</strong>, which simultaneously enhances target token likelihood while suppressing competing tokens, ensuring robust fingerprint integration without degrading core model functionality. FPEdit achieves 95–100% fingerprint retention under both full-parameter fine-tuning and parameter-efficient adaptation, remains robust under quantization, pruning, and stochastic decoding, and can embed 10 fingerprint pairs into LLaMA2-7B in under 2 minutes using less than 30 GB of GPU memory.
    </div>
    <div class="pub-links">
      <a class="pub-btn pub-btn-arxiv" href="https://arxiv.org/abs/2508.02092" target="_blank">
        📄 arXiv
      </a>
      <a class="pub-btn pub-btn-pdf" href="https://arxiv.org/pdf/2508.02092" target="_blank">
        📑 PDF
      </a>
    </div>
  </div>
</div>

</div>
