<h1 align="center">👋 Hi, I'm Muhammad Awais</h1>

<h3 align="center">🤖 AI Engineer &nbsp;|&nbsp; 🌐 Full-Stack Developer &nbsp;|&nbsp; 🔬 Aspiring AI Researcher</h3>

<p align="center">
  Computer vision · Generative AI · Agentic AI · RAG<br/>
  <b>Open to AI / full-stack engineering roles and MS (AI/CS) research opportunities</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/muhammad-awais32013">
    <img src="https://img.shields.io/badge/LinkedIn-%2300A0DC.svg?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" height="28"/>
  </a>
  <a href="mailto:dev.muhammadowais@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" alt="Email" height="28"/>
  </a>
  <a href="https://muhammad-awais-swe.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white" alt="Portfolio" height="28"/>
  </a>
  <a href="https://huggingface.co/AlphaCoder32">
    <img src="https://img.shields.io/badge/Hugging%20Face-%23FFD44A.svg?style=flat&logo=huggingface&logoColor=black" alt="Hugging Face" height="28"/>
  </a>
  <a href="https://www.kaggle.com/muhammadawaisqrni">
    <img src="https://img.shields.io/badge/Kaggle-%2320BEFF.svg?style=flat&logo=kaggle&logoColor=white" alt="Kaggle" height="28"/>
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=MuhammadAwais-32013" alt="Profile views"/>
</p>

---

## 👨‍💻 About Me

I'm a Computer Science graduate (B.S., NUML Islamabad, CGPA 3.34/4.00) who builds and evaluates AI systems that have to work reliably outside the lab: a real-time traffic perception system (YOLOv8 + multi-object tracking), RAG pipelines, and multi-agent LLM workflows, all shipped end to end with React/Next.js frontends and FastAPI backends.

I'm interested in **measuring whether AI systems can be trusted**: how detection errors propagate into decisions, and when vision-language models and LLM agents can complement purpose-built pipelines in low-resource, heterogeneous settings.

**Currently**
- 🎓 Applying for an **M.S. in Artificial Intelligence / Computer Science** (research-focused, scholarship-seeking)
- 💼 Open to **AI Engineer / Full-Stack / GenAI Developer** roles (remote or on-site)
- 🛠️ Working on formal groundedness and hallucination evaluation for my RAG health assistant (vs. a no-retrieval baseline)

---

## 🔬 Research Interests




| | Focus |
|---|---|
| **Computer vision and multimodal learning** | Object detection and tracking, video analytics, vision-language models, open-vocabulary scene understanding. |
| **Intelligent transportation and embodied AI** | Perception for traffic monitoring and autonomous systems; real-time, edge-deployable AI. |
| **LLM systems and agentic AI** |  Retrieval-augmented generation, LLM agents and multi-agent systems, evaluation of LLM systems.|
| **Trustworthy and applied AI** |  Reliability and error analysis, generative AI applications, AI for healthcare, machine learning for forecasting. |

---

## 🚀 Featured Projects

### 🚦 Real-Time Traffic Choking Point Detector *(Final Year Project)*
`YOLOv8` `ByteTrack` `OpenCV` `FastAPI` `React`

A real-time congestion monitoring system for two Islamabad junctions (NUML Gate, 7-Up Chowk). I was the AI engineer in a team of three, owning the pipeline from data collection and annotation through training, evaluation and web integration.

- **Data:** self-collected four-class dataset (Controller, Human, NUML bus, vehicle): 1,642 images, 6,612 labelled objects, 80/10/10 split
- **Model:** fine-tuned YOLOv8n (3.0M params, 6.3 MB) for 282 epochs (best epoch 232, ~2.7 h on a cloud GPU) + ByteTrack for persistent IDs and count-based congestion rules
- **Serving:** alerts delivered via a FastAPI backend to a React monitoring dashboard and SMS

| Split | mAP@50 | mAP@50–95 | Precision | Recall |
|---|---|---|---|---|
| Validation | 89.5% | 59.3% | 86.4% | 84.7% |
| Held-out test (162 images, 799 instances) | 89.1% | 54.8% | 82.2% | 86.8% |

