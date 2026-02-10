# Medical Chatbot

An AI-powered medical chatbot built with Streamlit, LangChain, and FAISS vector store. It uses the Gale Encyclopedia of Medicine as its knowledge base and Groq's LLM for generating responses.

## Features
- RAG (Retrieval-Augmented Generation) based medical Q&A
- FAISS vector store for fast similarity search
- Streamlit chat interface
- Powered by Groq API (LLama model)

## Setup

### Prerequisites
- Python 3.9+
- A [Groq API Key](https://console.groq.com/keys)

### Local Setup
```bash
pip install -r requirements.txt
```

Set your Groq API key:
```bash
export GROQ_API_KEY="your_groq_api_key_here"
```

Run the app:
```bash
streamlit run medibot.py
```

## Deployment on Streamlit Cloud
1. Push this repo to GitHub
2. Go to [share.streamlit.io](https://share.streamlit.io)
3. Connect your GitHub repo
4. Set main file as `medibot.py`
5. Add your `GROQ_API_KEY` in **Advanced Settings > Secrets**:
   ```toml
   GROQ_API_KEY = "your_groq_api_key_here"
   ```
