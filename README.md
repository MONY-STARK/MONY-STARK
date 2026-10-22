<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Monish&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Machine%20Learning%20%7C%20Deep%20Learning%20%7C%20Generative%20AI&descAlignY=60&descSize=18" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=36BCF7&center=true&vCenter=true&width=700&lines=Developer+who+dreams+of+building+AGI;Building+real-time+AI+systems+end+to+end;Computer+Vision+%7C+NLP+%7C+Generative+AI;Turning+ideas+into+working+ML+solutions" alt="Typing SVG" />

<br/>

<img src="https://img.shields.io/github/followers/MONY-STARK?style=flat&logo=github&label=Followers" alt="Followers" />

</div>

---

## 👨‍💻 About Me

I'm a developer working in **Machine Learning** and **Deep Learning**, with the goal of helping people and organizations that need ML/DL solutions. My move into AI started from a love of science fiction and technology, and I now build the kind of systems I used to only watch in movies.

- 🧠 Strong grasp of ML & DL algorithms, backed by a **solid mathematical foundation**
- 🔬 I love building and experimenting with ideas, end to end
- 🎓 B.Tech in Chemical Engineering (2022) → Diploma in Artificial Intelligence (2024)
- 🎮 Outside code: anime, games, and music

---

## 🧰 Tech Stack

<div align="center">

| | |
|---|---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++_(basic)-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) |
| **ML / DL** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black) |
| **Backend & Data** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6446?style=flat-square) |
| **Tools & Cloud** | ![AWS SageMaker](https://img.shields.io/badge/AWS_SageMaker-FF9900?style=flat-square&logo=amazonaws&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square) ![llama.cpp](https://img.shields.io/badge/llama.cpp-444?style=flat-square) |

</div>

---

## 🚀 Featured Projects

### 🎙️ Real-Time Multilingual Voice Agent: Clinical Appointment Booking
A real-time voice AI agent that books clinical appointments in **English, Hindi, and Tamil**.

- **Pipeline:** Silero VAD → Faster-Whisper large-v3 (STT) → language detection → NLLB-200 translation → Qwen 2.5 7B (reasoning + tool calling) → TTS
- **Design decision:** non-English input is translated to English before LLM reasoning, since 7B models are unreliable at multilingual tool calling
- **Memory:** Redis for session state, PostgreSQL for persistent memory, APScheduler for scheduling
- **Infra:** FastAPI + WebSockets, fully containerized with Docker Compose, runs on a single consumer GPU (RTX 4060 8GB)

`FastAPI` `WebSockets` `Whisper` `NLLB-200` `Ollama` `Redis` `PostgreSQL` `Docker`

🔗 [Repository](https://github.com/MONY-STARK/real_time_voice_assistant)

---

### 🤖 Jarvis: Local AI Voice Assistant
A fully local, privacy-first voice assistant that runs inside an **8GB VRAM** budget.

- **LLM:** Qwen3-8B (Q4_K_M) served via llama.cpp built from source with CUDA, benchmarked against other open models to find the best fit for the hardware
- **Low latency:** sentence-level streaming through a **three-thread producer-consumer pipeline** (LLM tokens → sentence buffer → TTS worker → playback worker)
- **Long-term memory:** ChromaDB-backed RAG plus a `save_memory` tool, with trimmed message history
- **Tool calling:** OpenAI-style tool schemas, a tool registry, and `<think>` block stripping for reasoning models
- **TTS research:** evaluated Kokoro, CosyVoice2, Chatterbox, and Fish Speech on latency vs quality trade-offs

`llama.cpp` `Qwen3` `ChromaDB` `RAG` `Tool Calling` `Python Threading` `TTS`

---

### 🧮 Stepwise DPO: Step-Level Rewards from a Generative Reward Model
An extension of Direct Preference Optimization that scores **each reasoning step** instead of whole responses.

- Used **Zephyr-7B** as a Generative Reward Model (GenRM) to score reasoning steps on **PRM800K**
- Reformatted PRM800K into `prompt / chosen / rejected` with per-step score columns
- Subclassed Hugging Face's `DPOTrainer` into a custom **`StepwiseDPOTrainer`**: handles variable-length step-score padding/collation and aggregates step rewards into the DPO loss

`PyTorch` `TRL` `DPO` `Reward Modeling` `LLM Alignment`

---

### 🐄 Real-Time Livestock Monitoring System *(Internship)*
Built a real-time monitoring system using **Deep Learning and Computer Vision** to track livestock from video feeds.

`Computer Vision` `Deep Learning` `Real-Time Inference`

---

## 🎯 Currently

- 🔭 Pushing Myself to build something great!!
- 🌱 Sharpening system design and clean OOP/SOLID code

---

## 📊 GitHub Stats

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=MONY-STARK&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MONY-STARK&layout=compact&theme=tokyonight&hide_border=true" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=MONY-STARK&theme=tokyonight&hide_border=true" />

</div>

---

## 🤝 Let's Connect

<div align="center">

<!-- Replace the links below with your own -->
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/monish-prasad-5724212b3)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:YOUR-EMAIL)

*I'm open to opportunities where ML/DL can make a real difference.*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" width="100%"/>

</div>
