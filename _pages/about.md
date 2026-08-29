---
permalink: /
layout: academic
title: ""
description: "Mengyu Yao is a Ph.D. student at Peking University researching security and privacy in AI systems."
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<section class="academic-intro" id="about-me" aria-labelledby="profile-name">
  <div class="academic-intro__copy">
    <h1 id="profile-name">Mengyu Yao</h1>
    <p>I am a Ph.D. student in Computer Science at <strong>Peking University</strong>, advised by Prof. Yao Guo. I am a member of the <a href="https://cs.pku.edu.cn/info/1166/1849.htm" target="_blank" rel="noopener noreferrer"><strong>Key Laboratory of High Confidence Software Technologies, Ministry of Education</strong></a> and expect to graduate in 2028.</p>
    <p>Before joining PKU, I received my B.S. in Computer Science and Technology from <strong>Nanjing University</strong> in 2023.</p>
    <nav class="academic-intro__links" aria-label="Contact and academic profiles">
      <a href="mailto:{{ site.author.email }}">Email</a><span aria-hidden="true">|</span>
      <a href="https://github.com/{{ site.author.github }}" target="_blank" rel="noopener noreferrer">GitHub</a><span aria-hidden="true">|</span>
      <a href="{{ site.author.googlescholar }}" target="_blank" rel="noopener noreferrer">Google Scholar</a>
    </nav>
  </div>
  <figure class="academic-intro__portrait">
    <img src="{{ site.author.avatar | relative_url }}" width="1589" height="1589" alt="Portrait of Mengyu Yao">
  </figure>
</section>

<h2 class="research-heading section-heading" id="research"><i class="fas fa-microscope section-heading__icon" aria-hidden="true"></i><span>Research <span class="research-heading__scholar">[<a href="{{ site.author.googlescholar }}" target="_blank" rel="noopener noreferrer">Google Scholar</a>]</span></span></h2>

<p class="research-intro">My research interests lie in <strong>security and privacy in AI systems</strong>, particularly retrieval-augmented generation, multimodal recommender systems, and AI agents.</p>

