<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Srinivasu Botta · AI & Data Science Portfolio</title>
  <!-- Google Fonts + Font Awesome 6 (free icons) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(145deg, #e9eff7 0%, #d9e2ef 100%);
      font-family: 'Inter', sans-serif;
      padding: 2rem 1.5rem;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    /* main card - modern glass border + smooth shadows */
    .portfolio-card {
      max-width: 1380px;
      width: 100%;
      background: rgba(255, 255, 255, 0.97);
      backdrop-filter: blur(0px);
      border-radius: 2.5rem;
      box-shadow: 0 25px 45px -12px rgba(0, 0, 0, 0.2), 0 4px 14px rgba(0, 0, 0, 0.02);
      overflow: hidden;
      transition: transform 0.2s ease, box-shadow 0.2s;
      border: 1px solid rgba(255, 255, 255, 0.7);
    }

    .portfolio-card:hover {
      box-shadow: 0 30px 50px -18px rgba(0, 0, 0, 0.25);
    }

    .container {
      padding: 2rem 2.2rem;
    }

    /* header with status ribbon */
    .header-row {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: flex-start;
      margin-bottom: 1.5rem;
      gap: 1rem;
    }

    .title-badge h1 {
      font-size: 2.6rem;
      font-weight: 800;
      background: linear-gradient(135deg, #0B2B4E, #1F5E8E);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      letter-spacing: -0.02em;
    }

    .title-badge p {
      font-size: 0.95rem;
      color: #2c3e66;
      font-weight: 500;
      margin-top: 0.35rem;
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      gap: 12px;
    }

    .open-badge {
      background: #1a4d3e;
      color: white;
      font-size: 0.7rem;
      font-weight: 600;
      padding: 0.3rem 1rem;
      border-radius: 40px;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.05);
    }

    .open-badge i {
      font-size: 0.75rem;
    }

    /* metrics / stats row */
    .stats-ribbon {
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
      background: #f0f4fa;
      padding: 0.85rem 1.8rem;
      border-radius: 60px;
      margin: 1rem 0 1.8rem 0;
      justify-content: space-between;
      align-items: center;
    }

    .stat-item {
      text-align: center;
    }

    .stat-number {
      font-size: 1.7rem;
      font-weight: 800;
      color: #0F2E4D;
      line-height: 1.2;
    }

    .stat-label {
      font-size: 0.7rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.5px;
      color: #4a627a;
    }

    /* skill proficiency bars */
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 1rem;
      margin: 1.5rem 0 1.8rem;
      background: #ffffffd9;
      border-radius: 2rem;
      padding: 1.2rem 1.5rem;
      border: 1px solid #eef2f8;
    }

    .skill-row {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 0.8rem;
      font-size: 0.85rem;
      font-weight: 500;
    }

    .skill-name i {
      width: 24px;
      color: #2b6e9e;
    }

    .skill-bar-bg {
      flex: 1;
      height: 8px;
      background: #e2e8f0;
      border-radius: 12px;
      overflow: hidden;
    }

    .skill-bar-fill {
      height: 100%;
      background: linear-gradient(90deg, #2c7da0, #1f5068);
      border-radius: 12px;
      width: 0%;
    }

    /* tech stack bubbles */
    .tech-stack-section {
      margin: 2rem 0 1.8rem;
    }

    .section-badge {
      font-size: 1rem;
      font-weight: 700;
      margin-bottom: 1rem;
      letter-spacing: -0.2px;
      display: flex;
      align-items: center;
      gap: 10px;
      border-left: 4px solid #1f6e8c;
      padding-left: 14px;
    }

    .tech-icons {
      display: flex;
      flex-wrap: wrap;
      gap: 0.7rem;
      background: #f9fbfe;
      padding: 1.2rem 1.2rem;
      border-radius: 2rem;
    }

    .tech-bubble {
      background: white;
      border-radius: 40px;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
      font-weight: 500;
      box-shadow: 0 2px 6px rgba(0,0,0,0.02);
      border: 1px solid #e2edf7;
      transition: all 0.2s ease;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .tech-bubble i, .tech-bubble span {
      font-size: 0.85rem;
    }

    .tech-bubble:hover {
      transform: translateY(-2px);
      border-color: #80b6d4;
      box-shadow: 0 8px 18px rgba(0, 0, 0, 0.05);
      background: #ffffff;
    }

    /* projects & roadmap grid */
    .projects-roadmap {
      display: grid;
      grid-template-columns: 1fr 0.9fr;
      gap: 1.8rem;
      margin: 2rem 0;
    }

    .projects-grid {
      background: #fefefe;
      border-radius: 1.8rem;
    }

    .project-card {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      border-bottom: 1px solid #eef2f0;
      padding: 1rem 0.2rem;
    }

    .project-info h4 {
      font-weight: 800;
      font-size: 1rem;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .project-stats {
      font-size: 0.7rem;
      font-weight: 600;
      color: #1f6e8c;
      background: #e5f2f7;
      border-radius: 40px;
      padding: 0.2rem 0.8rem;
      white-space: nowrap;
    }

    .roadmap {
      background: #f9fafc;
      border-radius: 1.8rem;
      padding: 1rem 1.2rem;
    }

    .roadmap-item {
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 0.65rem 0;
      border-bottom: 1px dashed #e0e7ed;
    }

    .status-icon {
      width: 28px;
      text-align: center;
    }

    .completed {
      color: #2b7a4b;
    }

    .progress {
      color: #e6a017;
    }

    /* certifications + connect row */
    .cert-connect {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      margin: 1.5rem 0;
      gap: 1rem;
    }

    .certs {
      background: #f3f6fc;
      border-radius: 1.5rem;
      padding: 1rem 1.5rem;
      flex: 2;
    }

    .cert-badge {
      font-weight: 500;
      font-size: 0.8rem;
      margin: 0.4rem 0;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .connect-links {
      background: #eef3fa;
      border-radius: 1.5rem;
      padding: 1rem 1.5rem;
      flex: 1;
      text-align: center;
    }

    .connect-links a {
      display: inline-flex;
      margin: 0.5rem 0.7rem;
      font-size: 1.4rem;
      color: #2c3e66;
      transition: 0.2s;
    }

    .connect-links a:hover {
      color: #0f5b86;
      transform: scale(1.05);
    }

    /* quote + code loop */
    .footer-quote {
      margin-top: 1.8rem;
      background: #0a1927;
      color: #bfd9e8;
      border-radius: 2rem;
      padding: 1.2rem 1.8rem;
      font-family: monospace;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      align-items: center;
    }

    .quote-text {
      font-style: italic;
      font-weight: 400;
      letter-spacing: 0.3px;
    }

    .code-loop {
      background: #0000002e;
      padding: 0.4rem 1rem;
      border-radius: 2rem;
      font-size: 0.75rem;
    }

    @media (max-width: 780px) {
      .container {
        padding: 1.2rem;
      }
      .projects-roadmap {
        grid-template-columns: 1fr;
        gap: 1.2rem;
      }
      .stats-ribbon {
        gap: 1rem;
        justify-content: center;
      }
      .title-badge h1 {
        font-size: 2rem;
      }
    }

    .glow-text {
      background: radial-gradient(circle at 30% 10%, #164863, #072437);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }

    i, .fas, .fab {
      margin-right: 4px;
    }

    /* extra micro animation */
    @keyframes subtlePulse {
      0% { opacity: 0.9; }
      100% { opacity: 1; }
    }
  </style>
</head>
<body>
<div class="portfolio-card">
  <div class="container">
    <!-- header row -->
    <div class="header-row">
      <div class="title-badge">
        <h1>Srinivasu Botta</h1>
        <p><i class="fas fa-graduation-cap"></i> B.Tech - Artificial Intelligence & Data Science · Andhra Pradesh, India
          <span class="open-badge"><i class="fas fa-briefcase"></i> Open to internships & research collabs</span>
        </p>
      </div>
    </div>

    <!-- stats metrics (12+,20+,30+,500+,5+) -->
    <div class="stats-ribbon">
      <div class="stat-item"><div class="stat-number">12+</div><div class="stat-label">ML Models</div></div>
      <div class="stat-item"><div class="stat-number">20+</div><div class="stat-label">Research Papers</div></div>
      <div class="stat-item"><div class="stat-number">30+</div><div class="stat-label">Kaggle Notebooks</div></div>
      <div class="stat-item"><div class="stat-number">500+</div><div class="stat-label">Code Commits</div></div>
      <div class="stat-item"><div class="stat-number">5+</div><div class="stat-label">End-to-end Pipelines</div></div>
    </div>

    <!-- skill proficiency (dynamic bars) -->
    <div class="skills-grid">
      <div class="skill-row"><span class="skill-name"><i class="fab fa-python"></i> Python</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 95%"></div></div><span>95%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-chart-line"></i> Data analysis</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 90%"></div></div><span>90%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-chart-simple"></i> Data visualization</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 88%"></div></div><span>88%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-database"></i> SQL</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 85%"></div></div><span>85%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-brain"></i> Machine Learning</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 92%"></div></div><span>92%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-microchip"></i> Deep Learning</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 88%"></div></div><span>88%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-language"></i> NLP / LLMs</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 85%"></div></div><span>85%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-eye"></i> Computer Vision</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 82%"></div></div><span>82%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-chart-line"></i> Time series</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 78%"></div></div><span>78%</span></div>
      <div class="skill-row"><span class="skill-name"><i class="fas fa-cloud-upload-alt"></i> MLOps / Deploy</span><div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 75%"></div></div><span>75%</span></div>
    </div>

    <!-- TECH STACK - enriched bubbles -->
    <div class="tech-stack-section">
      <div class="section-badge"><i class="fas fa-cubes"></i> TECH STACK</div>
      <div class="tech-icons">
        <div class="tech-bubble"><i class="fab fa-python"></i> Python</div><div class="tech-bubble">R</div><div class="tech-bubble"><i class="fas fa-database"></i> SQL</div><div class="tech-bubble"><i class="fab fa-cuttlefish"></i> C++</div>
        <div class="tech-bubble"><i class="fas fa-brain"></i> TensorFlow</div><div class="tech-bubble"><i class="fas fa-fire"></i> PyTorch</div><div class="tech-bubble"><i class="fas fa-robot"></i> HuggingFace</div>
        <div class="tech-bubble"><i class="fas fa-code-branch"></i> Transformers</div><div class="tech-bubble">Keras</div><div class="tech-bubble">Scikit-learn</div>
        <div class="tech-bubble">NLTK / spaCy</div><div class="tech-bubble">OpenCV · YOLO</div><div class="tech-bubble">Pandas/NumPy</div>
        <div class="tech-bubble">Streamlit · FastAPI</div><div class="tech-bubble">Flask · Docker</div><div class="tech-bubble">AWS · GCP · Azure</div>
        <div class="tech-bubble">MySQL · MongoDB</div><div class="tech-bubble">PostgreSQL</div>
      </div>
    </div>

    <!-- Currently learning + RAG / LLMs highlight -->
    <div style="margin: 0.5rem 0 0.2rem">
      <div class="section-badge"><i class="fas fa-graduation-cap"></i> CURRENTLY LEARNING 
        <span style="background:#ffe8cf; font-size:0.7rem; padding:2px 12px; border-radius:40px; margin-left:12px;"><i class="fas fa-microphone-alt"></i> LLMs & Prompt Engineering · Retrieval-Augmented Generation (RAG)</span>
      </div>
    </div>

    <!-- PROJECTS + ROADMAP dual column -->
    <div class="projects-roadmap">
      <div class="projects-grid">
        <div class="section-badge"><i class="fas fa-star"></i> FEATURED PROJECTS</div>
        <div class="project-card"><div class="project-info"><h4><i class="fas fa-eye"></i> Neural Image Classifier</h4><span>Multi-class deep CNN for image recognition</span></div><div class="project-stats"><i class="fas fa-chart-line"></i> 95%+ accuracy</div></div>
        <div class="project-card"><div class="project-info"><h4><i class="fas fa-comment-dots"></i> NLP Sentiment Engine</h4><span>Customer review sentiment analysis REST API</span></div><div class="project-stats"><i class="fas fa-cloud-upload-alt"></i> Deployed API</div></div>
        <div class="project-card"><div class="project-info"><h4><i class="fas fa-thumbs-up"></i> AI Recommender System</h4><span>Personalized content recommendation engine</span></div><div class="project-stats"><i class="fas fa-chart-simple"></i> 1M+ interactions</div></div>
        <div class="project-card"><div class="project-info"><h4><i class="fas fa-chart-line"></i> ML Analytics Dashboard</h4><span>Real-time predictive analytics & visualization</span></div><div class="project-stats"><i class="fas fa-chart-pie"></i> End-to-end pipeline</div></div>
        <div class="project-card"><div class="project-info"><h4><i class="fas fa-chart-simple"></i> Stock LSTM Predictor</h4><span>Market trend prediction via sequence modeling</span></div><div class="project-stats">📉 15% MAPE</div></div>
        <div class="project-card"><div class="project-info"><h4><i class="fas fa-video"></i> CV Object Detector</h4><span>Real-time object detection & tracking pipeline</span></div><div class="project-stats"><i class="fas fa-tachometer-alt"></i> 30+ FPS on CPU</div></div>
      </div>

      <!-- learning roadmap with status icons -->
      <div class="roadmap">
        <div class="section-badge"><i class="fas fa-map-signs"></i> LEARNING ROADMAP</div>
        <div class="roadmap-item"><div class="status-icon completed"><i class="fas fa-check-circle"></i></div><div>Python & data science fundamentals</div><span style="margin-left:auto; font-size:0.7rem;">completed</span></div>
        <div class="roadmap-item"><div class="status-icon completed"><i class="fas fa-check-circle"></i></div><div>Classical machine learning</div><span style="margin-left:auto;">✔️</span></div>
        <div class="roadmap-item"><div class="status-icon completed"><i class="fas fa-check-circle"></i></div><div>Deep learning & neural networks</div><span style="margin-left:auto;">✔️</span></div>
        <div class="roadmap-item"><div class="status-icon completed"><i class="fas fa-check-circle"></i></div><div>Computer vision & NLP</div><span style="margin-left:auto;">✔️</span></div>
        <div class="roadmap-item"><div class="status-icon progress"><i class="fas fa-spinner fa-pulse"></i></div><div>LLMs & GenAI</div><span style="margin-left:auto; background:#f2e3c2; padding:2px 10px; border-radius:20px;">in progress</span></div>
        <div class="roadmap-item"><div class="status-icon progress"><i class="fas fa-hourglass-half"></i></div><div>MLOps & production AI</div><span style="margin-left:auto;">in progress</span></div>
        <div class="roadmap-item"><div class="status-icon"><i class="fas fa-future"></i></div><div>Multimodal AI & AI agents</div><span style="margin-left:auto;">next ⏩</span></div>
        <div class="roadmap-item"><div class="status-icon"><i class="fas fa-chalkboard"></i></div><div>MLOps & Model Deployment at Scale</div><span style="margin-left:auto;">next</span></div>
        <div class="roadmap-item"><div class="status-icon"><i class="fas fa-language"></i></div><div>Multimodal AI — Vision + Language</div><span style="margin-left:auto;">exploring</span></div>
      </div>
    </div>

    <!-- certifications + connect with socials -->
    <div class="cert-connect">
      <div class="certs">
        <div class="section-badge"><i class="fas fa-certificate"></i> CERTIFICATIONS</div>
        <div class="cert-badge"><i class="fas fa-check-circle" style="color:#1f6e8c"></i> Machine Learning Specialization</div>
        <div class="cert-badge"><i class="fas fa-check-circle" style="color:#1f6e8c"></i> IBM Data Science Professional</div>
        <div class="cert-badge"><i class="fas fa-check-circle" style="color:#1f6e8c"></i> Python for Data Science & AI</div>
        <div class="cert-badge"><i class="fas fa-check-circle" style="color:#1f6e8c"></i> Deep Learning Specialization</div>
        <div class="cert-badge"><i class="fab fa-google"></i> Google Cloud ML Engineer</div>
        <div class="cert-badge"><i class="fas fa-microchip"></i> TensorFlow Developer Certificate</div>
      </div>
      <div class="connect-links">
        <div class="section-badge"><i class="fas fa-share-alt"></i> CONNECT WITH ME</div>
        <a href="#" target="_blank"><i class="fab fa-linkedin fa-2x"></i></a>
        <a href="#" target="_blank"><i class="fas fa-envelope fa-2x"></i></a>
        <a href="#" target="_blank"><i class="fab fa-kaggle fa-2x"></i></a>
        <a href="#" target="_blank"><i class="fas fa-robot"></i> HF</a>
        <div style="margin-top: 12px; font-size: 0.7rem; color:#366f8c"><i class="fab fa-github"></i> github.com/srinivasu-ai</div>
      </div>
    </div>

    <!-- quote + loop (while eat sleep code) -->
    <div class="footer-quote">
      <div class="quote-text"><i class="fas fa-quote-left"></i> "The best way to predict the future is to build it."</div>
      <div class="code-loop">
        <i class="fas fa-code"></i> while(true) { eat(); sleep(); code(); repeat(); }
      </div>
    </div>

    <!-- micro stats footer (accuracy, fps) -->
    <div style="display: flex; justify-content: flex-end; margin-top: 1rem; gap: 1.2rem; font-size:0.7rem; color:#446688">
      <span><i class="fas fa-chart-line"></i> 95%+ accuracy</span> 
      <span><i class="fas fa-tachometer-alt"></i> 30 FPS on CPU</span> 
      <span><i class="fas fa-chart-line"></i> 15% MAPE</span> 
      <span><i class="fas fa-database"></i> 1M+ interactions</span>
    </div>
  </div>
</div>
</body>
</html>
