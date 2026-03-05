---
layout: archive
title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&family=Playfair+Display:ital,wght@0,600;1,600&display=swap" rel="stylesheet">

<style>
/* ------------------------------------
   Ultimate Modern CV Aesthetic 
   ------------------------------------ */
:root {
  --primary: #4338ca;
  --primary-light: #6366f1;
  --secondary: #8b5cf6;
  --accent: #f43f5e;
  --bg-gradient: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
  --card-bg: rgba(255, 255, 255, 0.85);
  --card-border: rgba(255, 255, 255, 0.6);
  --text-main: #0f172a;
  --text-muted: #64748b;
  --text-light: #94a3b8;
}

body {
  background-color: var(--bg-color) !important;
}

.modern-cv {
  font-family: 'Outfit', sans-serif;
  color: var(--text-main);
  background: var(--bg-gradient);
  padding: 3.5rem 2.5rem;
  border-radius: 32px;
  box-shadow: 
    0 25px 50px -12px rgba(0, 0, 0, 0.05),
    inset 0 0 0 1px rgba(255, 255, 255, 0.5);
  margin-top: -2rem;
  position: relative;
  overflow: hidden;
  z-index: 1;
}

/* Dynamic Animated Background Shapes */
.modern-cv::before, .modern-cv::after {
  content: '';
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  z-index: -1;
  animation: float 20s infinite ease-in-out alternate;
}

.modern-cv::before {
  width: 400px;
  height: 400px;
  background: rgba(99, 102, 241, 0.15);
  top: -100px;
  left: -100px;
}

.modern-cv::after {
  width: 500px;
  height: 500px;
  background: rgba(139, 92, 246, 0.15);
  bottom: -200px;
  right: -150px;
  animation-delay: -10s;
}

@keyframes float {
  0% { transform: translate(0, 0) scale(1); }
  50% { transform: translate(50px, 30px) scale(1.1); }
  100% { transform: translate(-30px, 60px) scale(0.9); }
}

/* Header Section */
.cv-header {
  text-align: center;
  margin-bottom: 4rem;
  position: relative;
}

.cv-header h1 {
  font-family: 'Playfair Display', serif;
  font-size: 3.5rem;
  font-weight: 600;
  line-height: 1.2;
  margin-bottom: 0.5rem;
  border-bottom: none;
  background: linear-gradient(to right, var(--primary), var(--secondary));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  display: inline-block;
}

.cv-header p {
  font-size: 1.2rem;
  color: var(--text-muted);
  font-weight: 300;
  letter-spacing: 1px;
}

/* Section Titles */
.section-header {
  font-size: 1.8rem;
  font-weight: 800;
  color: var(--text-main);
  margin-top: 4rem;
  margin-bottom: 2.5rem;
  display: flex;
  align-items: center;
  gap: 1rem;
  position: relative;
  border-bottom: none;
  text-transform: uppercase;
  letter-spacing: 2px;
}

.section-header::before {
  content: "";
  display: block;
  width: 32px;
  height: 4px;
  background: linear-gradient(90deg, var(--primary-light), var(--accent));
  border-radius: 2px;
}

/* Glassmorphism Cards */
.cv-card {
  background: var(--card-bg);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid var(--card-border);
  border-radius: 20px;
  padding: 2rem;
  margin-bottom: 2rem;
  box-shadow: 0 10px 30px -10px rgba(0,0,0,0.05);
  transition: all 0.5s cubic-bezier(0.2, 0.8, 0.2, 1);
  position: relative;
  overflow: hidden;
  z-index: 2;
}

.cv-card::before {
  content: "";
  position: absolute;
  top: 0; left: 0; right: 0; height: 100%;
  background: linear-gradient(135deg, rgba(255,255,255,0.4) 0%, rgba(255,255,255,0) 100%);
  pointer-events: none;
  opacity: 0;
  transition: opacity 0.5s ease;
}

.cv-card:hover {
  transform: translateY(-8px) scale(1.01);
  box-shadow: 0 25px 40px -15px rgba(0,0,0,0.1), 0 0 0 1px rgba(99, 102, 241, 0.1);
}

