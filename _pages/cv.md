---
layout: archive
title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
/* Clean, Fast, and Elegant CV Aesthetic without heavy scripts or renders */
:root {
  --primary: #3b82f6;
  --secondary: #6366f1;
  --bg-color: #ffffff;
  --card-bg: #f8fafc;
  --card-border: #e2e8f0;
  --text-main: #1e293b;
  --text-muted: #475569;
}

.clean-cv {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  color: var(--text-main);
  background: var(--bg-color);
  line-height: 1.6;
}

.cv-header {
  text-align: center;
  margin-bottom: 3rem;
  padding-bottom: 2rem;
  border-bottom: 1px solid var(--card-border);
}

.cv-header h1 {
  font-size: 2.25rem;
  font-weight: 700;
  color: var(--text-main);
  margin-bottom: 0.5rem;
}

.cv-header p {
  font-size: 1.1rem;
  color: var(--text-muted);
}

.section-title {
  font-size: 1.4rem;
  font-weight: 700;
  color: var(--text-main);
  margin-top: 2.5rem;
  margin-bottom: 1.5rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid var(--primary);
  display: inline-block;
}

.cv-item {
  background: var(--card-bg);
  border: 1px solid var(--card-border);
  border-radius: 8px;
  padding: 1.5rem;
  margin-bottom: 1.5rem;
}

.item-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 1rem;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.item-title {
  font-size: 1.2rem;
  font-weight: 600;
  margin: 0;
  color: var(--text-main);
}

.item-subtitle {
  font-size: 1rem;
  color: var(--text-muted);
  margin: 0.25rem 0 0 0;
  font-weight: 500;
}

.item-date {
  font-size: 0.9rem;
  font-weight: 600;
  color: var(--secondary);
}

.badge {
  display: inline-block;
  font-size: 0.8rem;
  font-weight: 600;
  background: #e0e7ff;
  color: #3730a3;
  padding: 0.2rem 0.6rem;
  border-radius: 4px;
  margin-bottom: 0.5rem;
  text-transform: uppercase;
}

.badge-success {
  background: #dcfce7;
  color: #166534;
}