<article class="publication">
  <a class="publication__media" href="https://www.usenix.org/conference/usenixsecurity26/presentation/yao-dots" target="_blank" rel="noopener noreferrer" aria-label="Open Connect the Dots paper">
    <img src="{{ '/paper_figs/ragcrawler.png' | relative_url }}" width="528" height="438" loading="lazy" alt="RAGCrawler framework for knowledge-graph-guided query generation">
  </a>
  <div class="publication__body">
    <h3><a href="https://www.usenix.org/conference/usenixsecurity26/presentation/yao-dots" target="_blank" rel="noopener noreferrer">Connect the Dots: Knowledge Graph-Guided Crawler Attack on Retrieval-Augmented Generation Systems</a></h3>
    <p class="publication__authors"><strong>Mengyu Yao</strong>, Ziqi Zhang, Ning Luo, Shaofei Li, Yifeng Cai, Xiangqun Chen, Yao Guo, and Ding Li.</p>
    <p class="publication__venue"><em>35th USENIX Security Symposium, 2026</em> <span class="publication__note">(Long Presentation)</span></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media" href="https://www.usenix.org/conference/usenixsecurity26/presentation/yao-zero" target="_blank" rel="noopener noreferrer" aria-label="Open From Zero to Hero paper">
    <img src="{{ '/paper_figs/mrs.png' | relative_url }}" width="1380" height="596" loading="lazy" alt="CREAM framework for cross-modal adversarial item promotion">
  </a>
  <div class="publication__body">
    <h3><a href="https://www.usenix.org/conference/usenixsecurity26/presentation/yao-zero" target="_blank" rel="noopener noreferrer">From Zero to Hero: Cross-modal-enhanced Adversarial Item Promotion Attack against Multimodal Recommender Systems</a></h3>
    <p class="publication__authors"><strong>Mengyu Yao</strong>, Ziqi Zhang, Yifeng Cai, Junlin Liu, Xinyi Fu, Weiqiang Wang, Xiangqun Chen, Yao Guo, and Ding Li.</p>
    <p class="publication__venue"><em>35th USENIX Security Symposium, 2026</em> <span class="publication__note">(Long Presentation)</span></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media" href="https://doi.org/10.1145/3820771" target="_blank" rel="noopener noreferrer" aria-label="Open PredComp paper">
    <img src="{{ '/paper_figs/predcomp.png' | relative_url }}" width="1312" height="436" loading="lazy" alt="PredComp training and prediction pipeline">
  </a>
  <div class="publication__body">
    <h3><a href="https://doi.org/10.1145/3820771" target="_blank" rel="noopener noreferrer">PredComp: Predicting Compiler Optimization Options with Multi-stage Learning</a></h3>
    <p class="publication__authors">Bingyu Gao, Ziming Wang, <strong>Mengyu Yao</strong>, Zhihong Xue, Xiangqun Chen, Ding Li, and Yao Guo.</p>
    <p class="publication__venue"><em>ACM Transactions on Architecture and Code Optimization (TACO), 2026</em></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media" href="https://www.usenix.org/conference/usenixsecurity25/presentation/cai-yifeng" target="_blank" rel="noopener noreferrer" aria-label="Open I Can Tell Your Secrets paper">
    <img src="{{ '/paper_figs/theft.png' | relative_url }}" width="1634" height="588" loading="lazy" alt="Attack-model training, confidence calibration, and online privacy inference workflow">
  </a>
  <div class="publication__body">
    <h3><a href="https://www.usenix.org/conference/usenixsecurity25/presentation/cai-yifeng" target="_blank" rel="noopener noreferrer">I Can Tell Your Secrets: Inferring Privacy Attributes from Mini-app Interaction History in Super-apps</a></h3>
    <p class="publication__authors">Yifeng Cai, Ziqi Zhang, <strong>Mengyu Yao</strong>, Junlin Liu, Xiaoke Zhao, Xinyi Fu, Ruoyu Li, Zhe Li, Xiangqun Chen, Yao Guo, and Ding Li.</p>
    <p class="publication__venue"><em>34th USENIX Security Symposium, 2025</em></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media" href="https://doi.org/10.1145/3735452.3735530" target="_blank" rel="noopener noreferrer" aria-label="Open GroupTuner paper">
    <img src="{{ '/paper_figs/grouptuner.png' | relative_url }}" width="1060" height="382" loading="lazy" alt="GroupTuner option grouping and group-aware iterative search workflow">
  </a>
  <div class="publication__body">
    <h3><a href="https://doi.org/10.1145/3735452.3735530" target="_blank" rel="noopener noreferrer">GroupTuner: Efficient Group-Aware Compiler Auto-tuning</a></h3>
    <p class="publication__authors">Bingyu Gao, <strong>Mengyu Yao</strong>, Ziming Wang, Dong Liu, Ding Li, Xiangqun Chen, and Yao Guo.</p>
    <p class="publication__venue"><em>ACM SIGPLAN/SIGBED International Conference on Languages, Compilers, and Tools for Embedded Systems (LCTES), 2025</em></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media" href="https://doi.org/10.1145/3721126" target="_blank" rel="noopener noreferrer" aria-label="Open Not All Exceptions Are Created Equal paper">
    <img src="{{ '/paper_figs/exception.png' | relative_url }}" width="1308" height="602" loading="lazy" alt="ABEL architecture for triaging exception logs">
  </a>
  <div class="publication__body">
    <h3><a href="https://doi.org/10.1145/3721126" target="_blank" rel="noopener noreferrer">Not All Exceptions Are Created Equal: Triaging Error Logs in Real-World Enterprises</a></h3>
    <p class="publication__authors">Junlin Liu, <strong>Mengyu Yao</strong>, Shaofei Li, Dingyu Yang, Zheshun Wu, Xiaojun Qu, Ziqi Zhang, Ding Li, Yao Guo, and Xiangqun Chen.</p>
    <p class="publication__venue"><em>ACM Transactions on Software Engineering and Methodology (TOSEM), 2025</em></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media" href="https://doi.org/10.1145/3707453" target="_blank" rel="noopener noreferrer" aria-label="Open TEESlice paper">
    <img src="{{ '/paper_figs/teeslice.png' | relative_url }}" width="900" height="470" loading="lazy" alt="Comparison of existing TSDP solutions and TEESlice partition-before-training">
  </a>
  <div class="publication__body">
    <h3><a href="https://doi.org/10.1145/3707453" target="_blank" rel="noopener noreferrer">TEESlice: Protecting Sensitive Neural Network Models in Trusted Execution Environments when Attackers Have Pre-Trained Models</a></h3>
    <p class="publication__authors">Ding Li, Ziqi Zhang, <strong>Mengyu Yao</strong>, Yifeng Cai, Yao Guo, and Xiangqun Chen.</p>
    <p class="publication__venue"><em>ACM Transactions on Software Engineering and Methodology (TOSEM), 2025</em></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media" href="https://arxiv.org/abs/2510.26212" target="_blank" rel="noopener noreferrer" aria-label="Open Who Grants the Agent Power paper">
    <img src="{{ '/paper_figs/agent_power.png' | relative_url }}" width="618" height="222" loading="lazy" alt="AgentSentry task-centric access-control architecture">
  </a>
  <div class="publication__body">
    <h3><a href="https://arxiv.org/abs/2510.26212" target="_blank" rel="noopener noreferrer">Who Grants the Agent Power? Defending Against Instruction Injection via Task-Centric Access Control</a></h3>
    <p class="publication__authors">Yifeng Cai, Ziming Wang, Zhaomeng Deng, <strong>Mengyu Yao</strong>, Junlin Liu, Yutao Hu, Ziqi Zhang, Yao Guo, and Ding Li.</p>
    <p class="publication__venue"><em>SaTS 2025 (Co-located with ACM CCS 2025)</em></p>
  </div>
</article>

