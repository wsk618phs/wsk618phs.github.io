---
layout: archive
title: "OSI-Lab: Organization of Science and Innovation Lab"
permalink: /lab/
author_profile: true
---

OSI-Lab is a computational social science lab at the Graduate School of Science and Technology Policy, KAIST, studying how science works: how research teams organize and divide labor, how AI is reshaping scientific work, and how science informs policy and innovation. We build large-scale data pipelines over millions of publications, patents, and policy documents — combining bibliometrics, natural language processing, LLM-based information extraction, and causal inference — on our in-house computing infrastructure.

Our research spans the science of science, science–policy interactions, and the governance of emerging technologies. Ongoing projects are listed below, alongside longer-running interests in research misconduct and retraction, mentoring and the reproduction of scientists, and scientific careers and mobility.

Data & Computing
======

The lab runs its analyses on a dedicated in-house Linux server with multi-terabyte storage, hosting web-scale research corpora — OpenAlex, SciSciNet, PubMed Central Open Access full text (millions of biomedical papers), Overton policy documents, Retraction Watch, and multinational patent databases. Our workflows combine Python-based data engineering, transformer embeddings (SciBERT, SPECTER2, patent-specific models), and batched large-language-model APIs for structured information extraction, together with reproducible Jupyter analysis pipelines and econometric identification (fixed effects, difference-in-differences, mixed models).

Projects in Progress
======

