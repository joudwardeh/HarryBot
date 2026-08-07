# 🧙 HarryBot - Harry Potter AI Chatbot

<p align="center">

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![Streamlit](https://img.shields.io/badge/Interface-Streamlit-red?style=for-the-badge&logo=streamlit)
![FAISS](https://img.shields.io/badge/Search-FAISS-green?style=for-the-badge)
![AI](https://img.shields.io/badge/AI-Chatbot-purple?style=for-the-badge)

</p>

---

## 📌 Overview

**HarryBot** is an AI-powered retrieval-based chatbot designed to answer questions about the Harry Potter universe.

The system combines **semantic search, FAISS vector retrieval, conversational memory, similarity threshold filtering, and a language model** to provide accurate and context-aware responses.

Unlike general-purpose chatbots, HarryBot is restricted to its provided knowledge base to reduce hallucinations and prevent unsupported answers.

---

## ✨ Features

- 🔎 Uses **FAISS vector search** for efficient information retrieval
- 🧠 Uses **Sentence Transformers embeddings** for semantic similarity matching
- 💬 Supports **conversational memory** for follow-up questions
- 🎯 Applies **similarity threshold filtering** to improve answer reliability
- 📚 Answers questions using a dedicated Harry Potter knowledge base
- 🚫 Rejects unsupported or out-of-scope questions
- 👋 Handles greetings and chatbot-related questions
- 🛡️ Includes protections against prompt injection and jailbreak attempts
- 🖥️ Provides an interactive **Streamlit user interface**

---

# 🏗️ System Architecture

The chatbot follows a retrieval-based question answering pipeline:


User Question
|
↓
Streamlit Interface
|
↓
Generate Query Embedding
|
↓
FAISS Similarity Search
|
↓
Similarity Threshold Check
|
┌───────────────┐
│ │
High Similarity Low Similarity
│ │
↓ ↓
Return Answer Retrieve Context
|
↓
Language Model
|
↓
Generated Response


---

# 🛠️ Technology Stack

| Component | Technology |
|-----------|------------|
| Programming Language | Python 3.11 |
| User Interface | Streamlit |
| Data Processing | Pandas, OpenPyXL |
| Embedding Model | Sentence Transformers (all-MiniLM-L6-v2) |
| Vector Database/Search | FAISS (IndexFlatIP) |
| Language Model | Qwen-Plus |
| API Client | OpenAI Python SDK |
| Numerical Processing | NumPy |

---

# 📂 Project Structure


HarryBot/
│
├── app.py
│ └── Streamlit application interface
│
├── chatbot.py
│ └── Core chatbot implementation
│
├── harry_potter_data_02.xlsx
│ └── Harry Potter knowledge base
│
├── requirements.txt
│ └── Required Python packages
│
└── README.md
└── Project documentation


---

# ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone <repository-url>
2. Install dependencies
pip install -r requirements.txt
3. Run the application
streamlit run app.py
💬 Example Behavior
Supported Question
User:
Who is Hermione Granger?

HarryBot retrieves relevant information from the knowledge base and generates a response.

Unsupported Question
User:
What is the weather today?

Response:

I cannot answer that..
📸 Screenshots

Add screenshots here:

screenshots/
├── interface.png
└── response.png

Example:

🚀 Future Improvements
Expand the knowledge base with additional Harry Potter information
Improve retrieval accuracy with advanced ranking methods
Add voice interaction capabilities
Deploy the chatbot as a web application
Enhance memory management for longer conversations
👩‍💻 Author
Joud Wardeh