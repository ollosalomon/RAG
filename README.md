# rag-qa-self
RAG based application on question and answer about myself

**Overview**

This AI-powered app, built with Streamlit, uses a Large Language Model (LLM) to answer questions based on PDF data about Ana. Key technologies include:

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
