---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Jun Xia is currently at the Hong Kong University of Science and Technology and the ACCESS Chip Center as a Postdoctoral Research Fellow, advised by Prof. Yuan Xie. He has been a Postdoctoral Research Associate at the University of Notre Dame since 2023 (advised by Prof. Yiyu Shi). He obtained his Ph.D. degree from East China Normal University in 2023 (advised by Prof. Mingsong Chen). He obtained his M.S. degree and B.S. degree from Jiangnan University (supervised by Prof. Zhilei Chai and Prof. Wei Yan from Peking University) and Hainan University in 2019 and 2016, respectively.

His research interests include Heterogeneous On-device Federated Learning and Trustworthy AI. 

---

# 📝 Selected Publications 

<style>
  /* 全局与色彩变量 */
  :root {
    --primary-color: #0366d6;
    --text-main: #24292f;
    --text-muted: #57606a;
    --bg-light: #f6f8fa;
    --border-color: #d0d7de;
    --card-bg: #ffffff;
    --badge-venue-bg: #ddf4ff;
    --badge-venue-text: #0969da;
    --badge-ccf-bg: #dafbe1;
    --badge-ccf-text: #1a7f37;
    --badge-ratio-bg: #fff8c5;
    --badge-ratio-text: #9a6700;
  }

  /* 标题样式 */
  h1, h2, h3 {
    color: var(--text-main);
    border-bottom: 2px solid var(--bg-light);
    padding-bottom: 8px;
    margin-top: 32px;
    font-weight: 600;
  }

  /* 论文卡片设计 */
  .paper-card {
    background: var(--card-bg);
    border: 1px solid var(--border-color);
    border-radius: 10px;
    padding: 20px;
    margin-bottom: 20px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.04);
    transition: all 0.3s ease;
  }
  .paper-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 15px rgba(0,0,0,0.08);
    border-color: #b0c4de;
  }

  /* 论文标题与作者 */
  .paper-title {
    font-size: 1.15em;
    font-weight: 600;
    margin-bottom: 8px;
    line-height: 1.4;
  }
  .paper-title a {
    color: var(--primary-color);
    text-decoration: none;
  }
  .paper-title a:hover {
    text-decoration: underline;
  }
  .paper-authors {
    font-size: 0.95em;
    color: var(--text-main);
    margin-bottom: 12px;
  }
  .paper-authors b {
    color: #000;
    font-weight: 700;
    background-color: #fffbdd; /* 微微高亮自己的名字 */
    padding: 0 4px;
    border-radius: 3px;
  }

  /* 徽章样式 */
