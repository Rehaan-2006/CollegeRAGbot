![Python](https://img.shields.io/badge/Python-3.10-blue)
![Streamlit](https://img.shields.io/badge/UI-Streamlit-red)
![ChromaDB](https://img.shields.io/badge/VectorDB-ChromaDB-orange)
![Ollama](https://img.shields.io/badge/LLM-Ollama-black)
![RAG](https://img.shields.io/badge/Architecture-RAG-green)
![Status](https://img.shields.io/badge/Status-Active-success)
![Stars](https://img.shields.io/github/stars/Rehaan-2006/CollegeRAGbot?style=social)
![Forks](https://img.shields.io/github/forks/Rehaan-2006/CollegeRAGbot?style=social)

# 📚 CollegeRAGbot

CollegeRAGbot is a fully **local Retrieval-Augmented Generation (RAG)
chatbot** designed to answer college-related queries using data scraped
from the official college website.

Instead of relying on generic internet responses, the bot retrieves
relevant context from a vector database built from college resources and
generates grounded answers --- all running locally.

------------------------------------------------------------------------

## 🚀 Features

-   📘 Retrieval-Augmented Generation (RAG) architecture\
-   🧠 Fully local LLM execution using Ollama\
-   🗂 ChromaDB vector storage for semantic search\
-   🌐 Crawl4AI for website data extraction\
-   💻 Streamlit-based interactive UI\
-   🔒 No API keys required

------------------------------------------------------------------------

## 🧩 Tech Stack

-   Python 3.10\
-   Ollama (Local LLM runtime)\
-   ChromaDB (Vector database)\
-   Crawl4AI (Web scraping)\
-   Streamlit (Frontend UI)

------------------------------------------------------------------------

## 🗂 Project Structure

    📦 CollegeRAGbot
    ├─ insert_docs.py       # Inserts scraped documents into vector DB
    ├─ rag_agent.py         # Core RAG pipeline logic
    ├─ streamlit_app.py     # Streamlit interface
    ├─ utils.py             # Helper functions
    ├─ requirements.txt     # Dependencies
    └─ README.md

------------------------------------------------------------------------

## ⚙️ Installation

### 1️⃣ Clone the repository

``` bash
git clone https://github.com/Rehaan-2006/CollegeRAGbot.git
cd CollegeRAGbot
```

### 2️⃣ Create virtual environment

``` bash
python -m venv venv
source venv/bin/activate     # macOS/Linux
venv\Scripts\activate        # Windows
```

### 3️⃣ Install dependencies

``` bash
pip install -r requirements.txt
```

### 4️⃣ Start Ollama

Ensure Ollama is installed and running locally before launching the bot.

------------------------------------------------------------------------

## 🧠 Insert College Data

Before running the chatbot, scrape and insert documents:

``` bash
python insert_docs.py
```

This extracts, embeds, and stores documents inside ChromaDB.

------------------------------------------------------------------------

## 💬 Run the Chatbot

Launch the Streamlit app:

``` bash
streamlit run streamlit_app.py
```

Open the local URL shown in the terminal and start asking questions.

------------------------------------------------------------------------

## 🧠 How It Works

1.  Crawl college website data\
2.  Chunk and embed documents\
3.  Store embeddings in ChromaDB\
4.  Retrieve relevant context\
5.  Generate grounded response using Ollama\
6.  Display answer via Streamlit

------------------------------------------------------------------------

## 📌 Future Improvements

-   Add multilingual support\
-   Add authentication layer\
-   Improve ranking & retrieval strategy\
-   Deploy as a containerized application

------------------------------------------------------------------------

## 📄 License

This project is licensed under the MIT License.