Inference runs at **3.1–5.7 ms/image** on a Tesla T4. Error analysis shows mistakes are mostly background false positives rather than class mix-ups; *Human* is the weakest class (test mAP@50 76.6%).

🔗 [Dataset](https://REPLACE-DATASET-LINK) · [Training notebook](https://REPLACE-NOTEBOOK-LINK) · [Code](https://github.com/MuhammadAwais-32013/REPLACE-REPO)

---

### 🩺 DiaBP Diet Consultant: RAG-Powered Health Assistant
`FastAPI` `Gemini` `FAISS` `Sentence Transformers` `Next.js` `Flutter` `Docker`

Full-stack assistant for diabetes and hypertension patients. A retrieval-augmented pipeline grounds a WebSocket chatbot and personalised multi-week diet plans in medical literature. Includes OCR for uploaded medical documents, authentication, health tracking, an admin dashboard, and a GitHub Actions workflow for Azure deployment.

🧪 *In progress: groundedness and hallucination evaluation against a no-retrieval baseline.*

🔗 [GitHub](https://github.com/MuhammadAwais-32013/REPLACE-DIABP-REPO)

---

### 🎙️ Podcaster Crew: Multi-Agent LLM Pipeline
`CrewAI` `Gemini` `Tool calling` `Speech synthesis`

Role-specialised agents (researcher, reporting analyst, scriptwriter) use web-search tools to turn a topic into a scripted audio podcast via Gemini speech synthesis. Planned: comparison with a single-prompt baseline on citation correctness and unsupported claims.

🔗 [GitHub](https://github.com/MuhammadAwais-32013/REPLACE-PODCASTER-REPO)

---

### ✍️ Multi-Agent Content Generation System
`CrewAI` `Gemini` `LiteLLM` `Python`

Planner, Writer and Editor agents collaborate to turn a topic into a polished, SEO-optimised blog article, with explicit roles, goals and task-level expected outputs.

🔗 [GitHub](https://github.com/MuhammadAwais-32013/REPLACE-CONTENT-AGENTS-REPO)

---

### 📰 ArticleSift: LLM News Q&A
`LLaMA 3.1` `Google Custom Search API` `Streamlit` `gTTS`

Retrieves and analyses live news for question answering and summarisation. Five API endpoints, audio narration, and translation into Urdu, English, Spanish and French.

🔗 [GitHub](https://github.com/MuhammadAwais-32013/REPLACE-ARTICLESIFT-REPO)

---

### 📈 Sales Demand Forecasting with XGBoost
`XGBoost` `Scikit-learn` `Pandas` `NumPy` `Matplotlib` `Seaborn`

End-to-end forecasting pipeline with lag, rolling-window (4-period mean/std) and calendar features. **R² = 0.92** on a held-out test set (train R² = 0.97).

🔗 [GitHub](https://github.com/MuhammadAwais-32013/REPLACE-FORECASTING-REPO)

---

### 🗣️ Voice-to-Voice Chatbot
Live demo of a voice-in, voice-out conversational app deployed on Hugging Face Spaces.

🔗 [Try it](https://huggingface.co/spaces/AlphaCoder32/voice_to_voice_chatBot)

---

## 💼 Experience

**Software Engineering Intern (Full Stack)** · National Incubation Center (NIC), Islamabad · *Jan 2026 – Mar 2026*
- Contributed to a tourism platform ([stayOvers.pk](https://stayovers.pk)) with AI-assisted booking workflows and role-based access control for guest, host and admin users
- Modular OOP backend, Git branching, Postman API test suites; Agile sprints and daily stand-ups

**Freelance Software Developer** · Fiverr, remote (international clients) · *May 2024 – Aug 2025*
- Delivered full-stack apps (React, Next.js, Python) with payment and authentication APIs; deployed on Vercel and Netlify

**A-Level Tutor (Hybrid)** · Private tutoring · *May 2024 – Apr 2026*
- Taught A-Level students online and in person, moving from theory to practical application

---

## 🎓 Education

**B.S. in Computer Science**, National University of Modern Languages (NUML), Islamabad · *2022 – 2026* · CGPA 3.34 / 4.00
- Coursework highlights: Artificial Intelligence (A), Data Structures & Algorithms (A+), Design & Analysis of Algorithms (A), Probability & Statistics (A+), Computer Graphics (A)
- Final Year Project (FYP-I & FYP-II): **A** in both

---

## 💡 Tech Stack

### 🧠 Generative & Agentic AI
![CrewAI](https://img.shields.io/badge/CrewAI-FF5A50?style=flat)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=flat&logo=openai&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-%239B4F96.svg?style=flat&logo=groq&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-%23FFD44A.svg?style=flat&logo=huggingface&logoColor=black)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat&logo=meta&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-%23FF4B4B.svg?style=flat&logo=streamlit&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-F97316?style=flat)

### 👁️ ML & Computer Vision
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat&logoColor=black)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-017CEE?style=flat)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)

### 🌐 Full-Stack
![React](https://img.shields.io/badge/React-%2361DAFB.svg?style=flat&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-%23000000.svg?style=flat&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-%2338B2AC.svg?style=flat&logo=tailwind-css&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-%231572B6.svg?style=flat&logo=css3&logoColor=white)

### 🧩 Languages & Databases
![Python](https://img.shields.io/badge/Python-%233776AB.svg?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-%23007ACC.svg?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=flat&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C%2B%2B-%2300599C.svg?style=flat&logo=c%2B%2B&logoColor=white)
![Java](https://img.shields.io/badge/Java-%23007396.svg?style=flat&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)

### ☁️ Cloud & DevOps
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-%23F05032.svg?style=flat&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-%23000000.svg?style=flat&logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-%2300C7B7.svg?style=flat&logo=netlify&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-%2320BEFF.svg?style=flat&logo=kaggle&logoColor=white)
![Colab](https://img.shields.io/badge/Colab-%23F9AB00.svg?style=flat&logo=googlecolab&logoColor=white)

---

## 🏆 Honors & Certifications

**Honors**
- 🥉 8th place, national-level Generative AI Hackathon (remote), Pakistan
- Participant in three international online hackathons

**Certifications**
- Machine Learning Specialization: Stanford Online / DeepLearning.AI (Coursera)
- Computer Vision: YOLO Custom Object Detection (Coursera)
- Agentic AI Level 2 Engineer (Panaversity / PIAIC)
- Generative AI Application Developer (Pak Angels, Silicon Valley, CA)
- MCP Automation in Production (Hugging Face) · PCAP: Python Essentials (Cisco) · Generative AI: Prompt Engineering (IBM) · SQL (DataCamp) · Postman API Fundamentals Expert

**Community & Events**
- Campus Outreach Deputy Head & Technology/AI Lead, **CareCascade**: delivered three in-person AI/tech sessions to ~250–300 students
- Team member (Job Fair pavilion), Indus AI Week 2026, Islamabad
- Attendee: ICECT 2025 (NUML) · AI Summit 2023, Islamabad

---

## 📊 GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=MuhammadAwais-32013&theme=tokyonight&hide_border=true&include_all_commits=false&count_private=false" alt="GitHub stats"/>
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MuhammadAwais-32013&theme=tokyonight&hide_border=true&layout=compact" alt="Top languages"/>
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com/?user=MuhammadAwais-32013&theme=tokyonight&hide_border=true" alt="GitHub streak"/>
</p>

---

## 📫 Let's Connect

I'm happy to discuss research collaborations, supervision opportunities, or engineering roles.

📧 [dev.muhammadowais@gmail.com](mailto:dev.muhammadowais@gmail.com) · 💼 [LinkedIn](https://www.linkedin.com/in/muhammad-awais32013) · 🌐 [Portfolio](https://muhammad-awais-swe.vercel.app/) · 📊 [Kaggle](https://www.kaggle.com/muhammadawaisqrni)
