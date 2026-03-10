# MultiModalRAG – Multimodal RAG Chatbot for Research Papers

**Chat with research papers like a human – understand text, images, tables, and figures together.**

MultiModalRAG is a local-first multimodal Retrieval-Augmented Generation (RAG) system that lets you ask natural questions about research papers (e.g., "Attention is All You Need") and get grounded answers from both text **and visual content** (diagrams, tables, figures).

## Approach 1: in MM-RAG
<img width="850" height="431" alt="image" src="https://github.com/user-attachments/assets/10c39482-64b2-4c60-b225-4b06c49df0e4" />

<img width="850" height="494" alt="image" src="https://github.com/user-attachments/assets/24bbc42d-fb97-4189-99b7-01b7b61a30e1" />


## Approach 2: in Multimodal-RAG 
Advanced Approach with CLIP + Ensemble Retriever using Similarity search and MMR(rereanker)

<img width="1536" height="1024" alt="ChatGPT Image Aug 17, 2025, 07_25_28 PM" src="https://github.com/user-attachments/assets/7cbd9cc4-aa9b-45cf-ad4c-9b2ca84b7d83" />

# Features

- Multimodal RAG pipeline using **LangChain** – handles text + embedded images/tables from PDFs.
- Two approaches:
  - **Approach 1** (`MM_RAG.ipynb`): Simple multimodal ingestion and retrieval.
  - **Approach 2** (`Multimodal_rag.ipynb`): Advanced ensemble retriever with CLIP embeddings + MMR re-ranking for better visual relevance.
- Local execution – no cloud API needed (use Ollama, local embeddings, etc.).
- Grounded Q&A – answers cite exact text passages **and** describe relevant figures/tables.
- Easy to extend: Swap LLMs, add more papers, improve chunking/visual extraction.
