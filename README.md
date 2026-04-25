# 🚀 RAG-Based Customer Support Assistant

A **Retrieval-Augmented Generation (RAG)** system that answers user queries using a PDF knowledge base.  
The system uses **semantic retrieval, workflow-based execution (LangGraph), and Human-in-the-Loop (HITL)** for improved reliability.

---

## 📌 Project Objective

To design and implement a system that:
- Processes a PDF knowledge base  
- Retrieves relevant information using embeddings  
- Generates context-aware answers  
- Uses a graph-based workflow for decision-making  
- Supports Human-in-the-Loop (HITL) escalation  

---

## ⚙️ Tech Stack

- Python  
- LangChain  
- ChromaDB  
- LangGraph  
- HuggingFace Embeddings  
- Jupyter Notebook / Google Colab  

---

## 🏗️ System Architecture


User Query
↓
LangGraph Workflow
↓
Retriever (ChromaDB)
↓
Answer Generator
↓
Decision Node
/
Output HITL


---

## 🔄 Workflow

1. Load PDF knowledge base  
2. Split into chunks  
3. Convert chunks into embeddings  
4. Store in vector database (ChromaDB)  
5. Accept user query  
6. Retrieve relevant chunks  
7. Generate answer  
8. Evaluate confidence  
9. Route:
   - High confidence → Return answer  
   - Low confidence → Escalate to human  

---

## 🧠 Key Features

- 📄 PDF-based knowledge system  
- 🔍 Semantic search using embeddings  
- 🔗 Vector database (ChromaDB)  
- 🔄 Graph-based workflow using LangGraph  
- ⚠️ Human-in-the-Loop (HITL) support  
- 🧪 Easy testing in Jupyter Notebook  

---

## 📂 Project Structure


project/
│
├── notebook.ipynb # Main implementation
├── support.pdf # Knowledge base
├── README.md # Project documentation
├── HLD.pdf # High-Level Design
├── LLD.pdf # Low-Level Design
└── Technical_Doc.pdf # Technical documentation


---

## ▶️ How to Run

### 1. Install Dependencies

pip install langchain langchain-community langgraph chromadb sentence-transformers pypdf


### 2. Upload PDF
Upload `support.pdf` in Jupyter/Colab.

### 3. Run Notebook Cells
- Load PDF  
- Chunk data  
- Create embeddings  
- Build vector database  
- Run LangGraph workflow  

### 4. Test Queries

ask("What is refund policy?")
ask("How long is shipping?")
ask("random question")


---

## ⚠️ HITL Behavior

If system confidence is low:


⚠️ Escalated to Human Agent


User manually enters response.

---

## 🔮 Future Enhancements

- Integrate LLM APIs (OpenAI / Groq)  
- Add web UI (Streamlit)  
- Multi-document support  
- Conversation memory  
- Feedback learning system  

---

## 🧪 Sample Queries

- What is refund policy?  
- How long is shipping?  
- How to contact support?  

---

## 📌 Conclusion

This project demonstrates a **practical implementation of RAG architecture** with workflow-based control and human escalation, making it suitable for real-world customer support applications.
