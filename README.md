# Knowledge Base Router using LangChain (Multi-Agent Architecture)

This project demonstrates how to build a **Knowledge Base Router** using **LangChain’s multi-agent routing mechanism**, where user queries are dynamically routed to the most relevant knowledge source based on intent and content.

The implementation follows the official LangChain documentation on **router-based multi-agent systems** and showcases how multiple domain-specific knowledge bases can be orchestrated intelligently.

---

## 🧠 Problem Statement

In real-world AI applications, a single knowledge base is often insufficient.  
Different user queries require answers from **different domains**, such as:

- Product documentation
- FAQs
- Technical manuals
- Support policies

This project solves that problem by **automatically routing user queries to the correct knowledge base** using an LLM-powered router.

---

## 🏗️ Architecture Overview

**Flow:**

1. User submits a query
2. Router Agent analyzes the intent
3. Query is routed to the most relevant Knowledge Base
4. Selected Knowledge Base retrieves context
5. Final response is generated using the retrieved information

---

## 🛠️ Tech Stack

- **Python**
- **LangChain**
- **LLM (OpenAI / compatible model)**
- **Vector Stores**
- **Multi-Agent Router Pattern**

---

## 📂 Project Structure

.
├── Knowledge_Base_Router_via_Langchain.ipynb
├── README.md
└── requirements.txt


---

## 🔍 Key Concepts Used

- **Router Chain**
- **Knowledge Base Selection**
- **Multi-Agent Coordination**
- **Semantic Routing**
- **LLM-based Decision Making**

---

## ⚙️ How It Works (High Level)

- Each knowledge base is defined as a **tool / retriever**
- A **router prompt** describes when each knowledge base should be used
- The router uses the LLM to decide:
  > “Which knowledge source is best suited to answer this query?”
- Only the selected knowledge base is queried, improving accuracy and efficiency
<img width="1274" height="455" alt="image" src="https://github.com/user-attachments/assets/16416794-66ef-42ed-a3d2-1c05e5326794" />

---

## 🚀 Getting Started

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
2️⃣ Set Environment Variables
export OPENAI_API_KEY="your_api_key_here"
3️⃣ Run the Notebook
Open and execute:

Knowledge_Base_Router_via_Langchain.ipynb
🧪 Example Use Cases
Intelligent customer support systems

Enterprise document search

AI-powered help desks

Domain-aware chatbots

Agentic RAG systems

📌 Why This Matters
✅ Reduces hallucinations
✅ Improves answer relevance
✅ Scales across multiple domains
✅ Core building block for Agentic AI systems

📚 Reference
LangChain Documentation:
https://docs.langchain.com/oss/python/langchain/multi-agent/router-knowledge-base
