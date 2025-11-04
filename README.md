# 👩‍💻 JURISTO.ai – AI Chatbot for Women Safety  

**JURISTO.ai** is an **AI-powered legal and safety assistance chatbot** designed to support **women’s safety, legal awareness, and empowerment**.  
It leverages **Natural Language Processing (NLP)**, **Machine Learning (ML)**, and **Transformer models (FLAN-T5, SentenceTransformers)** to provide **real-time support, verified legal guidance, and emergency information**.  

This project demonstrates advanced skills in **AI for Social Good**, **data curation**, and **LLM-based conversational systems**.  

---

## Problem Statement  

In India, women often face challenges in accessing immediate help, understanding legal rights, or filing harassment complaints due to lack of awareness or slow manual processes.  
**JURISTO.ai** bridges this gap through an AI-driven chatbot that:  
- Detects distress or safety-related keywords  
- Provides factual, empathetic, and contextual responses  
- Connects users to verified helplines and resources  
- Educates women about legal rights and safety laws  

---

## Objectives  

- Deliver **real-time legal and emergency assistance** through chat.  
- Integrate **AI + NLP models** for context understanding and intelligent response generation.  
- Build a **verified knowledge base** of Indian women’s laws and helplines.  
- Promote **AI for Social Good** by ensuring accessibility, awareness, and trust.  

---

## Tech Stack  

| Category | Tools / Frameworks |
|-----------|--------------------|
| **Programming Language** | Python |
| **AI / NLP Models** | FLAN-T5, SentenceTransformers (MiniLM) |
| **Machine Learning Libraries** | Scikit-learn, Transformers, Torch |
| **Vector Database** | FAISS |
| **Frameworks** | LangChain |
| **Text Preprocessing** | NLTK, spaCy |
| **Backend / Deployment** | Flask / FastAPI / Streamlit |
| **Storage** | JSON-based knowledge base |
| **Environment** | Google Colab / Jupyter Notebook |

---
###  Dataset Summary  

| Attribute | Description |
|------------|-------------|
| **File Name** | `women_dataset.json` |
| **Entries** | ~1,500–2,000 |
| **Format** | JSON |
| **Language** | English |
| **Categories** | Legal Rights, Helplines, Acts, Complaint Process, Safety Tips |
| **Embedding Model** | SentenceTransformers (MiniLM) |
| **Use Case** | Semantic Retrieval + Contextual Response Generation |

---

## Dataset Details  

The **`women_dataset.json`** file is a **manually created knowledge base** that powers JURISTO.ai’s legal and safety responses.  
It contains verified data collected from **official government and legal sources** related to **women’s safety, rights, and protection laws** in India.  

---

### Source of Data  
- **Government of India** and **National Commission for Women (NCW)** resources ([ncw.nic.in](https://ncw.nic.in))  
- Legal Acts:  
  - *National Commission for Women Act, 1990*  
  - *POSH Act, 2013*  
  - *Protection of Women from Domestic Violence Act, 2005*  
  - *IPC Sections* (354, 498A, 509)  
- Awareness Materials: complaint filing, online safety, helpline numbers (1091, 181, 100)

---

### Manual Data Creation Process  

1. **Data Collection:** Extracted information from verified PDFs, legal portals, and NCW website.  
2. **Cleaning:** Removed noise, HTML tags, and redundant content.  
3. **Structuring:** Created JSON format entries:  
   ```json
   {
     "category": "Legal Rights",
     "title": "POSH Act, 2013",
     "content": "The Sexual Harassment of Women at Workplace Act provides protection and redressal mechanisms..."
   }

---

## Dataset Overview  

### Preprocessing  
Used **spaCy** and **NLTK** for tokenization, lemmatization, and stopword removal.  

### Semantic Chunking  
Split long texts into smaller (200–300 word) contextual chunks.  

### Embedding  
Encoded using **`sentence-transformers/all-MiniLM-L6-v2`**.  

### Storage  
Indexed embeddings in **FAISS** for fast semantic retrieval.

---

User Query → Embedding (MiniLM) → Semantic Search (FAISS) → Context (Top 3 Chunks) → Response Generation (FLAN-T5) → Output (JURISTO.ai Chatbot)

--

## Key Achievements  

- **Built a dual-mode chatbot** (Retrieval + Generative AI) for contextual and empathetic responses.  
- **Created a manually verified dataset** using authentic government and NCW sources.  
- Achieved **high contextual accuracy** through FAISS-based semantic retrieval.  
- Implemented **Transformer-based empathy generation** using FLAN-T5.  
- Designed a **modular and scalable NLP pipeline** for real-world deployment.  

---

## Future Enhancements  

- Integrate **speech-to-text** capability for voice-based SOS commands.  
- Add **real-time GPS tracking** and automated emergency alerts.  
- Extend support for **regional Indian languages** (Hindi, Marathi, Tamil, etc.).  
- Build an **interactive dashboard** for law awareness and complaint tracking.  
- Deploy a **live demo** on Hugging Face Spaces or Streamlit for public access.  
