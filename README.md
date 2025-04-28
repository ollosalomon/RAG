# rag-qa-self

# rag-qa-self

Retrieval-Augmented Generation (RAG) application for personalized Question & Answering. 

---

## 🧠 Overview

This AI-powered application, built with  **Streamlit** , leverages a **Large Language Model (LLM)** to answer questions based on PDF documents about Ollo. It combines Retrieval-Augmented Generation (RAG) techniques with modern AI tooling to ensure accurate, context-aware responses.

**Key Technologies:**

* **LangChain** for orchestration
* **GPT4All** for embedding generation
* **Gemini 1.5** as the Language Model
* **Chroma DB** for the vector database
* **Streamlit** for the user interface

If the answer cannot be found within the provided data, the chatbot will gracefully indicate its inability to answer, minimizing misinformation.

---

## 🚀 Instructions

1. Clone the repository and navigate into the project directory `git clone https://github.com/ollosalomon/RAG.git`
2. Create a virtual environment `python -m venv "your virtual environnement name"`
3. Activate virtual environnement create `source "your virtual environnement name"/Scripts/activate`
4. Install the required dependencies:
   `pip install -r requirements.txt`
5. Get your **Gemini API Key** from [Google AI Studio](https://aistudio.google.com/).
6. Create a `.env` file in the project root with the following content:
   `GEMINI_API_KEY="YOUR_API_KEY_HERE`
7. Create the vector database from your PDF documents:
   `python create_db.py`
8. Launch the Streamlit app:
   `streamlit run main.py`

---

## 📄 Project Features

* **Document Ingestion:** Automatically splits PDFs into manageable chunks and stores them as embeddings.
* **Contextual Q&A:** Handles follow-up questions intelligently using chat history.
* **Reliable Responses:** Only answers based on retrieved context to reduce hallucinations.
* **Simple Deployment:** Lightweight Streamlit app for quick and easy access

RAG based application on question and answer about myself

**Overview**

This AI-powered app, built with Streamlit, uses a Large Language Model (LLM) to answer questions based on PDF data about Ollo. Key technologies include:

- Langchain as the framework,
- GPT4All for embedding generation,
- Gemini 1.5 as the LLM,
- Streamlit for the user interface, and
- Chroma DB as the vector database.

**Instructions**

1. run pip install -r requirements.txt
2. generate your own GEMINI API KEY from https://aistudio.google.com/ and put it in .env file as GEMINI_API_KEY = "YOUR_KEY"
3. run `python create_db.py` in the terminal to create the vector database from the documents.
4. run `streamlit run main.py` to launch streamlit UI in the browser
