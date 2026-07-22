---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<script>
function toggleAbstract(btn) {
  var abs = btn.nextElementSibling;
  var open = abs.classList.toggle('open');
  btn.innerHTML = (open ? '▾' : '▸') + ' Abstract';
}
</script>

<div class="academic-home">

<header class="home-intro">
  <div class="home-kicker">Multimodal Intelligence · Efficient &amp; Trustworthy AI</div>
  <h1>Shida Wang<span>.</span></h1>
  <p class="home-lede">I build efficient and trustworthy vision–language systems, with a focus on video understanding, adaptive token compression, and model security.</p>
  <nav class="home-actions" aria-label="Profile links">
    <a href="#publications">Selected work</a>
    <a href="mailto:wangshida@mail.ustc.edu.cn">Email</a>
    <a href="https://github.com/ShidaWang02" target="_blank" rel="noopener">GitHub</a>
  </nav>
</header>

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

<!-- ═══════════════ NEWS ═══════════════ -->
<div class="section-header"><h2>News</h2></div>
<div class="news-list">
  <div class="news-item">
    <div class="news-date">Jul 2026</div>
    <div class="news-body"><strong>FPEdit</strong> accepted to <strong>COLM 2026</strong>.</div>
  </div>
  <div class="news-item">
    <div class="news-date">Jun 2026</div>
    <div class="news-body">Started as <strong>dots · Ace Top Intern</strong> at Xiaohongshu (RED), Shanghai.</div>
  </div>
  <div class="news-item">
    <div class="news-date">Mar 2026</div>
    <div class="news-body">Released <strong>SCORE</strong> (Dynamic Token Compression for video) on arXiv.</div>
  </div>
  <div class="news-item">
    <div class="news-date">Feb 2026</div>
    <div class="news-body">Two papers (<strong>TableMix</strong>, <strong>DiG</strong>) accepted to <strong>CVPR 2026</strong>.</div>
  </div>
  <div class="news-item">
    <div class="news-date">Oct 2025</div>
    <div class="news-body">Joined <strong>Tencent Youtu Lab</strong> as a Research Intern.</div>
  </div>
  <div class="news-item">
    <div class="news-date">Aug 2025</div>
    <div class="news-body">Released <strong>FPEdit</strong> (robust LLM fingerprinting) on arXiv.</div>
  </div>
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
<div class="section-header" id="publications"><h2>Selected Publications</h2></div>
<div class="pub-list">

  <!-- SCORE -->
  <div class="pub-item">
    <div class="pub-thumb"><img src="/images/pubs/score.png" alt="SCORE teaser"></div>
    <div class="pub-info">
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
      <div class="pub-tldr">An RL-learned policy compresses video tokens for 16× prefill speedup at ~99.5% performance.</div>
      <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
      <div class="pub-abstract">
        Multimodal Large Language Models have demonstrated remarkable capabilities in video understanding, yet face prohibitive computational costs and performance degradation from "context rot" due to massive visual token redundancy. Existing compression strategies typically rely on heuristics or fixed transformations that are often decoupled from the downstream task objectives. We propose <strong>SCORE</strong> (Surprise-augmented token COmpression via REinforcement learning), a unified framework that learns an adaptive token compression policy. SCORE introduces a lightweight policy network conditioned on a surprise-augmented state representation that incorporates inter-frame residuals to capture temporal dynamics and motion saliency, optimized via a group-wise reinforcement learning scheme with a split-advantage estimator and a static→real two-stage curriculum. SCORE achieves a <strong>16× prefill speedup</strong> while preserving <strong>99.5% of original performance</strong> at a 10% retention ratio.
      </div>
      <div class="pub-links">
        <a href="https://arxiv.org/abs/2603.26365" target="_blank">arXiv</a>
        <a href="https://arxiv.org/pdf/2603.26365" target="_blank">PDF</a>
      </div>
    </div>
  </div>

  <!-- TableMix -->
  <div class="pub-item">
    <div class="pub-thumb ph">CVPR<br>2026</div>
    <div class="pub-info">
      <div class="pub-venue">CVPR 2026</div>
      <div class="pub-title">
        <a href="https://openaccess.thecvf.com/content/CVPR2026/papers/Liu_TableMix_Enhancing_Multimodal_Table_Reasoning_in_MLLMs_from_a_Data-Centric_CVPR_2026_paper.pdf" target="_blank">
          TableMix: Enhancing Multimodal Table Reasoning in MLLMs from a Data-Centric Perspective
        </a>
      </div>
      <div class="pub-authors">
        Chaohu Liu, <span class="me">Shida Wang</span>, Yubo Wang, Linli Xu
      </div>
      <div class="pub-tldr">A data-centric augmentation strategy that boosts multimodal table reasoning in MLLMs.</div>
      <div class="pub-links">
        <a href="https://openaccess.thecvf.com/content/CVPR2026/papers/Liu_TableMix_Enhancing_Multimodal_Table_Reasoning_in_MLLMs_from_a_Data-Centric_CVPR_2026_paper.pdf" target="_blank">PDF</a>
        <a href="https://openaccess.thecvf.com/content/CVPR2026/html/Liu_TableMix_Enhancing_Multimodal_Table_Reasoning_in_MLLMs_from_a_Data-Centric_CVPR_2026_paper.html" target="_blank">CVF</a>
      </div>
    </div>
  </div>

  <!-- DiG -->
  <div class="pub-item">
    <div class="pub-thumb"><img src="/images/pubs/dig.png" alt="DiG teaser"></div>
    <div class="pub-info">
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
      <div class="pub-tldr">MLLMs learn fine-grained perception by localizing all differences between similar image pairs.</div>
      <button class="pub-abstract-toggle" onclick="toggleAbstract(this)">▸ Abstract</button>
      <div class="pub-abstract">
        Multimodal Large Language Models (MLLMs) have achieved impressive performance across vision-language tasks, yet their fine-grained visual perception and precise spatial reasoning remain limited. We introduce <strong>DiG (Differential Grounding)</strong>, a proxy task framework where MLLMs learn fine-grained perception by identifying and localizing <em>all</em> differences between similar image pairs, without prior knowledge of the number of differences. To support scalable training, we develop an automated 3D-rendering-based data generation pipeline and employ curriculum learning for stable optimization. DiG significantly improves performance on RefCOCO, RefCOCO+, RefCOCOg, and general multimodal perception benchmarks.
      </div>
      <div class="pub-links">
        <a href="https://arxiv.org/abs/2512.12633" target="_blank">arXiv</a>
        <a href="https://arxiv.org/pdf/2512.12633" target="_blank">PDF</a>
      </div>
    </div>
  </div>

  <!-- FPEdit -->
  <div class="pub-item">
    <div class="pub-thumb"><img src="/images/pubs/fpedit.png" alt="FPEdit teaser"></div>
    <div class="pub-info">
      <div class="pub-venue">COLM 2026</div>
      <div class="pub-title">
        <a href="https://arxiv.org/abs/2508.02092" target="_blank">
          FPEdit: Robust LLM Fingerprinting through Localized Parameter Editing
        </a>
      </div>
      <div class="pub-authors">
        <span class="me">Shida Wang</span>, Chaohu Liu, Yubo Wang, Linli Xu
      </div>
      <div class="pub-tldr">Knowledge-editing injects robust natural-language fingerprints into LLMs in under 2 minutes.</div>
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

</div>

<!-- ═══════════════ INTERNSHIPS ═══════════════ -->
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

<!-- ═══════════════ EDUCATION ═══════════════ -->
<div class="section-header"><h2>Education</h2></div>
<div class="tl">
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">Sept. 2024 – Present</div>
      <div class="tl-role">M.S. in Artificial Intelligence</div>
      <div class="tl-org"><a href="https://www.ustc.edu.cn/" target="_blank">USTC</a> · School of Artificial Intelligence and Data Science, Hefei</div>
    </div>
  </div>
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">Sept. 2021 – July 2024</div>
      <div class="tl-role">B.S. in Artificial Intelligence</div>
      <div class="tl-org"><a href="https://www.ustc.edu.cn/" target="_blank">USTC</a> · School of Artificial Intelligence and Data Science, Hefei</div>
    </div>
  </div>
  <div class="tl-item">
    <div class="tl-rail"><div class="tl-dot"></div><div class="tl-line"></div></div>
    <div class="tl-body">
      <div class="tl-period">Sept. 2020 – July 2021</div>
      <div class="tl-role">B.S. in Management (transferred)</div>
      <div class="tl-org"><a href="https://www.ustc.edu.cn/" target="_blank">USTC</a> · School of Management, Hefei</div>
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
