# HelpMate – RAG-Powered Insurance Query Bot

A Capstone Project for GenAI UpGrad x IIITB  
*Effortlessly navigate insurance documents with Retrieval-Augmented Generation (RAG) and OpenAI’s GPT-based language models.*

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/python-3.8%2B-brightgreen.svg)](https://www.python.org/)

---

## ✨ Project Overview

**AssistAI** is a smart assistant built to demystify and simplify the process of querying dense and jargon-heavy insurance documents. Reading through lengthy policy terms or filing procedures can be a challenge—this tool streamlines that experience using Retrieval-Augmented Generation (RAG), combining powerful retrieval mechanisms with the language fluency of large language models.

**Example queries it can handle:**
- “Does my plan cover maternity expenses?”
- “What documents are required to file a car insurance claim?”

---

## 🔍 Core Features

- 🔎 **Accurate Data Retrieval** – Uses vector embeddings to fetch the most relevant snippets from documents.
- 🧠 **Contextual AI Responses** – Generates human-readable explanations using modern LLMs like GPT-4, Gemini, or Claude.
- 🚀 **Fast Performance** – Caching and ChromaDB optimization ensures rapid turnaround times.
- 💡 **Document Intelligence** – Extracts content from PDFs, including tables and structured data.
- 🧾 **Multi-Model Flexibility** – Easily switch between GPT-based models or integrate any SOTA LLM via APIs.
- 👨‍💻 **Intuitive UX** – Designed for ease of use through a streamlined Jupyter Notebook interface.

---

## ⚙️ Technology Stack

- **Programming Language:** Python (via Jupyter Notebooks)
- **Libraries & Frameworks:** Transformers, ChromaDB, PDFplumber, Sentence Transformers
- **Models & APIs:** GPT-4 / GPT-4o / Gemini / Claude / Other modern LLMs
- **Environment:** Local setup or cloud-deployable using Docker (optional)

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or later
- Docker (optional, for containerization)

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/vikrampawar88/Helpmate_RAG_Project.git
   ```

2. **Navigate to the Project Folder**
   ```bash
   cd HelpMate_AI_Project_GenAI_UpGrad_IIITB
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure API Keys**
   Update the notebook/code with your OpenAI or Gemini API key.

5. **Run the Application**
   Launch `helpmate-ai-rag-project_vikram.ipynb` inside your Jupyter environment.

---

## 📚 Reference Documentation

This solution integrates tools and models that are well-documented. For detailed understanding, please refer to:

- [ChromaDB](https://docs.trychroma.com/)  
- [PDFplumber](https://pypi.org/project/pdfplumber/)  
- [Sentence Transformers](https://www.sbert.net/docs/)  
- [OpenAI API Docs](https://platform.openai.com/docs/)

---

## 🧩 Challenges and Solutions

- **PDF Parsing Tools** – Initial tools like PyPDF2 didn’t suffice. Settled on `pdfplumber` for accurate text and table extraction.
- **Table Handling** – Rewrote parsing logic to handle table structures, maintaining data sequence.
- **Embedding Optimization** – Introduced caching in ChromaDB to skip redundant embeddings and speed up retrieval.
- **Improved Passage Ranking** – Used a Cross Encoder Reranker to improve passage relevance for better answers.
- **Prompt Engineering** – Reworked system prompts with few-shot examples and guiding instructions to improve output quality.

---

## 🚧 Upcoming Enhancements

- [ ] Integrate additional model providers (e.g., Claude, HuggingFace Transformers, Mistral, etc.)
- [ ] Add advanced filtering/search options for queries.
- [ ] Enable vector store switching (e.g., Pinecone, Weaviate).

---

## 🛡️ License

This project is open-source and licensed under the MIT License. Check the `LICENSE` file for more details.

---
