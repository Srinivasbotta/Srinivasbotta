<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Srinivasu Botta · AI & Data Science Portfolio</title>
  <!-- Tailwind CSS v3 + Font Awesome + Google Fonts -->
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      font-family: 'Inter', sans-serif;
    }
    /* custom gradient & subtle animations (Tailwind couldn't cover fully) */
    .gradient-text {
      background: linear-gradient(135deg, #0B2B4E, #1F5E8E);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }
    .skill-fill {
      background: linear-gradient(90deg, #2c7da0, #1f5068);
    }
    .hover-lift:hover {
      transform: translateY(-2px);
      transition: all 0.2s ease;
    }
    .card-hover:hover {
      transform: translateY(-4px);
      box-shadow: 0 30px 50px -18px rgba(0, 0, 0, 0.25);
      transition: all 0.25s ease;
    }
    .tech-bubble-hover:hover {
      transform: translateY(-2px);
      border-color: #80b6d4;
      box-shadow: 0 8px 18px rgba(0, 0, 0, 0.05);
      background-color: #ffffff;
    }
    .status-icon {
      width: 28px;
      text-align: center;
    }
  </style>
</head>
<body class="bg-gradient-to-br from-[#e9eff7] to-[#d9e2ef] p-6 md:p-8 flex items-center justify-center min-h-screen">

  <!-- Main Card: glassmorphic + smooth corners -->
  <div class="max-w-[1380px] w-full bg-white/97 backdrop-blur-0 rounded-[2.5rem] shadow-xl border border-white/70 transition-all duration-200 card-hover">
    <div class="p-5 md:p-8 lg:p-9">

      <!-- ========= HEADER SECTION ========= -->
      <div class="flex flex-wrap justify-between items-start gap-4 mb-5">
        <div>
          <h1 class="text-3xl md:text-4xl font-extrabold gradient-text tracking-tight">Srinivasu Botta</h1>
          <div class="flex flex-wrap items-center gap-3 mt-2 text-sm md:text-base text-slate-700">
            <i class="fas fa-graduation-cap text-[#1f6e8c]"></i>
            <span>B.Tech - Artificial Intelligence & Data Science · Andhra Pradesh, India</span>
            <span class="inline-flex items-center gap-2 bg-[#1a4d3e] text-white text-[0.7rem] font-semibold px-3 py-1.5 rounded-full shadow-sm">
              <i class="fas fa-briefcase text-xs"></i> Open to internships & research collabs
            </span>
          </div>
        </div>
      </div>

      <!-- ========= STATS RIBBON (12+ / 20+ / 30+ / 500+ / 5+) ========= -->
      <div class="flex flex-wrap justify-between items-center gap-5 bg-[#f0f4fa] py-3 px-5 md:px-7 rounded-full my-5">
        <div class="text-center"><div class="text-2xl md:text-3xl font-black text-[#0F2E4D]">12+</div><div class="text-[0.65rem] font-semibold uppercase tracking-wide text-slate-500">ML Models</div></div>
        <div class="text-center"><div class="text-2xl md:text-3xl font-black text-[#0F2E4D]">20+</div><div class="text-[0.65rem] font-semibold uppercase tracking-wide text-slate-500">Research Papers</div></div>
        <div class="text-center"><div class="text-2xl md:text-3xl font-black text-[#0F2E4D]">30+</div><div class="text-[0.65rem] font-semibold uppercase tracking-wide text-slate-500">Kaggle Notebooks</div></div>
        <div class="text-center"><div class="text-2xl md:text-3xl font-black text-[#0F2E4D]">500+</div><div class="text-[0.65rem] font-semibold uppercase tracking-wide text-slate-500">Code Commits</div></div>
        <div class="text-center"><div class="text-2xl md:text-3xl font-black text-[#0F2E4D]">5+</div><div class="text-[0.65rem] font-semibold uppercase tracking-wide text-slate-500">End-to-end Pipelines</div></div>
      </div>

      <!-- ========= SKILL PROFICIENCY BARS ========= -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-4 bg-white/90 rounded-2xl p-5 border border-[#eef2f8] my-6">
        <!-- Python -->
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fab fa-python text-[#2b6e9e]"></i> Python</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:95%"></div></div><span class="text-xs">95%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-chart-line text-[#2b6e9e]"></i> Data analysis</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:90%"></div></div><span class="text-xs">90%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-chart-simple text-[#2b6e9e]"></i> Data visualization</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:88%"></div></div><span class="text-xs">88%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-database text-[#2b6e9e]"></i> SQL</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:85%"></div></div><span class="text-xs">85%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-brain text-[#2b6e9e]"></i> Machine Learning</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:92%"></div></div><span class="text-xs">92%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-microchip text-[#2b6e9e]"></i> Deep Learning</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:88%"></div></div><span class="text-xs">88%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-language text-[#2b6e9e]"></i> NLP / LLMs</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:85%"></div></div><span class="text-xs">85%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-eye text-[#2b6e9e]"></i> Computer Vision</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:82%"></div></div><span class="text-xs">82%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-chart-line text-[#2b6e9e]"></i> Time series</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:78%"></div></div><span class="text-xs">78%</span></div>
        <div class="flex items-center justify-between gap-3 text-sm font-medium"><div class="w-28 flex items-center gap-1"><i class="fas fa-cloud-upload-alt text-[#2b6e9e]"></i> MLOps / Deploy</div><div class="flex-1 h-2 bg-gray-200 rounded-full overflow-hidden"><div class="h-full skill-fill rounded-full" style="width:75%"></div></div><span class="text-xs">75%</span></div>
      </div>

      <!-- ========= TECH STACK (modern bubble grid) ========= -->
      <div class="mt-6 mb-7">
        <div class="flex items-center gap-2 border-l-4 border-[#1f6e8c] pl-3 mb-4"><i class="fas fa-cubes text-[#1f6e8c]"></i><span class="font-bold text-gray-800">TECH STACK</span></div>
        <div class="flex flex-wrap gap-2 bg-[#f9fbfe] p-4 rounded-2xl">
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all"><i class="fab fa-python"></i> Python</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all">R</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all"><i class="fas fa-database"></i> SQL</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all"><i class="fab fa-cuttlefish"></i> C++</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all"><i class="fas fa-brain"></i> TensorFlow</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all"><i class="fas fa-fire"></i> PyTorch</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all"><i class="fas fa-robot"></i> HuggingFace</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium flex items-center gap-1 shadow-sm tech-bubble-hover transition-all">Transformers</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">Keras</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">Scikit-learn</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">NLTK / spaCy</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">OpenCV · YOLO</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">Pandas/NumPy</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">Streamlit · FastAPI</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">Flask · Docker</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">AWS · GCP · Azure</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">MySQL · MongoDB</span>
          <span class="bg-white border border-[#e2edf7] rounded-full px-3 py-1.5 text-xs font-medium shadow-sm tech-bubble-hover transition-all">PostgreSQL</span>
        </div>
      </div>

      <!-- ========= CURRENTLY LEARNING (highlight) ========= -->
      <div class="mt-2 mb-2">
        <div class="flex items-center gap-2 border-l-4 border-[#1f6e8c] pl-3 mb-2"><i class="fas fa-graduation-cap text-[#1f6e8c]"></i><span class="font-bold text-gray-800">CURRENTLY LEARNING</span>
          <span class="bg-amber-50 text-amber-800 text-[0.7rem] font-semibold px-3 py-1 rounded-full ml-2"><i class="fas fa-microphone-alt mr-1"></i> LLMs & Prompt Engineering · Retrieval-Augmented Generation (RAG)</span>
        </div>
      </div>

      <!-- ========= PROJECTS + ROADMAP (2 columns) ========= -->
      <div class="grid grid-cols-1 lg:grid-cols-[1fr_0.9fr] gap-6 my-7">
        <!-- LEFT: FEATURED PROJECTS -->
        <div>
          <div class="flex items-center gap-2 border-l-4 border-[#1f6e8c] pl-3 mb-3"><i class="fas fa-star text-[#1f6e8c]"></i><span class="font-bold text-gray-800">FEATURED PROJECTS</span></div>
          <div class="space-y-3">
            <div class="flex flex-wrap items-center justify-between border-b border-gray-100 pb-3"><div><h4 class="font-extrabold text-sm flex gap-2"><i class="fas fa-eye text-[#1f6e8c]"></i> Neural Image Classifier</h4><span class="text-xs text-gray-500">Multi-class deep CNN for image recognition</span></div><div class="text-[0.7rem] font-semibold bg-[#e5f2f7] px-3 py-1 rounded-full text-[#1f6e8c]"><i class="fas fa-chart-line"></i> 95%+ accuracy</div></div>
            <div class="flex flex-wrap items-center justify-between border-b border-gray-100 pb-3"><div><h4 class="font-extrabold text-sm flex gap-2"><i class="fas fa-comment-dots text-[#1f6e8c]"></i> NLP Sentiment Engine</h4><span class="text-xs text-gray-500">Customer review sentiment analysis REST API</span></div><div class="text-[0.7rem] font-semibold bg-[#e5f2f7] px-3 py-1 rounded-full text-[#1f6e8c]"><i class="fas fa-cloud-upload-alt"></i> Deployed API</div></div>
            <div class="flex flex-wrap items-center justify-between border-b border-gray-100 pb-3"><div><h4 class="font-extrabold text-sm flex gap-2"><i class="fas fa-thumbs-up text-[#1f6e8c]"></i> AI Recommender System</h4><span class="text-xs text-gray-500">Personalized content recommendation engine</span></div><div class="text-[0.7rem] font-semibold bg-[#e5f2f7] px-3 py-1 rounded-full text-[#1f6e8c]"><i class="fas fa-chart-simple"></i> 1M+ interactions</div></div>
            <div class="flex flex-wrap items-center justify-between border-b border-gray-100 pb-3"><div><h4 class="font-extrabold text-sm flex gap-2"><i class="fas fa-chart-line text-[#1f6e8c]"></i> ML Analytics Dashboard</h4><span class="text-xs text-gray-500">Real-time predictive analytics & visualization</span></div><div class="text-[0.7rem] font-semibold bg-[#e5f2f7] px-3 py-1 rounded-full text-[#1f6e8c]">End-to-end pipeline</div></div>
            <div class="flex flex-wrap items-center justify-between border-b border-gray-100 pb-3"><div><h4 class="font-extrabold text-sm flex gap-2"><i class="fas fa-chart-simple text-[#1f6e8c]"></i> Stock LSTM Predictor</h4><span class="text-xs text-gray-500">Market trend prediction via sequence modeling</span></div><div class="text-[0.7rem] font-semibold bg-[#e5f2f7] px-3 py-1 rounded-full text-[#1f6e8c]">📉 15% MAPE</div></div>
            <div class="flex flex-wrap items-center justify-between pb-1"><div><h4 class="font-extrabold text-sm flex gap-2"><i class="fas fa-video text-[#1f6e8c]"></i> CV Object Detector</h4><span class="text-xs text-gray-500">Real-time object detection & tracking pipeline</span></div><div class="text-[0.7rem] font-semibold bg-[#e5f2f7] px-3 py-1 rounded-full text-[#1f6e8c]"><i class="fas fa-tachometer-alt"></i> 30+ FPS on CPU</div></div>
          </div>
        </div>

        <!-- RIGHT: LEARNING ROADMAP with status -->
        <div class="bg-[#f9fafc] rounded-2xl p-4">
          <div class="flex items-center gap-2 border-l-4 border-[#1f6e8c] pl-3 mb-3"><i class="fas fa-map-signs"></i><span class="font-bold text-gray-800">LEARNING ROADMAP</span></div>
          <div class="space-y-2">
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-green-700"><i class="fas fa-check-circle"></i></div><span class="text-sm">Python & data science fundamentals</span><span class="ml-auto text-[0.65rem] font-medium text-green-700">completed</span></div>
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-green-700"><i class="fas fa-check-circle"></i></div><span class="text-sm">Classical machine learning</span><span class="ml-auto text-[0.65rem]">✔️</span></div>
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-green-700"><i class="fas fa-check-circle"></i></div><span class="text-sm">Deep learning & neural networks</span><span class="ml-auto text-[0.65rem]">✔️</span></div>
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-green-700"><i class="fas fa-check-circle"></i></div><span class="text-sm">Computer vision & NLP</span><span class="ml-auto text-[0.65rem]">✔️</span></div>
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-amber-600"><i class="fas fa-spinner fa-pulse"></i></div><span class="text-sm font-medium">LLMs & GenAI</span><span class="ml-auto bg-amber-100 text-amber-700 text-[0.6rem] font-bold px-2 py-0.5 rounded-full">in progress</span></div>
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-amber-600"><i class="fas fa-hourglass-half"></i></div><span class="text-sm">MLOps & production AI</span><span class="ml-auto text-[0.65rem] text-amber-600">in progress</span></div>
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-gray-500"><i class="fas fa-future"></i></div><span class="text-sm">Multimodal AI & AI agents</span><span class="ml-auto text-xs">next ⏩</span></div>
            <div class="flex items-center gap-3 border-b border-gray-200 pb-2"><div class="status-icon text-gray-500"><i class="fas fa-chalkboard"></i></div><span class="text-sm">MLOps & Model Deployment at Scale</span><span class="ml-auto text-xs">next</span></div>
            <div class="flex items-center gap-3"><div class="status-icon text-gray-500"><i class="fas fa-language"></i></div><span class="text-sm">Multimodal AI — Vision + Language</span><span class="ml-auto text-xs">exploring</span></div>
          </div>
        </div>
      </div>

      <!-- ========= CERTIFICATIONS + CONNECT SECTION ========= -->
      <div class="flex flex-wrap gap-5 my-6">
        <div class="flex-1 bg-[#f3f6fc] rounded-2xl p-5">
          <div class="flex items-center gap-2 border-l-4 border-[#1f6e8c] pl-3 mb-3"><i class="fas fa-certificate"></i><span class="font-bold text-gray-800">CERTIFICATIONS</span></div>
          <div class="grid grid-cols-1 md:grid-cols-2 gap-2 text-sm">
            <div class="flex items-center gap-2"><i class="fas fa-check-circle text-[#1f6e8c] text-xs"></i><span>Machine Learning Specialization</span></div>
            <div class="flex items-center gap-2"><i class="fas fa-check-circle text-[#1f6e8c] text-xs"></i><span>IBM Data Science Professional</span></div>
            <div class="flex items-center gap-2"><i class="fas fa-check-circle text-[#1f6e8c] text-xs"></i><span>Python for Data Science & AI</span></div>
            <div class="flex items-center gap-2"><i class="fas fa-check-circle text-[#1f6e8c] text-xs"></i><span>Deep Learning Specialization</span></div>
            <div class="flex items-center gap-2"><i class="fab fa-google text-[#1f6e8c] text-xs"></i><span>Google Cloud ML Engineer</span></div>
            <div class="flex items-center gap-2"><i class="fas fa-microchip text-[#1f6e8c] text-xs"></i><span>TensorFlow Developer Certificate</span></div>
          </div>
        </div>
        <div class="flex-1 bg-[#eef3fa] rounded-2xl p-5 text-center">
          <div class="flex items-center gap-2 border-l-4 border-[#1f6e8c] pl-3 mb-3 justify-center lg:justify-start"><i class="fas fa-share-alt"></i><span class="font-bold text-gray-800">CONNECT WITH ME</span></div>
          <div class="flex justify-center gap-5 text-2xl text-[#2c3e66]">
            <a href="#" class="hover:text-[#0f5b86] transition transform hover:scale-110 inline-block"><i class="fab fa-linkedin"></i></a>
            <a href="#" class="hover:text-[#0f5b86] transition transform hover:scale-110 inline-block"><i class="fas fa-envelope"></i></a>
            <a href="#" class="hover:text-[#0f5b86] transition transform hover:scale-110 inline-block"><i class="fab fa-kaggle"></i></a>
            <a href="#" class="hover:text-[#0f5b86] transition transform hover:scale-110 inline-block"><i class="fas fa-robot"></i></a>
          </div>
          <div class="mt-3 text-xs text-[#366f8c]"><i class="fab fa-github"></i> github.com/srinivasu-ai</div>
        </div>
      </div>

      <!-- ========= QUOTE + CODE LOOP (fun element) ========= -->
      <div class="mt-5 bg-[#0a1927] text-[#bfd9e8] rounded-2xl py-4 px-6 flex flex-wrap justify-between items-center gap-3 font-mono">
        <div class="italic text-sm"><i class="fas fa-quote-left mr-2"></i> "The best way to predict the future is to build it."</div>
        <div class="bg-black/20 px-3 py-1.5 rounded-full text-xs"><i class="fas fa-code mr-1"></i> while(true) { eat(); sleep(); code(); repeat(); }</div>
      </div>

    
      <div class="flex justify-end gap-4 mt-4 text-[0.65rem] text-[#446688] font-medium">
        <span><i class="fas fa-chart-line"></i> 95%+ accuracy</span>
        <span><i class="fas fa-tachometer-alt"></i> 30 FPS on CPU</span>
        <span><i class="fas fa-chart-line"></i> 15% MAPE</span>
        <span><i class="fas fa-database"></i> 1M+ interactions</span>
      </div>
    </div>
  </div>
</body>
</html>