.pub-list {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.pub-item {
  padding-bottom: 1.5rem;
  border-bottom: 1px solid var(--card-border);
}

.pub-item:last-child {
  border-bottom: none;
  padding-bottom: 0;
}

.pub-title {
  font-weight: 600;
  font-size: 1.1rem;
  margin-bottom: 0.5rem;
  color: var(--text-main);
}

.pub-authors {
  color: var(--text-muted);
  font-size: 0.95rem;
  margin-bottom: 0.25rem;
}

.pub-authors strong {
  color: var(--primary);
}

.pub-venue {
  font-style: italic;
  color: var(--secondary);
  font-size: 0.95rem;
  margin-bottom: 0.75rem;
}

.btn-download {
  display: inline-block;
  background: #f1f5f9;
  color: var(--primary) !important;
  text-decoration: none;
  font-size: 0.85rem;
  padding: 0.3rem 0.8rem;
  border-radius: 4px;
  font-weight: 500;
  border: 1px solid #cbd5e1;
}

.btn-download:hover {
  background: var(--primary);
  color: #ffffff !important;
  border-color: var(--primary);
}

.awards-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.awards-list li {
  padding: 1rem;
  background: var(--card-bg);
  border: 1px solid var(--card-border);
  border-radius: 8px;
  margin-bottom: 1rem;
}

.awards-list h4 {
  margin: 0 0 0.25rem 0;
  font-size: 1.05rem;
  color: var(--text-main);
}

.awards-list p {
  margin: 0;
  font-size: 0.9rem;
  color: var(--text-muted);
}

.skills-list {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.skill-tag {
  background: var(--card-bg);
  border: 1px solid var(--card-border);
  padding: 0.4rem 0.8rem;
  border-radius: 6px;
  font-size: 0.9rem;
  color: var(--text-main);
}

.cv-item p {
  margin-bottom: 0.5rem;
}
</style>

<div class="clean-cv">
  
  <div class="cv-header">
    <h1>Curriculum Vitae</h1>
    <p>wjt99@mail.ustc.edu.cn &bull; Hefei, China</p>
    <div style="margin-top: 1rem;">
      <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Ftinklert.github.io%2Fcv&count_bg=%233b82f6&title_bg=%231e293b&icon=&icon_color=%23E7E7E7&title=Views&edge_flat=true"/></a>
    </div>
  </div>

  <div style="background: var(--card-bg); border-left: 4px solid var(--primary); padding: 1.5rem; margin-bottom: 1.5rem; border-radius: 0 8px 8px 0; font-size: 1.05rem; line-height: 1.6; color: var(--text-main); box-shadow: 0 1px 3px rgba(0,0,0,0.02);">
    Juntao Wu is a Ph.D. candidate at the School of Management, University of Science and Technology of China. He earned his B.S. degree with Hefei University of Technology and is working toward his Ph.D. degree with the University of Science and Technology of China. His research areas include information systems, omni-channel retail, consumer behavior analysis, and data mining applications, etc. He has published in leading international journals and conferences such as <em>Decision Support Systems</em>, <em>Information Processing & Management</em>, <em>Expert Systems with Applications</em>, <em>Computers & Industrial Engineering</em>, and <em>International Conference on Information Systems (ICIS)</em>, among others.
  </div>

  <div style="text-align: center; margin-bottom: 2.5rem; padding: 1rem 2rem; position: relative;">
    <span style="font-size: 3rem; color: #e2e8f0; position: absolute; left: 0; top: -10px; font-family: serif;">"</span>
    <p style="font-size: 1.15rem; color: #475569; font-style: italic; margin: 0; font-family: 'STKaiti', 'KaiTi', '楷体', serif; line-height: 1.8; letter-spacing: 1px;">
      天将降大任于是人也，必先苦其心志，劳其筋骨，饿其体肤，空乏其身，行拂乱其所为，所以动心忍性，曾益其所不能。
    </p>
    <span style="font-size: 3rem; color: #e2e8f0; position: absolute; right: 0; bottom: -30px; font-family: serif;">"</span>
  </div>

  <h2 class="section-title">Education</h2>
  <div>
    <div class="cv-item">
      <div class="item-header">
        <div>
          <h3 class="item-title">Management Science and Engineering (PhD)</h3>
          <p class="item-subtitle">University of Science and Technology of China (USTC)</p>
        </div>
        <span class="item-date">2023.09 - 2026.06 (Expected)</span>
      </div>
    </div>
    <div class="cv-item">
      <div class="item-header">
        <div>
          <h3 class="item-title">Management Science and Engineering (Master)</h3>
          <p class="item-subtitle">University of Science and Technology of China (USTC)</p>
        </div>
        <span class="item-date">2021.09 - 2023.06</span>
      </div>
    </div>
    <div class="cv-item">
      <div class="item-header">
        <div>
          <h3 class="item-title">Industrial Engineering (Bachelor)</h3>
          <p class="item-subtitle">Hefei University of Technology (HFUT)</p>
        </div>
        <span class="item-date">2016.09 - 2020.06</span>
      </div>
    </div>
  </div>

  <h2 class="section-title">Internship Experience</h2>
  <div class="cv-item">
    <div class="item-header">
      <div>
        <h3 class="item-title">Algorithm Engineer</h3>
        <p class="item-subtitle">Qimai Technology</p>
      </div>
      <span class="item-date">2024.06 - Present</span>
    </div>
  </div>
  <div class="cv-item">
    <div class="item-header">
      <div>
        <h3 class="item-title">Algorithm Development Intern</h3>
        <p class="item-subtitle">Home Original Chicken (Lao Xiang Ji)</p>
      </div>
      <span class="item-date">2023.04 - 2023.06</span>
    </div>
  </div>
  <div class="cv-item">
    <div class="item-header">
      <div>
        <h3 class="item-title">Quantitative Research Intern</h3>
        <p class="item-subtitle">Zhejiang Yingyang Asset</p>
      </div>
      <span class="item-date">2022.06 - 2023.03</span>
    </div>
  </div>

  <h2 class="section-title">Research Experience</h2>
  
  <div class="cv-item">
    <div class="item-header">
      <h3 class="item-title">Malicious Consumer Detection Algorithm Design</h3>
      <span class="item-date">2025.03 - 2025.08</span>
    </div>
    <span class="badge">Description</span>
    <p>Jointly modeled consumer cross-channel behavior and cognitive resource investment during fine-grained page browsing processes. Utilized Graph Neural Networks (GNN) to mine user IP address networks for detecting malicious consumers.</p>
    <span class="badge badge-success">Achievement</span>
    <p>The algorithm was applied in the internship company, serving a large listed tea beverage enterprise.</p>
  </div>

  <div class="cv-item">
    <div class="item-header">
      <h3 class="item-title">Consumer Marketing Response Prediction Based on Decoupled Attribution</h3>
      <span class="item-date">2024.04 - 2025.03</span>
    </div>
    <span class="badge">Description</span>
    <p>Decomposed consumer repurchase behavior into "inertia" and "marketing stimulus". Used Heterogeneous Graph Neural Networks (HGNN) to model long-term user inertia, and dynamic time-series models to capture marketing fatigue and immediate reactions. Employed a decoupled attention mechanism to attribute the deviation between prediction and reality for precise consumer response prediction.</p>
  </div>

  <div class="cv-item">
    <div class="item-header">
      <h3 class="item-title">Full-Store All-Product Sales Prediction Based on Consumer Preference Mining</h3>
      <span class="item-date">2023.05 - 2024.01</span>
    </div>
    <span class="badge">Description</span>
    <p>Adopted a two-stage deep learning approach. First, used Heterogeneous Graph Neural Networks to mine user groups with similar preferences. Then, utilized a consumer preference attention mechanism to fuse data for sales prediction.</p>
    <span class="badge badge-success">Achievement</span>
    <p>The algorithm was launched in the internship company, serving over a thousand stores.</p>
  </div>

  <div class="cv-item">
    <div class="item-header">
      <h3 class="item-title">Shared Mobility Demand Prediction Based on Graph Neural Networks</h3>
      <span class="item-date">2022.05 - 2023.03</span>
    </div>
    <span class="badge">Description</span>
    <p>Combined Graph Convolutional Networks (GCN) and Long Short-Term Memory (LSTM) networks to extract spatial location features and temporal demand information of shared bike stations, respectively, integrating multi-dimensional factors for demand prediction modeling.</p>
  </div>

  <div class="cv-item">
    <div class="item-header">
      <h3 class="item-title">Business Process Fraud Detection Based on Deep Learning</h3>
      <span class="item-date">2021.09 - 2022.05</span>
    </div>
    <span class="badge">Description</span>
    <p>Comprehensively analyzed employee transaction data, personal information, and reporting texts to extract multi-dimensional features and build a fraud detection algorithm. On a real-world dataset, the model achieved a recall rate of 92% and an AUC of 97%.</p>
  </div>

  <div class="cv-item">
    <div class="item-header">
      <h3 class="item-title">Road Pedestrian Detection System Design Based on Machine Vision</h3>
      <span class="item-date">2019.12 - 2020.06</span>
    </div>
    <p style="font-weight: 500; color: var(--text-muted); margin-top: -10px; margin-bottom: 10px;">Graduation Thesis</p>
    <span class="badge">Description</span>
    <p>Focused on road pedestrian detection scenarios, improved the traditional HOG feature detection method, integrated Gaussian Mixture Models (GMM) for foreground extraction and denoising, and combined with LBP features to enhance detection performance.</p>
    <span class="badge badge-success">Achievement</span>
    <p>The graduation design was awarded "2020 Hefei University of Technology Excellent Undergraduate Graduation Design".</p>
  </div>


  <h2 class="section-title">Publications</h2>
  <div class="pub-list">
    
    <div class="pub-item">
      <div class="pub-title">Dynamic hypergraph neural networks for consumer purchase path prediction: Integrating promotions, experiences, and store heterogeneity</div>
      <div class="pub-authors"><strong>J Wu</strong>, Q Liu, L Chen, W Zhao, H Liu</div>
      <div class="pub-venue">Decision Support Systems, 114614, 2026</div>
      <a href="https://doi.org/10.1016/j.dss.2026.114614" class="btn-download" target="_blank" rel="noopener noreferrer">Download PDF</a>
    </div>

    <div class="pub-item">
      <div class="pub-title">Incorporating worker rivalry into task recommendations on crowdsourcing platforms: A novel framework for boosting participation and efficiency</div>
      <div class="pub-authors">H Liu, W Li, M Chen, <strong>J Wu</strong></div>
      <div class="pub-venue">Information Processing & Management, 63 (1), 104310, 2026</div>
      <a href="https://doi.org/10.1016/j.ipm.2026.104310" class="btn-download" target="_blank" rel="noopener noreferrer">Download PDF</a>
    </div>

    <div class="pub-item">
      <div class="pub-title">Apppoet: Large language model based android malware detection via multi-view prompt engineering</div>
      <div class="pub-authors">W Zhao, <strong>J Wu</strong>, Z Meng</div>
      <div class="pub-venue">Expert Systems with Applications, 262, 125546, 2025</div>
      <a href="https://doi.org/10.1016/j.eswa.2025.125546" class="btn-download" target="_blank" rel="noopener noreferrer">Download PDF</a>
    </div>

    <div class="pub-item">
      <div class="pub-title">Demand prediction for bike-sharing systems: A spatial and semantic modeling approach for enhanced accuracy and operational efficiency</div>
      <div class="pub-authors"><strong>J Wu</strong>, J Feng, J Fang, H Liu</div>
      <div class="pub-venue">Computers & Industrial Engineering, 111775, 2025</div>
      <a href="https://doi.org/10.1016/j.cie.2025.111775" class="btn-download" target="_blank" rel="noopener noreferrer">Download PDF</a>
    </div>

    <div class="pub-item">
      <div class="pub-title">Beyond the Match: Predicting Bilateral-matching Satisfaction with Multi-view Heterogeneous Graph Neural Network</div>
      <div class="pub-authors">J Feng, H Liu, <strong>J Wu</strong>, H Liu, P Zhao</div>
      <div class="pub-venue">ICIS 2025 Proceedings</div>
      <a href="https://aisel.aisnet.org/icis2025/da_bus/da_bus/4/" class="btn-download" target="_blank" rel="noopener noreferrer">Download PDF</a>
    </div>

    <div class="pub-item">
      <div class="pub-title">Unveiling consumer preferences: A two-stage deep learning approach to enhance accuracy in multi-channel retail sales forecasting</div>
      <div class="pub-authors"><strong>J Wu</strong>, H Liu, X Yao, L Zhang</div>
      <div class="pub-venue">Expert Systems with Applications, 257, 125066, 2024</div>
      <a href="https://doi.org/10.1016/j.eswa.2024.125066" class="btn-download" target="_blank" rel="noopener noreferrer">Download PDF</a>
    </div>

    <div class="pub-item">
      <div class="pub-title">Optimizing Restaurant Customer Flow and Revenue with Real-Time Coupon Allocation: A Deep Reinforcement Learning Approach</div>
      <div class="pub-authors">J Feng, <strong>J Wu</strong>, M Chen, J Qin</div>
      <div class="pub-venue">ICIS 2024 Proceedings</div>
      <a href="https://aisel.aisnet.org/icis2024/data_soc/data_soc/9/" class="btn-download" target="_blank" rel="noopener noreferrer">Download PDF</a>
    </div>

  </div>

  <h2 class="section-title">Working Papers</h2>
  <div class="pub-list" style="margin-bottom: 2rem;">
    
    <div class="pub-item">
      <div class="pub-title">Bridging Spaces: A Spatio-Temporal Fusion Model for Dynamic Intra- and Inter-Brand Competition in Sales Forecasting</div>
      <div class="pub-authors"><strong>Juntao Wu</strong>, Qianzhou Du, Hefu Liu</div>
      <div class="pub-venue" style="margin-bottom: 0;">Working Paper</div>
    </div>

    <div class="pub-item">
      <div class="pub-title">Combating Organized Promotion Abuse in Omnichannel Commerce: An Information Foraging Perspective on Graph-Based Anomaly Detection</div>
      <div class="pub-authors"><strong>Juntao Wu</strong>, Hongfei Bao, Qian Huang, Hefu Liu</div>
      <div class="pub-venue" style="margin-bottom: 0;">Working Paper</div>
    </div>

    <div class="pub-item">
      <div class="pub-title">Habit from Hype: A Disentangled Graph-Temporal Framework for Modeling Consumer Marketing Response</div>
      <div class="pub-authors"><strong>Juntao Wu</strong>, Hefu Liu</div>
      <div class="pub-venue" style="margin-bottom: 0;">Working Paper</div>
    </div>

    <div class="pub-item">
      <div class="pub-title">DualDependency: Capturing Consumer Path and Motivation Dynamics in Multi-Task Repurchase Prediction</div>
      <div class="pub-authors"><strong>Juntao Wu</strong>, Hefu Liu</div>
      <div class="pub-venue" style="margin-bottom: 0;">Working Paper</div>
    </div>

    <div class="pub-item">
      <div class="pub-title">Beyond the Mean Field: A Coupled Neuro-Dynamics Framework for Coupon-Driven Sales Forecasting with Fluctuation Corrections</div>
      <div class="pub-authors"><strong>Juntao Wu</strong></div>
      <div class="pub-venue" style="margin-bottom: 0;">Working Paper</div>
    </div>

  </div>

  <h2 class="section-title">Awards</h2>
  <ul class="awards-list">
    <li>
      <h4>🏆 Outstanding Graduation Thesis</h4>
      <p>Hefei University of Technology • 2020.06</p>
    </li>
    <li>
      <h4>🥈 Silver Award, Creative Group</h4>
      <p>5th "Internet+" Innovation and Entrepreneurship Competition • 2019.08</p>
    </li>
    <li>
      <h4>🌟 University-level "Advanced Individual"</h4>
      <p>Student Work Department • 2018.01</p>
    </li>
    <li>
      <h4>🎖️ "Excellent Youth League Cadre"</h4>
      <p>"May Fourth" Evaluation • 2017.05</p>
    </li>
  </ul>

  <h2 class="section-title">Skills and Courses</h2>
  <div class="cv-item">
    <h3 style="font-size: 1.1rem; color: var(--text-main); margin-bottom: 0.8rem; margin-top: 0;">Core Courses & Knowledge</h3>
    <div class="skills-list">
      <span class="skill-tag">Operations Research</span>
      <span class="skill-tag">Machine Learning</span>
      <span class="skill-tag">Convex Optimization</span>
      <span class="skill-tag">Game Theory</span>
      <span class="skill-tag">Stochastic System Modeling</span>
      <span class="skill-tag">Simulation</span>
      <span class="skill-tag">Algorithm Design Science</span>
    </div>
    
    <h3 style="font-size: 1.1rem; color: var(--text-main); margin-bottom: 0.8rem;">Language Proficiency</h3>
    <div class="skills-list" style="margin-bottom: 0;">
      <span class="skill-tag" style="background: #eef2ff; color: #4338ca; border-color: #c7d2fe;">CET-6 (516)</span>
    </div>
  </div>

</div>
