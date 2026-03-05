---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
/* Modern CV Design Wrapper */
.modern-cv {
  font-family: 'Outfit', sans-serif;
  color: #334155;
  background: linear-gradient(135deg, #f8fafc 0%, #e2e8f0 100%);
  padding: 2.5rem;
  border-radius: 24px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.04);
  margin-top: -1rem;
}

.modern-cv h2 {
  font-size: 1.75rem;
  font-weight: 700;
  color: #0f172a;
  margin-bottom: 2rem;
  margin-top: 3rem;
  display: flex;
  align-items: center;
  gap: 0.75rem;
  position: relative;
  border-bottom: none;
}

.modern-cv h2::before {
  content: "";
  display: inline-block;
  width: 12px;
  height: 24px;
  background: linear-gradient(to right, #6366f1, #a855f7);
  border-radius: 4px;
}

.modern-cv p {
  line-height: 1.7;
  color: #475569;
  font-size: 1.05rem;
}

/* Glassmorphism Cards */
.cv-card {
  background: rgba(255, 255, 255, 0.7);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.5);
  border-radius: 16px;
  padding: 1.5rem 2rem;
  margin-bottom: 1.5rem;
  box-shadow: 0 4px 6px rgba(0,0,0,0.02);
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  overflow: hidden;
}

.cv-card::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: linear-gradient(90deg, #6366f1, #3b82f6, #a855f7);
  opacity: 0;
  transition: opacity 0.3s ease;
}

.cv-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 25px -5px rgba(0,0,0,0.1), 0 10px 10px -5px rgba(0,0,0,0.04);
  background: #ffffff;
}

.cv-card:hover::after {
  opacity: 1;
}

.card-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 1rem;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.card-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: #1e293b;
  margin: 0;
}

.card-subtitle {
  font-size: 1rem;
  color: #64748b;
  font-weight: 500;
  margin: 0;
}

.card-date {
  font-size: 0.9rem;
  font-weight: 600;
  color: #4f46e5;
  background: #e0e7ff;
  padding: 0.25rem 0.75rem;
  border-radius: 9999px;
  white-space: nowrap;
}

/* Timeline specific styles */
.timeline {
  position: relative;
  padding-left: 2rem;
  border-left: 2px dashed #cbd5e1;
  margin-left: 1rem;
}

.timeline .cv-card {
  margin-left: 0;
  width: calc(100% - 1rem);
}

.timeline::before {
  content: "";
  position: absolute;
  left: -7px;
  top: 0;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #6366f1;
  box-shadow: 0 0 0 4px #e0e7ff;
}

.timeline-item {
  position: relative;
}

.timeline-item::before {
  content: '';
  position: absolute;
  left: -2rem;
  top: 2rem;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #fff;
  border: 3px solid #6366f1;
  transform: translateX(-50%);
  z-index: 10;
}

