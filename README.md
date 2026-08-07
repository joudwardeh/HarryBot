# 🧙 HarryBot
## Harry Potter Domain-Specific Question Answering Chatbot

<p align="center">

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![AI Chatbot](https://img.shields.io/badge/AI-Chatbot-purple?style=for-the-badge)
![Dataset](https://img.shields.io/badge/Knowledge%20Base-Excel-green?style=for-the-badge)

</p>

---

## 📌 Overview

**HarryBot** is a Python-based domain-specific chatbot designed to answer questions related to the Harry Potter universe using a structured knowledge dataset.

Unlike general-purpose chatbots, HarryBot operates within a defined knowledge boundary. The system retrieves information from a custom dataset and provides answers only when relevant information is available. If the requested information cannot be found, the chatbot avoids generating unsupported responses.

The project demonstrates the development of a controlled question-answering system using Python, data processing, and rule-based response handling.

---

# 🎯 Project Objectives

The main objectives of HarryBot are:

- Build a chatbot specialized in the Harry Potter domain.
- Use a structured dataset as the chatbot's knowledge source.
- Provide accurate answers based on available information.
- Prevent irrelevant or unsupported responses.
- Create a simple and reliable conversational experience.

---

# ✨ Features

## 🔎 Knowledge-Based Question Answering

HarryBot searches a dedicated Harry Potter knowledge dataset to find relevant information and generate responses.

## 🛡️ Controlled Response Generation

The chatbot follows a strict answering policy:

- If information exists in the dataset → provide the answer.
- If information is unavailable → respond with:


I cannot answer that..


This prevents the chatbot from guessing or creating unsupported information.

## 💬 User Interaction Handling

The chatbot supports:

- General greetings
- Questions about the chatbot
- Harry Potter-related questions

---

# 🏗️ System Workflow

          User Question
                |
                ↓
      Input Processing
                |
                ↓
    Search Knowledge Dataset
                |
                ↓
   Information Available?
          /          \
         /            \
       Yes             No
        |               |
        ↓               ↓
Generate Answer   "I cannot answer that.."

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Main programming language |
| Pandas | Dataset processing |
| Excel Dataset | Knowledge source |
| NLP Techniques | Text processing and matching |

---

# 📂 Project Structure


HarryBot/
│
├── app.py
│ └── Application interface
│
├── chatbot.py
│ └── Core chatbot logic
│
├── harry_potter_data_02.xlsx
│ └── Harry Potter knowledge dataset
│
├── requirements.txt
│ └── Required Python packages
│
├── README.md
│ └── Project documentation
│
└── .gitignore
└── Ignored files and folders


---

# ⚙️ Installation & Setup

## 1. Clone the Repository

```bash
git clone <repository-url>
2. Install Dependencies
pip install -r requirements.txt
3. Run the Application
python app.py
🧪 Example Interaction
Example 1
User:
Who is Harry Potter?

HarryBot:
Returns information based on the available dataset.
Example 2
User:
Tell me about something unrelated.

HarryBot:
I cannot answer that..
📌 Design Approach
Data Grounding

HarryBot relies on a predefined dataset instead of generating answers from external knowledge.

Reliability

The system prioritizes providing supported answers rather than making assumptions.

Knowledge Limitation

The chatbot clearly identifies when requested information is outside its available knowledge.

🚀 Future Improvements

Future enhancements may include:

Adding semantic search using embeddings.
Implementing Retrieval-Augmented Generation (RAG).
Improving natural language understanding.
Expanding the knowledge database.
Deploying the chatbot as a web application.
---

---

# 📸 Screenshots

## Chatbot Interface

Example interaction with HarryBot:

![HarryBot Interface](screenshots/chatbot_interface.png)

## Example Question Answering

HarryBot answering a Harry Potter-related question:

![HarryBot Response](screenshots/chatbot_response.png)

---



---
👩‍💻 Author

Joud Wardeh

AI & Machine Learning Project