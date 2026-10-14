# Hi, I'm Bhaskar Chari 👋

**AI/ML Engineer & Researcher** · Junior Research Fellow at DRDO R&DE(E)

I build intelligent systems for real-world problems, with a focus on **Generative AI, RAG, Computer Vision and NLP**. I like problems where the evaluation matters as much as the model.

[![Portfolio](https://img.shields.io/badge/Portfolio-deadbott--exe.github.io-0B0D0F?style=flat)](https://deadbott-exe.github.io/Portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-bhaskar--chari-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/bhaskar-chari)
[![Email](https://img.shields.io/badge/Email-charibhaskar2608%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:charibhaskar2608@gmail.com)
[![IEEE](https://img.shields.io/badge/IEEE-Published-00629B?style=flat)](https://ieeexplore.ieee.org/document/11502364)

---

## 🔭 What I'm working on

- **Now:** Junior Research Fellow at DRDO's Research & Development Establishment (Engineers) since Aug 2026. Project details are under NDA.
- **Focus areas:** validation-first RAG systems, hybrid rule-based + LLM pipelines, pose-based computer vision.

## 🚀 Projects

### [DocuMind AI](https://github.com/DeadBoTt-exe/DocuMind-AI)
A validation-first RAG system for querying large engineering documentation, designed like an internal enterprise docs assistant.

- Pipeline: PDF ingestion → cleaning and chunking with page-level metadata → `all-mpnet-base-v2` embeddings → Qdrant (HNSW) → Gemini generation
- **Grounding validation:** a second Gemini pass (temperature 0) rejects answers not supported by retrieved context, and fails closed if the validator is unavailable
- **Confidence score:** `0.7 × retrieval + 0.3 × coverage`
- Chose RAG over fine-tuning so the knowledge base can change without retraining
- FastAPI service, circuit breaker around the validator, observability and Pydantic schema validation

`Python` `FastAPI` `Qdrant` `Gemini` `Sentence Transformers` `Docker`

### SentimentR
A hybrid sentiment analysis framework: a fast rule-based core that routes only ambiguous, sarcastic or culturally marked text to a fine-tuned LLM. Published at IEEE CSNT 2026 (see below).

`NLP` `LLMs` `Prompt Engineering`

### [TarangAI](https://github.com/DeadBoTt-exe/TarangAI)
Team project on Indian classical dance. MediaPipe extracts body pose and 21-point hand landmarks, and deep learning models classify dance style and mudras. The repository is a fork of [Aanandvyas/TarangAI](https://github.com/Aanandvyas/TarangAI). My part: data gathering, dataset preparation and model training.

`MediaPipe` `OpenCV` `PyTorch` `Computer Vision`

---

## 📄 Research

**Cultural and Sarcastic Context Aware Sentimental Analysis with Large Language Model and Rule Based Heuristics: An Empirical Study**
IEEE CSNT 2026 · Al-Khobar, Saudi Arabia · DOI [10.1109/CSNT69054.2026.11502364](https://ieeexplore.ieee.org/document/11502364)

Co-authored with Umair Ullah, Hardik Rawat, Jay Vivek Yadav and Yuvraj Singh (VIT Bhopal). My part: data gathering, preprocessing and prompt engineering.

| Model (SARC, sarcasm-heavy) | Accuracy | F1 |
| --------------------------- | -------- | ---- |
| VADER                       | 0.52     | 0.51 |
| BERT                        | 0.78     | 0.77 |
| **SentimentR**              | **0.91** | **0.90** |

Ablation: removing the rule-based core gives similar accuracy (0.90) but latency jumps from **45 ms to 850 ms** on average.

---

## 🛠 Tech stack

| Area | Tools |
| ---- | ----- |
| Languages | Python |
| ML frameworks | PyTorch, TensorFlow, Keras, Scikit-learn |
| NLP & GenAI | LLMs, RAG, Embeddings, Hugging Face, NLTK |
| Vision & data | OpenCV, MediaPipe, Pandas, NumPy |
| Vector search & DB | Qdrant, MySQL |
| Engineering | FastAPI, Docker, Git, GitHub, PowerBI, PyQt5 |

## 🎓 Education & highlights

- **B.Tech, CSE (AI & ML)**, Vellore Institute of Technology, 2022–2026 · CGPA 8.49/10
- Space Lab Technical Intern, India Space Lab (Dec 2024 – Jan 2025)
- National finalist, Health Hackathon
- Lead, Vitronix Club (technical and non-technical events)
- Smart India Hackathon participant
- Spoken languages: English, Hindi, Telugu, Marathi

## 📫 Get in touch

- Portfolio: [deadbott-exe.github.io/Portfolio](https://deadbott-exe.github.io/Portfolio/)
- Resume: [PDF](https://deadbott-exe.github.io/Portfolio/BhaskarChari_AIMLEngineer_Resume.pdf)
- LinkedIn: [linkedin.com/in/bhaskar-chari](https://linkedin.com/in/bhaskar-chari)
- Email: charibhaskar2608@gmail.com
