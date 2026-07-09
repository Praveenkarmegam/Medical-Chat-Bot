# 🩺 Medical RAG Chatbot using BioMistral, LangChain & ChromaDB

An AI-powered **Medical Retrieval-Augmented Generation (RAG) Chatbot** built using **BioMistral-7B**, **LangChain**, **ChromaDB**, and **PubMedBERT Embeddings**. The chatbot retrieves relevant information from medical PDF documents and generates accurate, context-aware responses using a locally hosted BioMistral large language model.

## 🚀 Features

* 📄 Load multiple medical PDF documents
* ✂️ Automatic document chunking using LangChain
* 🧬 Medical embeddings with PubMedBERT
* 🔍 Semantic search using ChromaDB vector database
* 🤖 BioMistral-7B GGUF model for response generation
* 💬 Interactive command-line chatbot
* 🏥 Domain-specific medical question answering

---

## 🛠️ Tech Stack

* Python
* LangChain
* BioMistral-7B (GGUF)
* Llama.cpp
* ChromaDB
* Sentence Transformers
* PubMedBERT Embeddings
* PyPDF
* Google Colab

---

## 📂 Project Structure

```text
Medical-RAG-Chatbot/
│
├── Data/
│   ├── medical_book_1.pdf
│   ├── medical_book_2.pdf
│   └── ...
│
├── Model/
│   └── BioMistral-7B.Q4_K_M.gguf
│
├── Medical_Chat_Bot.ipynb
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/praveenkarmegam/Medical-RAG-Chatbot.git
cd Medical-RAG-Chatbot
```

Install the required dependencies:

```bash
pip install langchain
pip install sentence-transformers
pip install chromadb
pip install llama-cpp-python
pip install langchain-community
pip install pypdf
```

Or install everything at once:

```bash
pip install langchain sentence-transformers chromadb llama-cpp-python langchain-community pypdf
```

---

## 📥 Dataset

Place your medical PDF files inside:

```text
Data/
```

The chatbot automatically loads all PDFs from this directory.

---

## 🧠 Model

Download the **BioMistral-7B GGUF** model and place it inside:

```text
Model/
```

Example:

```text
Model/
└── BioMistral-7B.Q4_K_M.gguf
```

Update the model path in the notebook if necessary.

---

## 🔄 Workflow

1. Load medical PDF documents.
2. Split documents into smaller chunks.
3. Generate embeddings using PubMedBERT.
4. Store embeddings in ChromaDB.
5. Retrieve relevant document chunks for user queries.
6. Generate responses using BioMistral-7B.
7. Display context-aware medical answers.

```text
Medical PDFs
      │
      ▼
Document Loader
      │
      ▼
Text Splitter
      │
      ▼
PubMedBERT Embeddings
      │
      ▼
ChromaDB Vector Store
      │
      ▼
Retriever
      │
      ▼
BioMistral-7B
      │
      ▼
Medical Answer
```

---

## 💬 Example

**Input**

```text
Who is at risk of heart disease?
```

**Output**

```text
People with high blood pressure, diabetes, obesity, smoking habits,
high cholesterol, lack of physical activity, and a family history
of cardiovascular disease are at greater risk of developing heart disease.
```

---

## 📦 Libraries Used

* langchain
* langchain-community
* sentence-transformers
* chromadb
* llama-cpp-python
* pypdf

---

## 🎯 Future Improvements

* Web interface using Streamlit or React
* Chat history and conversation memory
* Voice input and speech output
* Medical report summarization
* Multi-document retrieval
* Source citations for generated responses
* Docker deployment
* Authentication and user management

---

## ⚠️ Disclaimer

This project is intended for educational and research purposes only. It should **not** be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult qualified healthcare professionals for medical decisions.

---

## 👨‍💻 Author

**Praveen Karmegam**

* GitHub: https://github.com/praveenkarmegam

If you found this project useful, consider giving it a ⭐ on GitHub.