.cv-card:hover::before {
  opacity: 1;
}

/* Card Typography */
.card-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 1.25rem;
  gap: 1rem;
}

.card-title {
  font-size: 1.35rem;
  font-weight: 700;
  color: var(--text-main);
  margin: 0 0 0.25rem 0;
  line-height: 1.4;
}

.card-subtitle {
  font-size: 1.05rem;
  color: var(--primary-light);
  font-weight: 500;
  margin: 0;
}

.card-date {
  font-size: 0.85rem;
  font-weight: 700;
  color: #fff;
  background: linear-gradient(135deg, var(--text-main), var(--text-muted));
  padding: 0.4rem 1rem;
  border-radius: 9999px;
  white-space: nowrap;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

/* Timeline specific styles */
.timeline {
  position: relative;
  padding-left: 3rem;
  margin-left: 1rem;
}

.timeline::before {
  content: "";
  position: absolute;
  left: 0;
  top: 1rem;
  bottom: 1rem;
  width: 2px;
  background: linear-gradient(to bottom, var(--primary-light) 0%, rgba(99, 102, 241, 0.2) 100%);
  border-radius: 1px;
}

.timeline-item {
  position: relative;
  margin-bottom: 2.5rem;
}

.timeline-item::before {
  content: '';
  position: absolute;
  left: -3rem;
  top: 2.5rem;
  width: 16px;
  height: 16px;
  border-radius: 50%;
  background: var(--bg-gradient);
  border: 4px solid var(--primary-light);
  transform: translateX(-50%) translateY(-50%);
  z-index: 10;
  box-shadow: 0 0 0 4px rgba(99, 102, 241, 0.1);
  transition: all 0.3s ease;
}

.timeline-item:hover::before {
  background: var(--primary-light);
  box-shadow: 0 0 0 6px rgba(99, 102, 241, 0.2);
  transform: translateX(-50%) translateY(-50%) scale(1.2);
}

/* Badges */
.badge-container {
  display: flex;
  gap: 0.5rem;
  margin-bottom: 1rem;
  flex-wrap: wrap;
}

.badge {
  display: inline-flex;
  align-items: center;
  font-size: 0.75rem;
  font-weight: 700;
  padding: 0.3rem 0.8rem;
  border-radius: 8px;
  text-transform: uppercase;
  letter-spacing: 1px;
  backdrop-filter: blur(4px);
}

.badge-info { background: rgba(59, 130, 246, 0.1); color: #2563eb; border: 1px solid rgba(59, 130, 246, 0.2); }
.badge-success { background: rgba(16, 185, 129, 0.1); color: #059669; border: 1px solid rgba(16, 185, 129, 0.2); }

.cv-card p {
  color: var(--text-muted);
  line-height: 1.8;
  font-size: 1.05rem;
  margin-bottom: 0.5rem;
}

/* Publications modern list */
.pub-list {
  display: grid;
  gap: 1.5rem;
}

.pub-item {
  background: var(--card-bg);
  border-radius: 20px;
  padding: 1.8rem;
  border: 1px solid var(--card-border);
  transition: all 0.4s ease;
  position: relative;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05);
  display: flex;
  flex-direction: column;
}

.pub-item::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: 0;
  width: 0;
  height: 3px;
  background: linear-gradient(90deg, var(--primary), var(--secondary));
  transition: width 0.4s ease;
}

.pub-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 30px -5px rgba(0, 0, 0, 0.1);
  background: #fff;
}

.pub-item:hover::after {
  width: 100%;
}

.pub-title {
  font-weight: 700;
  color: var(--text-main);
  font-size: 1.15rem;
  margin-bottom: 0.75rem;
  line-height: 1.5;
}

.pub-authors {
  color: var(--text-muted);
  font-size: 1rem;
  font-weight: 300;
  margin-bottom: 0.5rem;
}

.pub-authors strong {
  color: var(--primary);
  font-weight: 600;
}

