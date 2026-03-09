📚 RAG Chatbot using LangChain, Pinecone, and HuggingFace

This project implements a **Retrieval-Augmented Generation (RAG) chatbot** that answers questions based on the content of PDF documents.

The system extracts information from uploaded PDFs, stores document embeddings in a vector database, retrieves relevant content for a user query, and generates an answer using a language model.


🚀 Features

* 📄 **PDF Question Answering** – Ask questions about uploaded PDF documents
* 🔎 **Semantic Search** – Uses vector embeddings for intelligent document retrieval
* 🧠 **Conversation Memory** – Maintains context from previous questions
* ⚡ **Local LLM Inference** – Runs a local Llama-based model using `ctransformers`
* 📦 **Vector Database Storage** – Uses Pinecone to store and search embeddings


🏗 System Architecture

The chatbot follows the **RAG pipeline**:

PDF Documents
      ⬇
Document Loader
      ⬇
Text Splitter
      ⬇
Embeddings Model
      ⬇
Vector Database (Pinecone)
      ⬇
Retriever
      ⬇
Language Model
      ⬇
Generated Answer


🧰 Technologies Used

* LangChain
* Pinecone Vector Database
* HuggingFace Embeddings
* Sentence Transformers
* Local LLaMA Model (ctransformers)
* Python



📂 Project Structure


rag-chatbot
│
├── rag_chatbot.ipynb     # Main RAG chatbot notebook
├── pdf1.pdf              # Example document-1
├── pdf2.pdf              # Example document-2
└── README.md



⚙ Installation

Install required dependencies:

```
pip install langchain
pip install langchain-community
pip install langchain-core
pip install langchain-classic
pip install langchain-huggingface
pip install langchain-pinecone
pip install pinecone
pip install pypdf
pip install sentence-transformers
pip install ctransformers
pip install langchain-text-splitters
```


🔑 API Keys

This project requires the following API keys:

* Pinecone API Key
* HuggingFace API Token

Set them as environment variables before running the notebook.

Example:
```
export PINECONE_API_KEY="your_key"
export HUGGINGFACE_API_KEY="your_key"
```

THANK YOU😌
