# AI Restaurant Information Agent (n8n Workflow)

This repository contains an **AI-powered automation workflow built in n8n**.  
The agent reads restaurant documents from Google Drive, converts them into embeddings, stores them in Supabase, and provides intelligent answers to chat messages using OpenAI and Google Gemini models.

---

## 🚀 Project Overview

This AI Agent automatically:

- Detects new or updated files in Google Drive  
- Downloads and processes the restaurant document (`Urban Grill House Restaurant.docs`)  
- Splits the document into chunks and generates embeddings  
- Stores embeddings inside **Supabase Vector Store**  
- Responds to chat messages using **RAG (Retrieval-Augmented Generation)**  
- Uses **Google Gemini**, **OpenAI Embeddings**, **Supabase**, and **Memory** for accurate responses  

This workflow can be used for:

- Customer support automation  
- Restaurant or menu information bot  
- Business knowledge assistant  
- FAQ automation  
- Document-based RAG agents  

---

## 🧠 Features

### ✔ 1. Automated Google Drive → Vector Database Pipeline
- **Google Drive Trigger** detects file changes  
- **Download File** fetches the document  
- **Default Data Loader** + **Recursive Character Text Splitter** prepare text  
- **OpenAI Embeddings** generate vector representations  
- **Supabase Vector Store** saves embeddings for search  

### ✔ 2. Intelligent Chat Agent
- **When Chat Message Received** triggers the workflow  
- **AI Agent** node handles the conversation  
- Enhanced with:
  - Google Gemini Chat Model  
  - Simple Memory  
  - Supabase Vector Search  
  - OpenAI Embeddings  

### ✔ 3. RAG (Retrieval-Augmented AI Responses)
The agent retrieves relevant document chunks from Supabase before answering, ensuring:

- High accuracy  
- Context-aware responses  
- Data grounded in the uploaded restaurant document  

---

## 🗂 Workflow Structure


---

## 📥 How to Import the Workflow in n8n

1. Open **n8n**
2. Go to **Workflows**
3. Click **Import**
4. Upload `workflow.json`
5. Add your credentials:
   - Google Drive  
   - Supabase  
   - OpenAI  
   - Google Gemini  

Your automation agent is now ready to use.

---

## 🧩 Tech Stack

- **n8n** – Workflow automation  
- **Google Drive API** – File monitoring & downloading  
- **OpenAI Embeddings** – Vector generation  
- **Supabase Vector Store** – Semantic retrieval  
- **Google Gemini Chat Model** – AI response generation  
- **Simple Memory** – AI conversation context  
- **RAG Pipeline** – Document-grounded answers  

---

## 📌 Example Use Cases

- Restaurant menu Q&A assistant  
- Automated customer support bot  
- Document-based AI chat system  
- Internal knowledge agent for staff  
- FAQ system powered by business documents  

---

## 🤝 Contributing

Suggestions, improvements, and pull requests are welcome.

---

## ⭐ Support

If you find this project useful, please consider giving the repository a ⭐ **star**.

---
