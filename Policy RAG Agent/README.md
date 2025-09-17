# 🧠 MoF Policy RAG Agent

A Retrieval-Augmented Generation (RAG) agent built in **n8n** that delivers grounded, high-accuracy answers from internal policy documents. Designed for scalable support across departments, this agent uses Google Drive for ingestion, Gemini for embeddings and generation, and Supabase for vector storage.

---

## 📸 Workflow Overview  
<!-- Add your image below this line -->
![Workflow Diagram](../Assets/policy_rag_data_ingestion.png?raw=true "Policy RAG Agent Screenshot")

![Workflow Diagram](../Assets/policy_rag_main.png?raw=true "Policy RAG Agent Screenshot")

---

## 🔄 How It Works

### 1. 📁 Google Drive Trigger  
The workflow begins when a new document is added to a designated folder in Google Drive. This could be a policy PDF, internal memo, or reference guide.

### 2. 🧾 Document Processing & Meta Tagging  
- Each file is fetched and split into chunks using a **recursive character text splitter**  
- A **Code node** adds custom meta tags (e.g. department, topic, version) to each chunk  
- These tags are stored alongside the embeddings for filtered retrieval

### 3. 🧠 Embedding & Storage  
- Chunks are embedded using **Gemini’s embedding model**  
- Stored in a **Supabase vector database** for fast semantic search

### 4. 🎙️ Telegram Input Trigger  
Users send queries via Telegram—either as text or voice  
- Voice input is transcribed using AI  
- The query is passed to the RAG Agent

### 5. 📚 RAG Agent Response  
- Retrieves relevant chunks from Supabase based on semantic similarity  
- Generates a grounded, context-aware answer using Gemini  
- Sends the response back to the user via Telegram

---

## 🛠️ Tech Stack

- **n8n** – Workflow orchestration  
- **Google Drive** – Document ingestion  
- **Gemini** – Embedding + Generation  
- **Supabase** – Vector storage  
- **Telegram Bot** – User input and response channel  
- **JavaScript Code Node** – Meta tagging logic

---

## 🎯 Use Cases

- Internal policy support for government or enterprise teams  
- HR, legal, or compliance document Q&A  
- Scalable knowledge base assistant  
- Voice-enabled support bot for field teams

---

## 📌 Notes

- Meta tags allow for filtered retrieval 
- Voice input is transcribed and processed identically to text  
- New documents can be added to Drive to expand the knowledge base instantly  
- The system is modular—can be extended to support multiple departments or languages

---

> Built as part of my journey to become an AI automation specialist.  