<style>
.proj-fig { max-width: 100%; border: 1px solid #eee; border-radius: 4px; margin: 0.6em 0 2em; display: block; }
</style>

**AI and the Division of Labor in Science.** How is generative AI reshaping the organization of scientific work? We parse author contribution statements from 2.6 million PubMed Central full-text papers into author–task matrices, measure paper-level LLM use, and combine within-author fixed effects with staggered difference-in-differences designs around the release of ChatGPT. LLM use is followed by a higher division of labor: writing becomes more broadly shared while data collection and analysis grow more concentrated.

<img class="proj-fig" src="/images/lab/projects/ai_dol.png" alt="Scaling of task contributors with team size">

**What Makes Policy Ideas Spread.** Using 9.1 million policy documents from Overton, we build a population-based account of policy issue diffusion across 16 science-and-technology domains. Modeling an issue's continued circulation in discourse — not just its adoption — we find that an idea's embeddedness in an established structure of meaning matters more than the prominence of the organizations carrying it.

<img class="proj-fig" src="/images/lab/projects/policy_diffusion.png" alt="Within-domain coefficients by domain growth rate">

**The Science–Policy Dual Frontier.** Linking 3.2 million Overton policy documents with 89.8 million scientific papers, we assign every document its minimum citation distance to the science–policy boundary. The connection is structurally asymmetric: policy documents that draw on science mostly cite it directly, while on the science side indirect connections dominate — and proximity to the boundary predicts impact only in the science domain.

<img class="proj-fig" src="/images/lab/projects/dual_frontier.png" alt="Citation distance to the science–policy boundary">

**How Scientific Knowledge Is Consumed.** Embedding the citation contexts of 37,401 highly cited papers (15.1 million citing papers) with sentence transformers, we map knowledge consumption along two dimensions — semantic similarity and audience diversity — and trace how external events such as Nobel Prizes and retractions systematically reshape a paper's position in this space.

<img class="proj-fig" src="/images/lab/projects/knowledge_consumption.png" alt="Knowledge-consumption space of highly cited papers">

**Mapping the Export-Control Frontier of Innovation.** We transform multilateral export-control lists (Wassenaar, NSG, MTCR, Australia Group, CWC) into 2,619 machine-readable decision units and adjudicate them against 8.2 million U.S. patents using embedding-based retrieval and LLM claim-level judgment, locating where export-controlled technologies sit in the patent technology space and who owns them.

<img class="proj-fig" src="/images/lab/projects/export_control.png" alt="Export-control adjudication outcomes in patent technology space">

**Commercial Potential and International Research Collaboration.** Linking 21,880 projects from Korean government-funded research institutes to their publications in OpenAlex, we show that projects with higher commercial potential are systematically less likely to involve international collaboration — a tension between commercialization and open science that varies across research fields.

<img class="proj-fig" src="/images/lab/projects/intl_collab.png" alt="Patent orientation and international research collaboration">

People
======

<style>
.lab-people { display: flex; flex-direction: column; gap: 1.2em; margin-bottom: 1.5em; }
.lab-person { display: flex; align-items: flex-start; gap: 1.4em; border: 1px solid #e2e2e2; border-radius: 8px; padding: 1.2em; }
.lab-person img { width: 130px; height: 160px; object-fit: cover; border-radius: 4px; flex-shrink: 0; }
.lab-person .name { font-weight: bold; font-size: 1.15em; }
.lab-person .role { color: #666; margin-bottom: 0.5em; }
.lab-person .tags { margin-bottom: 0.6em; }
.lab-person .tag { display: inline-block; background: #f2f2f2; color: #555; border-radius: 4px; padding: 0.1em 0.6em; margin: 0 0.3em 0.3em 0; font-size: 0.8em; }
.lab-person .bio { font-size: 0.9em; line-height: 1.55; }
.lab-person .links { margin-top: 0.5em; font-size: 0.85em; }
.lab-person .links a { margin-right: 0.8em; }
@media (max-width: 600px) { .lab-person { flex-direction: column; } }
</style>

<div class="lab-people">
  <div class="lab-person">
    <img src="/images/photo_woo.jpg" alt="Seokkyun Woo">
    <div>
      <div class="name">Seokkyun Woo</div>
      <div class="role">Assistant Professor</div>
      <div class="tags"><span class="tag">Science of Science</span><span class="tag">Division of Labor in Research</span><span class="tag">AI and Scientific Work</span></div>
      <div class="bio">Seokkyun studies the social and organizational structure of science — the division of labor in research teams, mentoring and scientific careers, and the evolving role of AI in scientific production — combining large-scale bibliometric data with computational text and network analysis.</div>
      <div class="links"><a href="https://stp.kaist.ac.kr/FacultyFull_time_Professor/view/id/90">STP Profile</a><a href="/">Website</a></div>
    </div>
  </div>
  <div class="lab-person">
    <img src="/images/lab/seohyeon_park.jpg" alt="Seohyeon Park">
    <div>
      <div class="name">Seohyeon Park</div>
      <div class="role">PhD Student</div>
      <div class="tags"><span class="tag">S&amp;T Governance</span><span class="tag">Scientific Community</span><span class="tag">Public Understanding of S&amp;T</span></div>
      <div class="bio">Seohyeon holds Bachelor's and Master's degrees in Economics and explores how stakeholders within the science and technology ecosystem coordinate and evolve their roles through conflict and cooperation, and how R&amp;D agendas, objectives, and impact assessment emerge from these processes.</div>
      <div class="links"><a href="https://stp.kaist.ac.kr/ph_d_students">STP Profile</a></div>
    </div>
  </div>
  <div class="lab-person">
    <img src="/images/lab/moonyul_yang.jpg" alt="Moonyul Yang">
    <div>
      <div class="name">Moonyul Yang</div>
      <div class="role">PhD Student</div>
      <div class="tags"><span class="tag">Technology–Security Nexus</span><span class="tag">Dual-Use Technology</span><span class="tag">Export Controls</span><span class="tag">Defense-Industry Innovation</span><span class="tag">Geopolitical Knowledge Flows</span></div>
      <div class="bio">Moonyul's research examines the intersection of technology and security. It focuses on how dual-use technologies are defined, measured, and governed, as well as how export-control regimes and geopolitical relations shape their development and diffusion. Combining patent and citation data with computational text analysis, embedding-based retrieval, and LLM-assisted classification, he analyzes these processes across patents, firms, and countries — from defense-industry innovation to cross-national knowledge flows.</div>
      <div class="links"><a href="https://stp.kaist.ac.kr/ph_d_students">STP Profile</a></div>
    </div>
  </div>
  <div class="lab-person">
    <img src="/images/lab/seungchan_choi.png" alt="SeungChan Choi">
    <div>
      <div class="name">SeungChan Choi</div>
      <div class="role">PhD Student</div>
      <div class="tags"><span class="tag">Social Infrastructure</span><span class="tag">Geopolitics</span><span class="tag">Network Development</span></div>
      <div class="bio">SeungChan aims to understand social infrastructure as a new artificial geopolitical element, with a focus on network and communication infrastructure — including the history of the Internet's development in Korea — and the roles that companies and states play in building it.</div>
      <div class="links"><a href="https://stp.kaist.ac.kr/ph_d_students">STP Profile</a></div>
    </div>
  </div>
  <div class="lab-person">
    <img src="/images/lab/jeonghyun_seo.jpg" alt="Jeonghyun Seo">
    <div>
      <div class="name">Jeonghyun Seo</div>
      <div class="role">Integrated MS–PhD Student</div>
      <div class="tags"><span class="tag">Scientific Organizations</span><span class="tag">Science of Science</span></div>
      <div class="bio">Jeonghyun majored in Physics and developed an interest in scientific organizations and the behavior of scientists while working in laboratories. She analyzes competition and collaboration among scientists and explores ways to promote a better environment for cooperation.</div>
      <div class="links"><a href="https://stp.kaist.ac.kr/masters_students">STP Profile</a></div>
    </div>
  </div>
  <div class="lab-person">
    <img src="/images/lab/doah_kwak.jpg" alt="Doah Kwak">
    <div>
      <div class="name">Doah Kwak</div>
      <div class="role">MS Student</div>
      <div class="tags"><span class="tag">Digital Gap</span><span class="tag">ICT Governance</span><span class="tag">AI Ethics</span></div>
      <div class="bio">Doah studied Spanish and AI Convergence and developed an interest in global ICT governance, digital inequality, and AI ethics while interning at CITEL (OAS). She explores how international ICT governance frameworks are formed and how ICT and AI can be used in more inclusive and sustainable ways.</div>
      <div class="links"><a href="https://stp.kaist.ac.kr/masters_students">STP Profile</a></div>
    </div>
  </div>
  <div class="lab-person">
    <img src="/images/lab/hyeree_kim.jpg" alt="Hyeree Kim">
    <div>
      <div class="name">Hyeree Kim</div>
      <div class="role">MS Student</div>
      <div class="tags"><span class="tag">Science of Science</span><span class="tag">Science and Technology Policy</span><span class="tag">Knowledge Production</span></div>
      <div class="bio">Hyeree is interested in computational approaches to understanding scientific knowledge production. Her research explores how scientific knowledge is shaped by both epistemic processes and broader social systems, with the goal of contributing to science and technology policy.</div>
      <div class="links"><a href="https://stp.kaist.ac.kr/masters_students">STP Profile</a></div>
    </div>
  </div>
</div>

Join Us
======

We are accepting applications for graduate students interested in the science of science, computational social science, and science & technology policy. Strong candidates typically have (or are eager to build) skills in Python, data analysis, and working with large datasets. Contact: wsk618 [at] kaist.ac.kr.
