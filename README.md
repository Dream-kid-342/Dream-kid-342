<div align="center">

<!-- HEADER BANNER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a2332,100:21263a&height=220&section=header&text=Enock%20Mumo&fontSize=64&fontColor=4fc3f7&fontAlignY=40&fontFamily=JetBrains+Mono&desc=AI%20Engineer%20%E2%80%94%20Systems%20Architect%20%E2%80%94%20Kenya&descAlignY=60&descSize=17&descColor=90caf9" width="100%"/>

<br/>

<!-- TYPING ANIMATION -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=22&duration=3200&pause=1200&color=4FC3F7&center=true&vCenter=true&multiline=false&repeat=true&width=760&height=55&lines=Building+complete+AI+systems%2C+not+just+models.;Input+%E2%86%92+Model+%E2%86%92+Processing+%E2%86%92+Output+%E2%86%92+UI.;ML+%2B+Backend+%2B+Frontend+%E2%80%94+one+engineer.;From+raw+data+to+deployed+intelligence.)](https://git.io/typing-svg)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=Dream-kid-342&color=4fc3f7&style=flat-square&label=profile+views)
&nbsp;
[![GitHub followers](https://img.shields.io/github/followers/Dream-kid-342?color=4fc3f7&style=flat-square&logo=github&label=followers)](https://github.com/Dream-kid-342)

</div>

<br/>

---

<div align="center">

<h1><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=30&duration=1&pause=999999&color=4FC3F7&center=true&vCenter=true&width=300&height=48&lines=%3E+whoami" alt="> whoami"/></h1>

</div>

```python
class AIEngineer:
    name        : str  = "Enock Mumo"
    location    : str  = "Nairobi, Kenya"
    role        : str  = "AI Engineer  |  Systems Architect"
    background  : str  = "Transitioned from MERN stack into full AI engineering"
    focus       : list = [
        "End-to-End AI Pipelines",
        "Computer Vision  —  Floor Plan Intelligence",
        "RAG Systems with Local LLMs",
        "Custom Transformer Architectures",
        "FastAPI  x  React  x  Mobile Integration",
    ]
    philosophy  : str  = "I don't just train models — I build systems that think."

    def build(self, problem: str) -> str:
        return f"Input({problem}) -> Model() -> Processing() -> Output() -> UI()"
```

<br/>

---

<div align="center">

<h1><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=30&duration=1&pause=999999&color=4FC3F7&center=true&vCenter=true&width=480&height=48&lines=Engineering+Philosophy" alt="Engineering Philosophy"/></h1>

<br/>

<h3><em>"A model alone is not a product.<br/>A system that ingests, reasons, and delivers — that is engineering."</em></h3>

<br/>

<p>I design and ship AI systems where every layer is intentional. Raw data pipelines feed battle-tested ML models, results surface through clean APIs, and users interact through polished interfaces. The gap between a Jupyter notebook and a real-world AI system is exactly where I operate — and where I thrive.</p>

</div>

<br/>

---

<div align="center">

<h1><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=30&duration=1&pause=999999&color=4FC3F7&center=true&vCenter=true&width=420&height=48&lines=Featured+Projects" alt="Featured Projects"/></h1>

<br/><br/>

---

<h2>Floor Plan Intelligence System</h2>

<br/>

<p>Architects and engineers produce thousands of floor plan drawings that exist as raw images — unstructured, unsearchable, and disconnected from modern Building Information Modeling pipelines. Manually extracting spatial data such as rooms, doors, windows, and walls is expensive, slow, and deeply error-prone. This system eliminates that bottleneck entirely.</p>

<br/>

<p>The pipeline ingests raw floor plan images from the CubiCasa5K dataset — over 5,000 professionally annotated architectural drawings — and passes them through the FloorTrans model, a transformer-based segmentation architecture designed specifically for the structured geometric complexity of architectural drawings. Unlike traditional CNNs, FloorTrans preserves spatial relationships across walls, corridors, and rooms, making segmentation far more accurate at scale.</p>

<br/>

<p>Output is emitted as structured JSON encoded with room polygons, connectivity graphs, and element classifications — fully compatible with IFC (Industry Foundation Classes) for direct BIM ingestion. A Matplotlib visualization layer renders labeled overlays on top of the original image, and a cross-platform Tkinter desktop GUI gives non-technical architects the ability to run inference locally with zero command-line exposure.</p>

<br/>

<p><strong>Stack —</strong> Python · PyTorch · FloorTrans · CubiCasa5K · OpenCV · PIL · Matplotlib · Tkinter · JSON/SVG</p>

<br/><br/>

---

<h2>RAG System — Retrieval-Augmented Generation</h2>

<br/>

<p>Standard large language models hallucinate. They have knowledge cutoffs. They cannot reason over private documents. RAG solves all three simultaneously: by grounding generation in retrieved, verified context from your own data, responses become accurate, auditable, and domain-specific — without sending a single byte to an external server.</p>

<br/>

<p>This system is built with LangChain as the orchestration layer and Ollama to run large language models fully offline — Llama 3, Mistral, and Phi-3 depending on the task. Documents in PDF, Markdown, or plain text are chunked using a recursive semantic splitter, embedded with nomic-embed-text running locally via Ollama, and stored in a persistent FAISS or ChromaDB vector index on disk.</p>

<br/>

<p>At query time, the user's question is embedded and compared against the vector index using cosine similarity. Top-K candidate chunks are retrieved, re-ranked using a cross-encoder to eliminate noise, and injected into the prompt context before the local LLM generates its grounded response. The entire loop — from query to answer — runs on a single machine with zero internet dependency.</p>

<br/>

<p>A FastAPI backend exposes streaming endpoints so the frontend receives tokens in real time, matching the feel of cloud-hosted systems while remaining completely private. This architecture is production-deployable for enterprise knowledge bases, legal document Q&A, offline medical reference, and secure government document processing.</p>

<br/>

<p><strong>Stack —</strong> Python · LangChain · Ollama · FAISS · ChromaDB · FastAPI · nomic-embed-text · Llama 3 · Mistral</p>

<br/><br/>

---

<h2>Custom GPT — Transformer from Scratch</h2>

<br/>

<p>The only way to truly engineer on top of large language models is to understand what happens inside them at every layer. This project implements a decoder-only transformer — the GPT architecture — from scratch using pure PyTorch, with no Hugging Face wrappers, no shortcuts, and no abstraction hiding the mechanics.</p>

<br/>

<p>The implementation covers a custom BPE tokenizer trained on the target corpus, multi-head causal self-attention with masking, GELU-activated feed-forward blocks, residual connections, layer normalization, and a full language model head for next-token prediction. The training loop includes cosine learning rate scheduling with linear warmup, mixed-precision training via PyTorch AMP, and gradient checkpointing for memory efficiency on constrained hardware.</p>

<br/>

<p>Text generation supports temperature scaling, top-k sampling, and nucleus (top-p) sampling — giving precise control over creativity versus coherence. Every component is hand-implemented and documented so the architecture is fully auditable and extensible for fine-tuning, distillation, and domain adaptation experiments.</p>

<br/>

<p><strong>Stack —</strong> Python · PyTorch · Custom BPE Tokenizer · Mixed Precision AMP · Cosine LR Scheduler</p>

<br/><br/>

---

<h2>AI Pipeline System</h2>

<br/>

<p>A production-grade inference system that connects trained PyTorch models to a live API backend and multiple client surfaces — React web, Flutter mobile, and React Native — through a single unified FastAPI server. This is where ML engineering meets software engineering at full scale.</p>

<br/>

<p>The FastAPI server loads the model once at startup via dependency injection, exposing async endpoints validated by Pydantic schemas. Long-running inference jobs are offloaded to a background task queue so the API remains non-blocking under load. WebSocket support enables real-time streaming predictions to connected clients, delivering token-by-token or frame-by-frame output without polling overhead.</p>

<br/>

<p>The React frontend displays live inference feedback with a clean interface, Flutter handles on-device UI with native performance, and the whole stack is containerized with Docker for reproducible, portable deployment across any environment.</p>

<br/>

<p><strong>Stack —</strong> Python · PyTorch · FastAPI · Pydantic · WebSockets · React · Flutter · React Native · Docker</p>

</div>

<br/>

---

<div align="center">

<h1><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=30&duration=1&pause=999999&color=4FC3F7&center=true&vCenter=true&width=280&height=48&lines=Tech+Stack" alt="Tech Stack"/></h1>

<br/>

**Machine Learning & AI**

<p>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" width="46" title="Python"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pytorch/pytorch-original.svg" width="46" title="PyTorch"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/numpy/numpy-original.svg" width="46" title="NumPy"/>&nbsp;&nbsp;
  <img src="https://upload.wikimedia.org/wikipedia/commons/3/32/OpenCV_Logo_with_text_svg_version.svg" width="46" title="OpenCV"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/matplotlib/matplotlib-original.svg" width="46" title="Matplotlib"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/scikitlearn/scikitlearn-original.svg" width="46" title="Scikit-Learn"/>
</p>

<br/>

**LLM & RAG**

<p>
  <img src="https://avatars.githubusercontent.com/u/126733545?s=200&v=4" width="46" title="LangChain"/>&nbsp;&nbsp;
  <img src="https://ollama.ai/public/ollama.png" width="46" title="Ollama"/>
</p>

<br/>

**Backend & APIs**

<p>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fastapi/fastapi-original.svg" width="46" title="FastAPI"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" width="46" title="Node.js"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original.svg" width="46" title="Express"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg" width="46" title="Docker"/>
</p>

<br/>

**Databases**

<p>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg" width="46" title="MongoDB"/>&nbsp;&nbsp;
  <img src="https://seeklogo.com/images/S/supabase-logo-DCC676FFE2-seeklogo.com.png" width="46" title="Supabase"/>&nbsp;&nbsp;
  <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" width="46" title="Firebase"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg" width="46" title="PostgreSQL"/>
</p>

<br/>

**Mobile**

<p>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/flutter/flutter-original.svg" width="46" title="Flutter"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" width="46" title="React Native"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/kotlin/kotlin-original.svg" width="46" title="Kotlin"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original.svg" width="46" title="Android"/>
</p>

<br/>

**Frontend**

<p>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" width="46" title="React"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" width="46" title="TypeScript"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" width="46" title="JavaScript"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg" width="46" title="HTML5"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg" width="46" title="CSS3"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/tailwindcss/tailwindcss-original.svg" width="46" title="Tailwind CSS"/>
</p>

<br/>

**Tools**

<p>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" width="46" title="Git"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/github/github-original.svg" width="46" title="GitHub"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" width="46" title="Linux"/>&nbsp;&nbsp;
  <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" width="46" title="Postman"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/jupyter/jupyter-original.svg" width="46" title="Jupyter"/>&nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pycharm/pycharm-original.svg" width="46" title="PyCharm"/>
</p>

</div>

<br/>

---

<div align="center">

<h1><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=30&duration=1&pause=999999&color=4FC3F7&center=true&vCenter=true&width=340&height=48&lines=GitHub+Analytics" alt="GitHub Analytics"/></h1>

<br/>

<img height="175em" src="https://github-readme-stats.vercel.app/api?username=Dream-kid-342&show_icons=true&theme=github_dark&include_all_commits=true&count_private=true&border_color=4fc3f7&icon_color=4fc3f7&title_color=4fc3f7&hide_border=false&card_width=400" alt="Enock GitHub Stats"/>
&nbsp;&nbsp;
<img height="175em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Dream-kid-342&layout=compact&langs_count=8&theme=github_dark&border_color=4fc3f7&title_color=4fc3f7&hide_border=false&card_width=400" alt="Top Languages"/>

<br/><br/>

<img width="100%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Dream-kid-342&theme=github_dark"/>

<br/>

<img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Dream-kid-342&theme=github_dark"/>
&nbsp;
<img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Dream-kid-342&theme=github_dark"/>

<br/><br/>

[![GitHub Streak](https://streak-stats.demolab.com?user=Dream-kid-342&theme=github-dark-blue&border=4fc3f7&ring=4fc3f7&fire=ef5350&currStreakLabel=4fc3f7&sideLabels=90caf9&dates=90caf9)](https://git.io/streak-stats)

<br/><br/>

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=Dream-kid-342&bg_color=0d1117&color=4fc3f7&line=4fc3f7&point=ffffff&area=true&area_color=1a2332&hide_border=false&border_color=4fc3f7)](https://github.com/ashutosh00710/github-readme-activity-graph)

<br/><br/>

<img src="https://ghchart.rshah.org/4fc3f7/Dream-kid-342" alt="Contribution Chart" width="100%"/>

</div>

<br/>

---

<div align="center">

<h1><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=30&duration=1&pause=999999&color=4FC3F7&center=true&vCenter=true&width=340&height=48&lines=Current+Focus" alt="Current Focus"/></h1>

</div>

```bash
# enock@nairobi:~$ cat current_objectives.log

[DONE]  Floor Plan Intelligence System    — v1 shipped, BIM export in progress
[WIP ]  RAG System                        — hybrid search + cross-encoder re-ranking
[WIP ]  Custom GPT                        — scaling architecture, tokenizer improvements
[NEXT]  Multi-modal AI Pipeline           — vision + language unified system
[NEXT]  AI-powered Mobile App             — Flutter + on-device inference
```

<br/>

---

<div align="center">

<h1><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=30&duration=1&pause=999999&color=4FC3F7&center=true&vCenter=true&width=240&height=48&lines=Connect" alt="Connect"/></h1>

<br/>

<a href="mailto:Dream-kid-342@email.com">
  <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"/>
</a>
&nbsp;
<a href="https://twitter.com/Dream-kid-342">
  <img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X"/>
</a>
&nbsp;
<a href="https://linkedin.com/in/Dream-kid-342">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>
&nbsp;
<a href="https://Dream-kid-342.dev">
  <img src="https://img.shields.io/badge/Portfolio-4FC3F7?style=for-the-badge&logo=vercel&logoColor=black" alt="Portfolio"/>
</a>
&nbsp;
<a href="https://github.com/Dream-kid-342">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>

<br/><br/>

---

<br/>

[![Footer Quote](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=15&duration=4000&pause=2000&color=90CAF9&center=true&vCenter=true&multiline=false&repeat=true&width=760&height=36&lines=The+future+belongs+to+engineers+who+build+systems+that+learn%2C+adapt%2C+and+deliver.;Not+just+models+that+predict+%E2%80%94+but+systems+that+think.;Building+intelligent+systems+from+Nairobi%2C+Kenya.)](https://git.io/typing-svg)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:21263a,50:1a2332,100:0d1117&height=130&section=footer" width="100%"/>

</div>