.pub-venue {
  display: inline-block;
  font-style: italic;
  font-weight: 500;
  color: var(--secondary);
  background: rgba(139, 92, 246, 0.05);
  padding: 0.2rem 0.6rem;
  border-radius: 6px;
  font-size: 0.9rem;
  margin-bottom: 1rem;
}

.btn-download {
  align-self: flex-start;
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: var(--bg-gradient);
  color: var(--primary) !important;
  text-decoration: none;
  font-weight: 600;
  font-size: 0.9rem;
  padding: 0.6rem 1.2rem;
  border-radius: 12px;
  border: 1px solid rgba(99, 102, 241, 0.2);
  transition: all 0.3s;
}

.btn-download:hover {
  background: linear-gradient(135deg, var(--primaryLight), var(--secondary));
  color: #fff !important;
  border-color: transparent;
  transform: translateY(-2px);
  box-shadow: 0 10px 15px -3px rgba(99, 102, 241, 0.3);
}

.btn-download svg {
  transition: transform 0.3s;
}

.btn-download:hover svg {
  transform: translateY(2px);
}

/* Awards Section */
.awards-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
}

.award-card {
  background: var(--card-bg);
  border: 1px solid var(--card-border);
  border-radius: 16px;
  padding: 1.5rem;
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  transition: all 0.3s ease;
}

.award-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0,0,0,0.05);
  background: #fff;
}