.custom-badge-group {
    margin-bottom: 12px;
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    align-items: center;
  }
  .custom-badge {
    display: inline-block;
    padding: 3px 10px;
    border-radius: 12px;
    font-size: 0.85em;
    font-weight: 600;
  }
  /* 直接写入颜色，防止变量被模板覆盖 */
  .custom-badge-conf { background-color: #ddf4ff !important; color: #0969da !important; }
  .custom-badge-level { background-color: #dafbe1 !important; color: #1a7f37 !important; }
  .custom-badge-ratio { background-color: #fff8c5 !important; color: #9a6700 !important; }
  
  .custom-paper-tagline {
    font-size: 0.9em;
    color: #57606a;
    font-style: italic;
  }

  /* 摘要与链接 */
  .paper-abstract {
    font-size: 0.9em;
    color: var(--text-muted);
    background: var(--bg-light);
    padding: 12px 16px;
    border-radius: 6px;
    border-left: 4px solid var(--primary-color);
    margin: 12px 0;
    line-height: 1.5;
  }
  .paper-links a {
    display: inline-block;
    font-size: 0.9em;
    color: var(--card-bg);
    background-color: var(--text-main);
    padding: 4px 12px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: 500;
    transition: background 0.2s;
  }
  .paper-links a:hover {
    background-color: var(--primary-color);
  }

  /* 列表与时间线样式 */
  .timeline-list {
    list-style-type: none;
    padding-left: 0;
  }
  .timeline-list li {
    margin-bottom: 12px;
    padding-left: 28px;
    position: relative;
    line-height: 1.6;
  }
  .timeline-list.news li::before { content: "🔥"; position: absolute; left: 0; top: 1px; }
  .timeline-list.awards li::before { content: "🏆"; position: absolute; left: 0; top: 1px; }
  .timeline-list.edu li::before { content: "🎓"; position: absolute; left: 0; top: 1px; }
  .timeline-list.talks li::before { content: "🎤"; position: absolute; left: 0; top: 1px; }
  .timeline-list.work li::before { content: "💼"; position: absolute; left: 0; top: 1px; }
  
  .date-tag {
    font-family: Monaco, Consolas, monospace;
    background: var(--bg-light);
    color: var(--text-muted);
    padding: 2px 6px;
    border-radius: 4px;
    font-size: 0.85em;
    margin-right: 8px;
    border: 1px solid var(--border-color);
  }
</style>

# 🔥 News
<ul class="timeline-list news">
  <li><span class="date-tag">2026.02</span> 🎉🎉 A paper accepted by DAC 2026.</li>
  <li><span class="date-tag">2026.02</span> 🎉🎉 Two papers accepted by CVPR 2026 (congratulations Boyu and Zixuan).</li>
  <li><span class="date-tag">2024.12</span> 🎉🎉 A paper accepted by T-SUSC 2024.</li>
  <li><span class="date-tag">2024.12</span> 🎉🎉 A paper accepted by DATE 2025.</li>
  <li><span class="date-tag">2024.09</span> 🎉🎉 A paper accepted by NeurIPS 2024.</li>
  <li><span class="date-tag">2024.07</span> 🎉🎉 A paper accepted by ICCAD 2024.</li>
  <li><span class="date-tag">2024.02</span> 🎉🎉 A paper accepted by DAC 2024.</li>
</ul>

---

# 📝 Selected Publications 

<div class="paper-card">
  <div class="paper-title">
    <a href="#">RTFL: Energy-Aware Federated Learning for AIoT Design Via Adaptive Quantization-based Multi-Agent Scheduling</a>
  </div>
  <div class="paper-authors">
    <b>Jun Xia</b>, Junqi Zhang, Zhaorong Zhu, Wenjie Chen, Mingsong Chen.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">DAC 2026</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 25%</span>
    <span class="custom-paper-tagline">Embedded System</span>
  </div>
  <div class="paper-abstract">
    We introduce RTFL, a novel energy-aware Real-Time Federated Learning framework based on Multi-Agent Reinforcement Learning (MARL), aiming to enhance the knowledge sharing across AIoT devices within a specified training time constraint. Specifically, RTFL employs an Adaptive Quantization-based Multi-Agent Scheduling (AQMAS) strategy, enabling a team of agents to intelligently select devices with specific model quantization levels for each round of local training, taking into account the resource constraints of the current devices.
  </div>
  <div class="paper-links">
    <a href="#">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="#">Fast3DGSW: Toward Fast and Robust Watermarking for Quantization-Aware 3D Gaussian Splatting</a>
  </div>
  <div class="paper-authors">
    Boyu Wang, <b>Jun Xia</b>, Mingsong Chen.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">CVPR 2026</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 25%</span>
    <span class="custom-paper-tagline">Computer Vision</span>
  </div>
  <div class="paper-links">
    <a href="#">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="https://arxiv.org/abs/2310.11595">WaveAttack: Asymmetric Frequency Obfuscation-based Backdoor Attacks Against Deep Neural Networks</a>
  </div>
  <div class="paper-authors">
    <b>Jun Xia</b>, Zhihao Yue, Yingbo Zhou, Zhiwei Ling, Yiyu Shi, Xian Wei, Mingsong Chen.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">NeurIPS 2024</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 25%</span>
    <span class="custom-paper-tagline">Machine Learning</span>
  </div>
  <div class="paper-abstract">
    We obtain image high-frequency features through the Discrete Wavelet Transform (DWT) to generate backdoor triggers.
  </div>
  <div class="paper-links">
    <a href="https://scholar.google.com/citations?view_op=view_citation&hl=en&user=K4JXEHUAAAAJ&sortby=pubdate&citation_for_view=K4JXEHUAAAAJ:0EnyYjriUFMC">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="https://arxiv.org/abs/2405.08183">Towards Energy-Aware Federated Learning via MARL: A Dual-Selection Approach for Model and Client</a>
  </div>
  <div class="paper-authors">
    <b>Jun Xia</b>, Yi Zhang, Yiyu Shi.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">ICCAD 2024</span>
    <span class="custom-badge custom-badge-level">CCF-B</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 24%</span>
    <span class="custom-paper-tagline">Embedded System / EDA</span>
  </div>
  <div class="paper-abstract">
    We propose an energy-aware FL framework named DR-FL, which considers the energy constraints in both clients and heterogeneous deep learning models to enable energy-efficient FL. Unlike Vanilla FL, DR-FL adopts our proposed Multi-Agent Reinforcement Learning (MARL)-based dual-selection method...
  </div>
  <div class="paper-links">
    <a href="https://scholar.google.com/citations?view_op=view_citation&hl=en&user=K4JXEHUAAAAJ&sortby=pubdate&citation_for_view=K4JXEHUAAAAJ:Wp0gIr-vW9MC">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="https://dl.acm.org/doi/10.1145/3489517.3530608">Enabling On-Device Large Language Model Personalization with Self-Supervised Data Selection and Synthesis</a>
  </div>
  <div class="paper-authors">
    Ruiyang Qin, <b>Jun Xia</b>, Zhenge Jia, Meng Jiang, Ahmed Abbasi, Peipei Zhou, Jingtong Hu, Yiyu Shi.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">DAC 2024</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 25%</span>
    <span class="custom-paper-tagline">Embedded System</span>
  </div>
  <div class="paper-abstract">
    In this paper, we propose a novel framework to select and store the most representative data online in a self-supervised way. Such data has a small memory footprint and allows infrequent requests of user annotations for further fine-tuning.
  </div>
  <div class="paper-links">
    <a href="https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=K4JXEHUAAAAJ&sortby=pubdate&authuser=2&citation_for_view=K4JXEHUAAAAJ:Zph67rFs4hoC">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="https://arxiv.org/pdf/2204.09975">Eliminating Backdoor Triggers for Deep Neural Networks Using Attention Relation Graph Distillation</a>
  </div>
  <div class="paper-authors">
    <b>Jun Xia</b>, Ting Wang, Jiepin Ding, Xian Wei, Mingsong Chen.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">IJCAI 2022</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 14%</span>
    <span class="custom-paper-tagline">Artificial Intelligence</span>
  </div>
  <div class="paper-abstract">
    We introduce a novel backdoor defense framework named Attention Relation Graph Distillation (ARGD), which fully explores the correlation among attention features with different orders using our proposed Attention Relation Graphs (ARGs).
  </div>
  <div class="paper-links">
    <a href="https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="https://dl.acm.org/doi/10.1145/3489517.3530608">Accelerated Synthesis of Neural Network-based Barrier Certificates Using Collaborative Learning</a>
  </div>
  <div class="paper-authors">
    <b>Jun Xia</b>, Ming Hu, Xin Chen, Mingsong Chen.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">DAC 2022</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 23%</span>
    <span class="custom-paper-tagline">Embedded System</span>
  </div>
  <div class="paper-abstract">
    We fully exploit the parallel processing capability of the underlying hardware to enable a quick search for a barrier certificate.
  </div>
  <div class="paper-links">
    <a href="https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="https://dl.acm.org/doi/10.1145/3489517.3530608">PervasiveFL: Pervasive Federated Learning for Heterogeneous IoT Systems</a>
  </div>
  <div class="paper-authors">
    <b>Jun Xia</b>, Tian Liu, Zhiwei Ling, Ting Wang, Xin Fu, Mingsong Chen.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">TCAD 2022</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 23%</span>
    <span class="custom-paper-tagline">Embedded System Journal</span>
  </div>
  <div class="paper-abstract">
    We propose a novel framework named PervasiveFL that enables efficient and effective FL among heterogeneous IoT devices. Without modifying original local models, PervasiveFL installs one lightweight NN model named modellet on each device.
  </div>
  <div class="paper-links">
    <a href="https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC">Project</a>
  </div>
</div>

<div class="paper-card">
  <div class="paper-title">
    <a href="https://dl.acm.org/doi/10.1145/3489517.3530608">Model-Contrastive Learning for Backdoor Elimination</a>
  </div>
  <div class="paper-authors">
    Zhihao Yue, <b>Jun Xia</b>, Zhiwei Ling, Ming Hu, Ting Wang, Xian Wei, Mingsong Chen.
  </div>
  <div class="custom-badge-group">
    <span class="custom-badge custom-badge-conf">ACM MM 2022</span>
    <span class="custom-badge custom-badge-level">CCF-A</span>
    <span class="custom-badge custom-badge-ratio">Acceptance Ratio: 25%</span>
    <span class="custom-paper-tagline">Multi-Media</span>
  </div>
  <div class="paper-abstract">
    In this paper, we propose a novel two-stage backdoor defense method, named MCLDef, based on Model-Contrastive Learning (MCL). MCLDef can purify the backdoored model by pulling the feature representations of poisoned data towards those of their clean data counterparts.
  </div>
  <div class="paper-links">
    <a href="https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC">Project</a>
  </div>
</div>

---

# 📖 Educations
<ul class="timeline-list edu">
  <li><span class="date-tag">2023.09 - 2026.05</span> <b>Postdoc</b>, University of Notre Dame, Department of CSE. <i>Advisor: Prof. Yiyu Shi.</i></li>
  <li><span class="date-tag">2019.09 - 2023.06</span> <b>PhD</b>, East China Normal University, Department of Software Engineering (A-level subject rating). <i>Supervisor: Prof. Mingsong Chen.</i></li>
  <li><span class="date-tag">2016.09 - 2019.06</span> <b>Master</b>, Jiangnan University, Department of Internet of Things, Computer Science. <i>Supervisor: Prof. Zhilei Chai.</i></li>
</ul>

# 🎖 Honors and Awards
<ul class="timeline-list awards">
  <li><span class="date-tag">2024.12</span> The National Artificial Intelligence Research Resource (NAIRR) Pilot Award (PI; First Year; Cash Equivalent <b>$98,400</b>; Hope to see you in Washington, 2025.2.19 - 2.21).</li>
  <li><span class="date-tag">2023.03</span> China National Scholarship ($4280)</li>
  <li><span class="date-tag">2023.06</span> Shanghai Outstanding Graduates</li>
  <li><span class="date-tag">2022.06</span> PhD Outstanding Program (ECNU) PI ($4280)</li>
  <li><span class="date-tag">2021.06</span> Outstanding Student (ECNU)</li>
</ul>

# 💻 Research Internships
<ul class="timeline-list work">
  <li><span class="date-tag">2016.12 - 2019.06</span> <b>Peking University</b>, <i>Supervisor: Prof. Wei Yan.</i></li>
</ul>

# 💬 Invited Talks & Services
<ul class="timeline-list talks">
  <li><span class="date-tag">2026.03</span> Invited Talk at Shandong University.</li>
  <li><span class="date-tag">2024.10</span> ICCAD 2024 Session Chair.</li>
  <li><span class="date-tag">2022.12</span> Invited Talk at East China Normal University.</li>
</ul>

# 📖 Teachings
<ul class="timeline-list edu">
  <li><span class="date-tag">2025 Spring</span> <b>Official Instructor</b> (Experimental Part), CSE 60685, University of Notre Dame.</li>
  <li><span class="date-tag">2024 Spring</span> <b>Teaching Assistant</b>, CSE 60685, University of Notre Dame.</li>
</ul>

> *His research interests include Heterogeneous On-device Federated Learning and Trustworthy AI.*

# 📖 Reviews and PC Members
*(Content to be added)*