<article class="publication">
  <a class="publication__media publication__media--paper" href="https://arxiv.org/abs/2510.26210" target="_blank" rel="noopener noreferrer" aria-label="Open Who Moved My Transaction paper">
    <img src="{{ '/paper_figs/transaction-paper.png' | relative_url }}" width="1100" height="1400" loading="lazy" alt="First-page preview of the Who Moved My Transaction paper">
  </a>
  <div class="publication__body">
    <h3><a href="https://arxiv.org/abs/2510.26210" target="_blank" rel="noopener noreferrer">Who Moved My Transaction? Uncovering Post-Transaction Auditability Vulnerabilities in Modern Super Apps</a></h3>
    <p class="publication__authors">Junlin Liu, Zhaomeng Deng, Ziming Wang, <strong>Mengyu Yao</strong>, Yifeng Cai, Yutao Hu, Ziqi Zhang, Yao Guo, and Ding Li.</p>
    <p class="publication__venue"><em>SaTS 2025 (Co-located with ACM CCS 2025)</em></p>
  </div>
</article>

<h2 class="section-heading" id="internship-experience"><i class="fas fa-briefcase section-heading__icon" aria-hidden="true"></i><span>Internship Experience</span></h2>

<div class="cv-entry">
  <div class="cv-entry__heading">
    <div><strong>Huawei Technologies</strong><span>2012 Laboratories</span></div>
    <span class="cv-entry__date">Aug 2025 – Jul 2026</span>
  </div>
  <p class="cv-entry__role">Research Intern</p>
  <p>Conducted research on the security and privacy of AI agents.</p>
</div>

<div class="cv-entry">
  <div class="cv-entry__heading">
    <div><strong>Ant Group</strong><span>Security &amp; Machine Intelligence</span></div>
    <span class="cv-entry__date">Aug 2024 – Jan 2025</span>
  </div>
  <p class="cv-entry__role">Research Intern</p>
  <p>Worked on model-cluster load optimization and the security of multimodal recommender systems. The latter resulted in the first-author paper <a href="https://www.usenix.org/conference/usenixsecurity26/presentation/yao-zero" target="_blank" rel="noopener noreferrer"><em>From Zero to Hero: Cross-modal-enhanced Adversarial Item Promotion Attack against Multimodal Recommender Systems</em></a> at USENIX Security 2026 (Long Presentation).</p>
</div>

<h2 class="section-heading" id="teaching-experience"><i class="fas fa-chalkboard-teacher section-heading__icon" aria-hidden="true"></i><span>Teaching Experience</span></h2>

<div class="cv-entry">
  <div class="cv-entry__heading">
    <div><strong>Teaching Assistant</strong><span>Introduction to Computing · Peking University</span></div>
    <span class="cv-entry__date">Fall 2024</span>
  </div>
</div>

<div class="cv-entry">
  <div class="cv-entry__heading">
    <div><strong>Teaching Assistant</strong><span>Problem Solving · Nanjing University</span></div>
    <span class="cv-entry__date">Fall 2021 – Spring 2023</span>
  </div>
</div>

<h2 class="section-heading" id="education"><i class="fas fa-graduation-cap section-heading__icon" aria-hidden="true"></i><span>Education</span></h2>

<div class="cv-entry">
  <div class="cv-entry__heading">
    <div><strong>Peking University</strong><span>School of Computer Science</span></div>
    <span class="cv-entry__date">Sep 2023 – Jun 2028 (Expected)</span>
  </div>
  <p class="cv-entry__role">Ph.D. in Computer Science (Computer Software and Theory)</p>
  <p>Advisor: Prof. Yao Guo</p>
</div>

<div class="cv-entry">
  <div class="cv-entry__heading">
    <div><strong>Nanjing University</strong><span>Department of Computer Science and Technology</span></div>
    <span class="cv-entry__date">Sep 2019 – Jun 2023</span>
  </div>
  <p class="cv-entry__role">B.S. in Computer Science and Technology, Top-notch Undergraduate Program</p>
  <p>GPA: 4.643 / 5.0 (Top 1%)</p>
</div>

<h2 class="section-heading" id="honors-and-awards"><i class="fas fa-award section-heading__icon" aria-hidden="true"></i><span>Honors and Awards</span></h2>

<ul class="honors-list">
  <li><span>Peking University Outstanding Scientific Research Award</span><time datetime="2024-12">Dec 2024</time></li>
  <li><span>Canon Scholarship</span><time datetime="2024-12">Dec 2024</time></li>
  <li><span>Outstanding Graduate of Nanjing University</span><time datetime="2023-06">Jun 2023</time></li>
  <li><span>Special Scholarship for Basic Disciplines, Excellence Award</span><time datetime="2022-11">Nov 2022</time></li>
  <li><span>People's Scholarship</span><time datetime="2022-11">Nov 2022</time></li>
  <li><span>Special Scholarship for Basic Disciplines, Excellence Award</span><time datetime="2021-11">Nov 2021</time></li>
  <li><span>Top-notch Undergraduate Program Scholarship, First Prize</span><time datetime="2020-11">Nov 2020</time></li>
  <li><span>Outstanding Student, Nanjing University</span><time datetime="2020-11">Nov 2020</time></li>
</ul>