.award-icon {
  font-size: 2rem;
  background: linear-gradient(135deg, #fef08a, #f59e0b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  filter: drop-shadow(0 2px 4px rgba(245, 158, 11, 0.3));
}

.award-details h4 {
  margin: 0 0 0.5rem 0;
  font-size: 1.1rem;
  font-weight: 700;
  color: var(--text-main);
  line-height: 1.4;
}

.award-details p {
  margin: 0;
  font-size: 0.9rem;
  color: var(--text-muted);
}

/* Skills/Tags */
.skills-container {
  display: flex;
  flex-wrap: wrap;
  gap: 0.8rem;
  margin-top: 1rem;
}

.skill-tag {
  background: #fff;
  color: var(--text-main);
  border: 1.5px solid rgba(99, 102, 241, 0.1);
  padding: 0.6rem 1.2rem;
  border-radius: 12px;
  font-weight: 600;
  font-size: 0.95rem;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  box-shadow: 0 2px 4px rgba(0,0,0,0.02);
  cursor: default;
}

.skill-tag:hover {
  background: linear-gradient(135deg, var(--primary), var(--secondary));
  color: white;
  border-color: transparent;
  transform: translateY(-3px) scale(1.05);
  box-shadow: 0 10px 15px -3px rgba(99, 102, 241, 0.4);
}

/* Scroll Animation Classes */
.fade-in-up {
  opacity: 0;
  transform: translateY(40px);
  transition: opacity 0.8s cubic-bezier(0.2, 0.8, 0.2, 1), transform 0.8s cubic-bezier(0.2, 0.8, 0.2, 1);
}
.fade-in-up.visible {
  opacity: 1;
  transform: translateY(0);
}

/* Responsive */
@media (max-width: 768px) {
  .modern-cv {
    padding: 2rem 1.5rem;
    border-radius: 20px;
  }
  .cv-header h1 {
    font-size: 2.5rem;
  }
  .card-header {
    flex-direction: column;
  }
  .timeline {
    margin-left: 0;
    border-left: none;
    padding-left: 0;
  }
  .timeline::before {
    display: none;
  }
  .timeline-item::before {
    display: none;
  }
  .timeline-item .cv-card {
    margin-bottom: 1.5rem;
  }
  .awards-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="modern-cv">
  
  <div class="cv-header fade-in-up">
    <h1>Curriculum Vitae</h1>
    <p>wjt99@mail.ustc.edu.cn &bull; Hefei, China</p>
  </div>

  <h2 class="section-header fade-in-up">Education</h2>
  <div class="timeline">
    <div class="timeline-item fade-in-up">
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
    <div class="timeline-item fade-in-up">
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
    <div class="timeline-item fade-in-up">
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

  <h2 class="section-header fade-in-up">Internship Experience</h2>
  <div class="cv-card fade-in-up">
    <div class="card-header">
      <div>
        <h3 class="card-title">Algorithm Engineer</h3>
        <p class="card-subtitle">Qimai Technology</p>
      </div>
      <span class="card-date" style="background: linear-gradient(135deg, #10b981, #059669);">2024.06 - Present</span>
    </div>
  </div>
  <div class="cv-card fade-in-up">
    <div class="card-header">
      <div>
        <h3 class="card-title">Algorithm Development Intern</h3>
        <p class="card-subtitle">Home Original Chicken (Lao Xiang Ji)</p>
      </div>
      <span class="card-date">2023.04 - 2023.06</span>
    </div>
  </div>
  <div class="cv-card fade-in-up">
    <div class="card-header">
      <div>
        <h3 class="card-title">Quantitative Research Intern</h3>
        <p class="card-subtitle">Zhejiang Yingyang Asset</p>
      </div>
      <span class="card-date">2022.06 - 2023.03</span>
    </div>
  </div>

  <h2 class="section-header fade-in-up">Research Experience</h2>
  
  <div class="cv-card fade-in-up">
    <div class="card-header">
      <h3 class="card-title">Malicious Consumer Detection Algorithm Design</h3>
      <span class="card-date">2025.03 - 2025.08</span>
    </div>
    <div class="badge-container">
      <span class="badge badge-info">Description</span>
    </div>
    <p>Jointly modeled consumer cross-channel behavior and cognitive resource investment during fine-grained page browsing processes. Utilized Graph Neural Networks (GNN) to mine user IP address networks for detecting malicious consumers.</p>
    <div class="badge-container" style="margin-top: 1rem;">
      <span class="badge badge-success">Achievement</span>
    </div>
    <p>The algorithm was applied in the internship company, serving a large listed tea beverage enterprise.</p>
  </div>

  <div class="cv-card fade-in-up">
    <div class="card-header">
      <h3 class="card-title">Consumer Marketing Response Prediction Based on Decoupled Attribution</h3>
      <span class="card-date">2024.04 - 2025.03</span>
    </div>
    <div class="badge-container">
      <span class="badge badge-info">Description</span>
    </div>
    <p>Decomposed consumer repurchase behavior into "inertia" and "marketing stimulus". Used Heterogeneous Graph Neural Networks (HGNN) to model long-term user inertia, and dynamic time-series models to capture marketing fatigue and immediate reactions. Employed a decoupled attention mechanism to attribute the deviation between prediction and reality for precise consumer response prediction.</p>
  </div>

  <div class="cv-card fade-in-up">
    <div class="card-header">
      <h3 class="card-title">Full-Store All-Product Sales Prediction Based on Consumer Preference Mining</h3>
      <span class="card-date">2023.05 - 2024.01</span>
    </div>
    <div class="badge-container">
      <span class="badge badge-info">Description</span>
    </div>
    <p>Adopted a two-stage deep learning approach. First, used Heterogeneous Graph Neural Networks to mine user groups with similar preferences. Then, utilized a consumer preference attention mechanism to fuse data for sales prediction.</p>
    <div class="badge-container" style="margin-top: 1rem;">
      <span class="badge badge-success">Achievement</span>
    </div>
    <p>The algorithm was launched in the internship company, serving over a thousand stores.</p>
  </div>

  <div class="cv-card fade-in-up">
    <div class="card-header">
      <h3 class="card-title">Shared Mobility Demand Prediction Based on Graph Neural Networks</h3>
      <span class="card-date">2022.05 - 2023.03</span>
    </div>
    <div class="badge-container">
      <span class="badge badge-info">Description</span>
    </div>
    <p>Combined Graph Convolutional Networks (GCN) and Long Short-Term Memory (LSTM) networks to extract spatial location features and temporal demand information of shared bike stations, respectively, integrating multi-dimensional factors for demand prediction modeling.</p>
  </div>

  <div class="cv-card fade-in-up">
    <div class="card-header">
      <h3 class="card-title">Business Process Fraud Detection Based on Deep Learning</h3>
      <span class="card-date">2021.09 - 2022.05</span>
    </div>
    <div class="badge-container">
      <span class="badge badge-info">Description</span>
    </div>
    <p>Comprehensively analyzed employee transaction data, personal information, and reporting texts to extract multi-dimensional features and build a fraud detection algorithm. On a real-world dataset, the model achieved a recall rate of 92% and an AUC of 97%.</p>
  </div>

  <div class="cv-card fade-in-up">
    <div class="card-header">
      <h3 class="card-title">Road Pedestrian Detection System Design Based on Machine Vision</h3>
      <span class="card-date">2019.12 - 2020.06</span>
    </div>
    <p style="font-weight: 600; color: var(--secondary); margin-top: -10px; margin-bottom: 15px;">Graduation Thesis</p>
    <div class="badge-container">
      <span class="badge badge-info">Description</span>
    </div>
    <p>Focused on road pedestrian detection scenarios, improved the traditional HOG feature detection method, integrated Gaussian Mixture Models (GMM) for foreground extraction and denoising, and combined with LBP features to enhance detection performance.</p>
    <div class="badge-container" style="margin-top: 1rem;">
      <span class="badge badge-success">Achievement</span>
    </div>
    <p>The graduation design was awarded "2020 Hefei University of Technology Excellent Undergraduate Graduation Design".</p>
  </div>


  <h2 class="section-header fade-in-up">Publications</h2>
  <div class="pub-list">
    
    <div class="pub-item fade-in-up">
      <div class="pub-title">Dynamic hypergraph neural networks for consumer purchase path prediction: Integrating promotions, experiences, and store heterogeneity</div>
      <div class="pub-authors"><strong>J Wu</strong>, Q Liu, L Chen, W Zhao, H Liu</div>
      <div class="pub-venue">Decision Support Systems, 114614, 2026</div>
      <a href="https://doi.org/10.1016/j.dss.2026.114614" class="btn-download" target="_blank" rel="noopener noreferrer">
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
        Download PDF
      </a>
    </div>

    <div class="pub-item fade-in-up">
      <div class="pub-title">Incorporating worker rivalry into task recommendations on crowdsourcing platforms: A novel framework for boosting participation and efficiency</div>
      <div class="pub-authors">H Liu, W Li, M Chen, <strong>J Wu</strong></div>
      <div class="pub-venue">Information Processing & Management, 63 (1), 104310, 2026</div>
      <a href="https://doi.org/10.1016/j.ipm.2026.104310" class="btn-download" target="_blank" rel="noopener noreferrer">
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
        Download PDF
      </a>
    </div>

    <div class="pub-item fade-in-up">
      <div class="pub-title">Apppoet: Large language model based android malware detection via multi-view prompt engineering</div>
      <div class="pub-authors">W Zhao, <strong>J Wu</strong>, Z Meng</div>
      <div class="pub-venue">Expert Systems with Applications, 262, 125546, 2025</div>
      <a href="https://doi.org/10.1016/j.eswa.2025.125546" class="btn-download" target="_blank" rel="noopener noreferrer">
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
        Download PDF
      </a>
    </div>

    <div class="pub-item fade-in-up">
      <div class="pub-title">Demand prediction for bike-sharing systems: A spatial and semantic modeling approach for enhanced accuracy and operational efficiency</div>
      <div class="pub-authors"><strong>J Wu</strong>, J Feng, J Fang, H Liu</div>
      <div class="pub-venue">Computers & Industrial Engineering, 111775, 2025</div>
      <a href="https://doi.org/10.1016/j.cie.2025.111775" class="btn-download" target="_blank" rel="noopener noreferrer">
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
        Download PDF
      </a>
    </div>

    <div class="pub-item fade-in-up">
      <div class="pub-title">Beyond the Match: Predicting Bilateral-matching Satisfaction with Multi-view Heterogeneous Graph Neural Network</div>
      <div class="pub-authors">J Feng, H Liu, <strong>J Wu</strong>, H Liu, P Zhao</div>
      <div class="pub-venue">ICIS 2025 Proceedings</div>
      <a href="https://aisel.aisnet.org/icis2025/da_bus/da_bus/4/" class="btn-download" target="_blank" rel="noopener noreferrer">
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
        Download PDF
      </a>
    </div>

    <div class="pub-item fade-in-up">
      <div class="pub-title">Unveiling consumer preferences: A two-stage deep learning approach to enhance accuracy in multi-channel retail sales forecasting</div>
      <div class="pub-authors"><strong>J Wu</strong>, H Liu, X Yao, L Zhang</div>
      <div class="pub-venue">Expert Systems with Applications, 257, 125066, 2024</div>
      <a href="https://doi.org/10.1016/j.eswa.2024.125066" class="btn-download" target="_blank" rel="noopener noreferrer">
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
        Download PDF
      </a>
    </div>

    <div class="pub-item fade-in-up">
      <div class="pub-title">Optimizing Restaurant Customer Flow and Revenue with Real-Time Coupon Allocation: A Deep Reinforcement Learning Approach</div>
      <div class="pub-authors">J Feng, <strong>J Wu</strong>, M Chen, J Qin</div>
      <div class="pub-venue">ICIS 2024 Proceedings</div>
      <a href="https://aisel.aisnet.org/icis2024/data_soc/data_soc/9/" class="btn-download" target="_blank" rel="noopener noreferrer">
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
        Download PDF
      </a>
    </div>

  </div>

  <h2 class="section-header fade-in-up">Awards</h2>
  <div class="awards-grid">
    <div class="award-card fade-in-up">
      <div class="award-icon">🏆</div>
      <div class="award-details">
        <h4>Outstanding Graduation Thesis</h4>
        <p>Hefei University of Technology • 2020.06</p>
      </div>
    </div>
    <div class="award-card fade-in-up">
      <div class="award-icon">🥈</div>
      <div class="award-details">
        <h4>Silver Award, Creative Group</h4>
        <p>5th "Internet+" Innovation and Entrepreneurship Competition • 2019.08</p>
      </div>
    </div>
    <div class="award-card fade-in-up">
      <div class="award-icon">🌟</div>
      <div class="award-details">
        <h4>University-level "Advanced Individual"</h4>
        <p>Student Work Department • 2018.01</p>
      </div>
    </div>
    <div class="award-card fade-in-up">
      <div class="award-icon">🎖️</div>
      <div class="award-details">
        <h4>"Excellent Youth League Cadre"</h4>
        <p>"May Fourth" Evaluation • 2017.05</p>
      </div>
    </div>
  </div>

  <h2 class="section-header fade-in-up">Skills and Courses</h2>
  <div class="cv-card fade-in-up">
    <div style="margin-bottom: 2rem;">
      <h3 style="font-size: 1.2rem; color: var(--text-main); margin-bottom: 1rem; font-weight: 700;">Core Courses & Knowledge</h3>
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
      <h3 style="font-size: 1.2rem; color: var(--text-main); margin-bottom: 1rem; font-weight: 700;">Language Proficiency</h3>
      <div class="skills-container">
        <span class="skill-tag" style="background: linear-gradient(135deg, #eef2ff, #e0e7ff); border-color: #c7d2fe; color: #4338ca;">CET-6 (516)</span>
      </div>
    </div>
  </div>

</div>

<script>
// Dynamic Scroll Animation Script
document.addEventListener("DOMContentLoaded", function() {
  const observerOptions = {
    threshold: 0.1,
    rootMargin: "0px 0px -50px 0px"
  };

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
        observer.unobserve(entry.target); // Animate only once
      }
    });
  }, observerOptions);

  // Small delay to ensure styles are loaded
  setTimeout(() => {
    document.querySelectorAll('.fade-in-up').forEach((el, index) => {
      // Add staggered delay for child elements
      el.style.transitionDelay = `${(index % 5) * 0.1}s`;
      observer.observe(el);
    });
  }, 100);
});
</script>