/* Badges */
.badge {
  display: inline-block;
  font-size: 0.8rem;
  font-weight: 600;
  padding: 0.2rem 0.6rem;
  border-radius: 6px;
  margin-right: 0.5rem;
  margin-bottom: 0.5rem;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

.badge-info { background: #dbeafe; color: #1e40af; }
.badge-success { background: #dcfce7; color: #166534; }
.badge-purple { background: #f3e8ff; color: #6b21a8; }

/* Publications specific */
.pub-item {
  background: #fff;
  border-radius: 12px;
  padding: 1.25rem;
  margin-bottom: 1rem;
  border-left: 4px solid transparent;
  transition: all 0.3s;
  box-shadow: 0 2px 4px rgba(0,0,0,0.02);
}

.pub-item:hover {
  border-left-color: #8b5cf6;
  box-shadow: 0 10px 15px -3px rgba(0,0,0,0.05);
  transform: translateX(4px);
}

.pub-title {
  font-weight: 600;
  color: #0f172a;
  font-size: 1.1rem;
  margin-bottom: 0.5rem;
}

.pub-authors {
  color: #475569;
  font-size: 0.95rem;
  margin-bottom: 0.5rem;
}

.pub-venue {
  font-style: italic;
  color: #6366f1;
  font-size: 0.9rem;
}

.btn-download {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: linear-gradient(135deg, #6366f1, #8b5cf6);
  color: white !important;
  text-decoration: none;
  font-weight: 500;
  font-size: 0.85rem;
  padding: 0.4rem 1rem;
  border-radius: 9999px;
  margin-top: 0.5rem;
  box-shadow: 0 4px 6px -1px rgba(99, 102, 241, 0.4);
  transition: all 0.3s;
}

.btn-download:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 8px -1px rgba(99, 102, 241, 0.6);
  background: linear-gradient(135deg, #4f46e5, #7c3aed);
}

/* Skills/Tags */
.skills-container {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-top: 1rem;
}

.skill-tag {
  background: #f1f5f9;
  color: #334155;
  border: 1px solid #e2e8f0;
  padding: 0.4rem 1rem;
  border-radius: 999px;
  font-weight: 500;
  font-size: 0.9rem;
  transition: all 0.2s;
  cursor: default;
}

.skill-tag:hover {
  background: #3b82f6;
  color: white;
  border-color: #3b82f6;
  transform: translateY(-2px) scale(1.05);
}

/* Responsive */
@media (max-width: 768px) {
  .modern-cv {
    padding: 1.5rem;
  }
  .card-header {
    flex-direction: column;
  }
  .timeline {
    margin-left: 0;
    border-left: none;
    padding-left: 0;
  }
  .timeline-item::before {
    display: none;
  }
}
</style>

<div class="modern-cv">
  
  <div style="text-align: center; margin-bottom: 3rem;">
    <h1 style="font-size: 2.5rem; font-weight: 700; background: linear-gradient(to right, #2563eb, #9333ea); -webkit-background-clip: text; -webkit-text-fill-color: transparent; margin-bottom: 0.5rem; border: none;">Curriculum Vitae</h1>
    <p style="font-size: 1.1rem; color: #64748b; margin-top: 0;">wjt99@mail.ustc.edu.cn</p>
  </div>

  <h2>Education</h2>
  <div class="timeline">
    <div class="timeline-item">
      <div class="cv-card">
        <div class="card-header">
          <div>
            <h3 class="card-title">Management Science and Engineering (PhD)</h3>
            <p class="card-subtitle">University of Science and Technology of China (USTC)</p>
          </div>
          <span class="card-date">2023.09 - 2026.06 (Expected)</span>
        </div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="cv-card">
        <div class="card-header">
          <div>
            <h3 class="card-title">Management Science and Engineering (Master)</h3>
            <p class="card-subtitle">University of Science and Technology of China (USTC)</p>
          </div>
          <span class="card-date">2021.09 - 2023.06</span>
        </div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="cv-card">
        <div class="card-header">
          <div>
            <h3 class="card-title">Industrial Engineering (Bachelor)</h3>
            <p class="card-subtitle">Hefei University of Technology (HFUT)</p>
          </div>
          <span class="card-date">2016.09 - 2020.06</span>
        </div>
      </div>
    </div>
  </div>

  <h2>Internship Experience</h2>
  <div class="cv-card">
    <div class="card-header">
      <div>
        <h3 class="card-title">Algorithm Engineer</h3>
        <p class="card-subtitle">Qimai Technology</p>
      </div>
      <span class="card-date" style="background: #ecfdf5; color: #059669;">2024.06 - Present</span>
    </div>
  </div>
  <div class="cv-card">
    <div class="card-header">
      <div>
        <h3 class="card-title">Algorithm Development Intern</h3>
        <p class="card-subtitle">Home Original Chicken (Lao Xiang Ji)</p>
      </div>
      <span class="card-date">2023.04 - 2023.06</span>
    </div>
  </div>
  <div class="cv-card">
    <div class="card-header">
      <div>
        <h3 class="card-title">Quantitative Research Intern</h3>
        <p class="card-subtitle">Zhejiang Yingyang Asset</p>
      </div>
      <span class="card-date">2022.06 - 2023.03</span>
    </div>
  </div>

  <h2>Research Experience</h2>
  
  <div class="cv-card">
    <div class="card-header">
      <h3 class="card-title">Malicious Consumer Detection Algorithm Design</h3>
      <span class="card-date">2025.03 - 2025.08</span>
    </div>
    <p><span class="badge badge-info">Description</span> Jointly modeled consumer cross-channel behavior and cognitive resource investment during fine-grained page browsing processes. Utilized Graph Neural Networks (GNN) to mine user IP address networks for detecting malicious consumers.</p>
    <p><span class="badge badge-success">Achievement</span> The algorithm was applied in the internship company, serving a large listed tea beverage enterprise.</p>
  </div>

  <div class="cv-card">
    <div class="card-header">
      <h3 class="card-title">Consumer Marketing Response Prediction Based on Decoupled Attribution</h3>
      <span class="card-date">2024.04 - 2025.03</span>
    </div>
    <p><span class="badge badge-info">Description</span> Decomposed consumer repurchase behavior into "inertia" and "marketing stimulus". Used Heterogeneous Graph Neural Networks (HGNN) to model long-term user inertia, and dynamic time-series models to capture marketing fatigue and immediate reactions. Employed a decoupled attention mechanism to attribute the deviation between prediction and reality for precise consumer response prediction.</p>
  </div>

  <div class="cv-card">
    <div class="card-header">
      <h3 class="card-title">Full-Store All-Product Sales Prediction Based on Consumer Preference Mining</h3>
      <span class="card-date">2023.05 - 2024.01</span>
    </div>
    <p><span class="badge badge-info">Description</span> Adopted a two-stage deep learning approach. First, used Heterogeneous Graph Neural Networks to mine user groups with similar preferences. Then, utilized a consumer preference attention mechanism to fuse data for sales prediction.</p>
    <p><span class="badge badge-success">Achievement</span> The algorithm was launched in the internship company, serving over a thousand stores.</p>
  </div>

  <div class="cv-card">
    <div class="card-header">
      <h3 class="card-title">Shared Mobility Demand Prediction Based on Graph Neural Networks</h3>
      <span class="card-date">2022.05 - 2023.03</span>
    </div>
    <p><span class="badge badge-info">Description</span> Combined Graph Convolutional Networks (GCN) and Long Short-Term Memory (LSTM) networks to extract spatial location features and temporal demand information of shared bike stations, respectively, integrating multi-dimensional factors for demand prediction modeling.</p>
  </div>

  <div class="cv-card">
    <div class="card-header">
      <h3 class="card-title">Business Process Fraud Detection Based on Deep Learning</h3>
      <span class="card-date">2021.09 - 2022.05</span>
    </div>
    <p><span class="badge badge-info">Description</span> Comprehensively analyzed employee transaction data, personal information, and reporting texts to extract multi-dimensional features and build a fraud detection algorithm. On a real-world dataset, the model achieved a recall rate of 92% and an AUC of 97%.</p>
  </div>

  <div class="cv-card">
    <div class="card-header">
      <h3 class="card-title">Road Pedestrian Detection System Design Based on Machine Vision</h3>
      <span class="card-date">2019.12 - 2020.06</span>
    </div>
    <p style="font-size: 0.9rem; color: #64748b; margin-top: -10px; margin-bottom: 10px;">Graduation Thesis</p>
    <p><span class="badge badge-info">Description</span> Focused on road pedestrian detection scenarios, improved the traditional HOG feature detection method, integrated Gaussian Mixture Models (GMM) for foreground extraction and denoising, and combined with LBP features to enhance detection performance.</p>
    <p><span class="badge badge-success">Achievement</span> The graduation design was awarded "2020 Hefei University of Technology Excellent Undergraduate Graduation Design".</p>
  </div>


  <h2>Publications</h2>
  
  <div class="pub-item">
    <div class="pub-title">Dynamic hypergraph neural networks for consumer purchase path prediction: Integrating promotions, experiences, and store heterogeneity</div>
    <div class="pub-authors">J Wu, Q Liu, L Chen, W Zhao, H Liu</div>
    <div class="pub-venue">Decision Support Systems, 114614, 2026</div>
    <a href="https://doi.org/10.1016/j.dss.2026.114614" class="btn-download" target="_blank" rel="noopener noreferrer">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16"><path d="M8 2a5.53 5.53 0 0 0-3.594 1.342c-.766.66-1.321 1.52-1.464 2.383C1.266 6.095 0 7.555 0 9.318 0 11.366 1.708 13 3.781 13h8.906C14.502 13 16 11.57 16 9.773c0-1.636-1.242-2.969-2.834-3.194C12.923 3.999 10.69 2 8 2zm2.354 6.854l-2 2a.5.5.5 0 0 1-.708 0l-2-2a.5.5.5 0 1 1 .708-.708L7.5 9.293V5.5a.5.5.5 0 0 1 1 0v3.793l1.146-1.147a.5.5.5 0 0 1 .708.708z"/></svg>
      Download PDF
    </a>
  </div>

  <div class="pub-item">
    <div class="pub-title">Incorporating worker rivalry into task recommendations on crowdsourcing platforms: A novel framework for boosting participation and efficiency</div>
    <div class="pub-authors">H Liu, W Li, M Chen, J Wu</div>
    <div class="pub-venue">Information Processing & Management, 63 (1), 104310, 2026</div>
    <a href="https://doi.org/10.1016/j.ipm.2026.104310" class="btn-download" target="_blank" rel="noopener noreferrer">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16"><path d="M8 2a5.53 5.53 0 0 0-3.594 1.342c-.766.66-1.321 1.52-1.464 2.383C1.266 6.095 0 7.555 0 9.318 0 11.366 1.708 13 3.781 13h8.906C14.502 13 16 11.57 16 9.773c0-1.636-1.242-2.969-2.834-3.194C12.923 3.999 10.69 2 8 2zm2.354 6.854l-2 2a.5.5.5 0 0 1-.708 0l-2-2a.5.5.5 0 1 1 .708-.708L7.5 9.293V5.5a.5.5.5 0 0 1 1 0v3.793l1.146-1.147a.5.5.5 0 0 1 .708.708z"/></svg>
      Download PDF
    </a>
  </div>

  <div class="pub-item">
    <div class="pub-title">Apppoet: Large language model based android malware detection via multi-view prompt engineering</div>
    <div class="pub-authors">W Zhao, J Wu, Z Meng</div>
    <div class="pub-venue">Expert Systems with Applications, 262, 125546, 2025</div>
    <a href="https://doi.org/10.1016/j.eswa.2025.125546" class="btn-download" target="_blank" rel="noopener noreferrer">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16"><path d="M8 2a5.53 5.53 0 0 0-3.594 1.342c-.766.66-1.321 1.52-1.464 2.383C1.266 6.095 0 7.555 0 9.318 0 11.366 1.708 13 3.781 13h8.906C14.502 13 16 11.57 16 9.773c0-1.636-1.242-2.969-2.834-3.194C12.923 3.999 10.69 2 8 2zm2.354 6.854l-2 2a.5.5.5 0 0 1-.708 0l-2-2a.5.5.5 0 1 1 .708-.708L7.5 9.293V5.5a.5.5.5 0 0 1 1 0v3.793l1.146-1.147a.5.5.5 0 0 1 .708.708z"/></svg>
      Download PDF
    </a>
  </div>

  <div class="pub-item">
    <div class="pub-title">Demand prediction for bike-sharing systems: A spatial and semantic modeling approach for enhanced accuracy and operational efficiency</div>
    <div class="pub-authors">J Wu, J Feng, J Fang, H Liu</div>
    <div class="pub-venue">Computers & Industrial Engineering, 111775, 2025</div>
    <a href="https://doi.org/10.1016/j.cie.2025.111775" class="btn-download" target="_blank" rel="noopener noreferrer">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16"><path d="M8 2a5.53 5.53 0 0 0-3.594 1.342c-.766.66-1.321 1.52-1.464 2.383C1.266 6.095 0 7.555 0 9.318 0 11.366 1.708 13 3.781 13h8.906C14.502 13 16 11.57 16 9.773c0-1.636-1.242-2.969-2.834-3.194C12.923 3.999 10.69 2 8 2zm2.354 6.854l-2 2a.5.5.5 0 0 1-.708 0l-2-2a.5.5.5 0 1 1 .708-.708L7.5 9.293V5.5a.5.5.5 0 0 1 1 0v3.793l1.146-1.147a.5.5.5 0 0 1 .708.708z"/></svg>
      Download PDF
    </a>
  </div>

  <div class="pub-item">
    <div class="pub-title">Beyond the Match: Predicting Bilateral-matching Satisfaction with Multi-view Heterogeneous Graph Neural Network</div>
    <div class="pub-authors">J Feng, H Liu, J Wu, H Liu, P Zhao</div>
    <div class="pub-venue">ICIS 2025 Proceedings, 2025</div>
    <a href="https://aisel.aisnet.org/icis2025/da_bus/da_bus/4/" class="btn-download" target="_blank" rel="noopener noreferrer">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16"><path d="M8 2a5.53 5.53 0 0 0-3.594 1.342c-.766.66-1.321 1.52-1.464 2.383C1.266 6.095 0 7.555 0 9.318 0 11.366 1.708 13 3.781 13h8.906C14.502 13 16 11.57 16 9.773c0-1.636-1.242-2.969-2.834-3.194C12.923 3.999 10.69 2 8 2zm2.354 6.854l-2 2a.5.5.5 0 0 1-.708 0l-2-2a.5.5.5 0 1 1 .708-.708L7.5 9.293V5.5a.5.5.5 0 0 1 1 0v3.793l1.146-1.147a.5.5.5 0 0 1 .708.708z"/></svg>
      Download PDF
    </a>
  </div>

  <div class="pub-item">
    <div class="pub-title">Unveiling consumer preferences: A two-stage deep learning approach to enhance accuracy in multi-channel retail sales forecasting</div>
    <div class="pub-authors">J Wu, H Liu, X Yao, L Zhang</div>
    <div class="pub-venue">Expert Systems with Applications, 257, 125066, 2024</div>
    <a href="https://doi.org/10.1016/j.eswa.2024.125066" class="btn-download" target="_blank" rel="noopener noreferrer">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16"><path d="M8 2a5.53 5.53 0 0 0-3.594 1.342c-.766.66-1.321 1.52-1.464 2.383C1.266 6.095 0 7.555 0 9.318 0 11.366 1.708 13 3.781 13h8.906C14.502 13 16 11.57 16 9.773c0-1.636-1.242-2.969-2.834-3.194C12.923 3.999 10.69 2 8 2zm2.354 6.854l-2 2a.5.5.5 0 0 1-.708 0l-2-2a.5.5.5 0 1 1 .708-.708L7.5 9.293V5.5a.5.5.5 0 0 1 1 0v3.793l1.146-1.147a.5.5.5 0 0 1 .708.708z"/></svg>
      Download PDF
    </a>
  </div>

  <div class="pub-item">
    <div class="pub-title">Optimizing Restaurant Customer Flow and Revenue with Real-Time Coupon Allocation: A Deep Reinforcement Learning Approach</div>
    <div class="pub-authors">J Feng, J Wu, M Chen, J Qin</div>
    <div class="pub-venue">ICIS 2024 Proceedings, 2024</div>
    <a href="https://aisel.aisnet.org/icis2024/data_soc/data_soc/9/" class="btn-download" target="_blank" rel="noopener noreferrer">
      <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16"><path d="M8 2a5.53 5.53 0 0 0-3.594 1.342c-.766.66-1.321 1.52-1.464 2.383C1.266 6.095 0 7.555 0 9.318 0 11.366 1.708 13 3.781 13h8.906C14.502 13 16 11.57 16 9.773c0-1.636-1.242-2.969-2.834-3.194C12.923 3.999 10.69 2 8 2zm2.354 6.854l-2 2a.5.5.5 0 0 1-.708 0l-2-2a.5.5.5 0 1 1 .708-.708L7.5 9.293V5.5a.5.5.5 0 0 1 1 0v3.793l1.146-1.147a.5.5.5 0 0 1 .708.708z"/></svg>
      Download PDF
    </a>
  </div>

  <h2>Awards</h2>
  <ul style="list-style: none; padding-left: 0;">
    <li style="display:flex; align-items:flex-start; margin-bottom: 0.8rem; background: #fff; padding: 1rem; border-radius: 12px; box-shadow: 0 2px 5px rgba(0,0,0,0.02)">
      <span style="font-size: 1.2rem; margin-right: 1rem; color: #f59e0b;">🏆</span>
      <div>
        <div style="font-weight: 600; color: #1e293b;">Outstanding Graduation Thesis</div>
        <div style="font-size: 0.9rem; color: #64748b;">Hefei University of Technology • 2020.06</div>
      </div>
    </li>
    <li style="display:flex; align-items:flex-start; margin-bottom: 0.8rem; background: #fff; padding: 1rem; border-radius: 12px; box-shadow: 0 2px 5px rgba(0,0,0,0.02)">
      <span style="font-size: 1.2rem; margin-right: 1rem; color: #94a3b8;">🥈</span>
      <div>
        <div style="font-weight: 600; color: #1e293b;">Silver Award in the Creative Group, 5th "Internet+" Innovation and Entrepreneurship Competition</div>
        <div style="font-size: 0.9rem; color: #64748b;">2019.08</div>
      </div>
    </li>
    <li style="display:flex; align-items:flex-start; margin-bottom: 0.8rem; background: #fff; padding: 1rem; border-radius: 12px; box-shadow: 0 2px 5px rgba(0,0,0,0.02)">
      <span style="font-size: 1.2rem; margin-right: 1rem; color: #8b5cf6;">🏅</span>
      <div>
        <div style="font-weight: 600; color: #1e293b;">University-level "Advanced Individual"</div>
        <div style="font-size: 0.9rem; color: #64748b;">Student Work Department of the Party Committee • 2018.01</div>
      </div>
    </li>
    <li style="display:flex; align-items:flex-start; margin-bottom: 0.8rem; background: #fff; padding: 1rem; border-radius: 12px; box-shadow: 0 2px 5px rgba(0,0,0,0.02)">
      <span style="font-size: 1.2rem; margin-right: 1rem; color: #10b981;">🎖️</span>
      <div>
        <div style="font-weight: 600; color: #1e293b;">"Excellent Youth League Cadre" in the "May Fourth" Evaluation</div>
        <div style="font-size: 0.9rem; color: #64748b;">2017.05</div>
      </div>
    </li>
  </ul>

  <h2>Skills and Courses</h2>
  <div class="cv-card">
    <div style="margin-bottom: 1.5rem;">
      <h3 style="font-size: 1.1rem; color: #0f172a; margin-bottom: 0.5rem;">Core Courses & Knowledge</h3>
      <div class="skills-container">
        <span class="skill-tag">Operations Research</span>
        <span class="skill-tag">Machine Learning</span>
        <span class="skill-tag">Convex Optimization</span>
        <span class="skill-tag">Game Theory</span>
        <span class="skill-tag">Stochastic System Modeling</span>
        <span class="skill-tag">Simulation</span>
        <span class="skill-tag">Algorithm Design Science</span>
      </div>
    </div>
    
    <div>
      <h3 style="font-size: 1.1rem; color: #0f172a; margin-bottom: 0.5rem;">Language Proficiency</h3>
      <div class="skills-container">
        <span class="skill-tag" style="background: #eef2ff; border-color: #c7d2fe; color: #4338ca;">CET-6 (516)</span>
      </div>
    </div>
  </div>

</div>
