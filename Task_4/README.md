Task 4: Context-Aware Chatbot Using LangChain (RAG)
Objective

To build a chatbot that:

Retrieves relevant information from a custom knowledge base
Uses vector embeddings for semantic search
Maintains conversational context using chat memory
Provides accurate answers grounded in retrieved documents
Key Features
Retrieval-Augmented Generation (RAG) pipeline
FAISS vector database for similarity search
HuggingFace sentence embeddings
Custom knowledge base on Pakistan climate
Conversation memory for context awareness
Lightweight interactive chatbot (Colab-based CLI)
Dataset

A custom textual knowledge base was created covering:

Climate of Northern Areas
Punjab climate conditions
Sindh desert and coastal climate (Karachi)
Balochistan arid climate
Monsoon season in Pakistan
Flood events (2010, 2022)
Climate change impacts

The dataset is defined manually within the notebook.

Methodology / Approach
1. Data Preparation

A structured climate knowledge base was created and converted into LangChain Document format.

2. Text Processing

Documents were split into smaller chunks using RecursiveCharacterTextSplitter to improve retrieval accuracy.

3. Embedding Generation

Text chunks were converted into dense vector representations using:

sentence-transformers/all-MiniLM-L6-v2
4. Vector Database

FAISS was used to store embeddings and perform efficient similarity search.

5. Retrieval System

User queries are converted into embeddings and matched with the most relevant documents.

6. Chatbot Logic

Retrieved context is combined with user input and previous conversation history to generate grounded responses.

Chatbot Workflow

User Query → Embedding → FAISS Retrieval → Relevant Context → Response Generation → Output

Example Queries
Input:

What is the climate of Sindh?

Output:

Sindh has a hot desert climate. Karachi experiences humid coastal weather due to the Arabian Sea.

Input:

Tell me about Punjab climate

Output:

Punjab experiences very hot summers above 40°C and cool winters.

Input:

What are floods in Pakistan?

Output:

Severe floods occurred in 2010 and 2022 affecting millions of people in Pakistan.

Key Results & Observations
FAISS enabled efficient semantic retrieval of climate-related data
Embedding-based search improved accuracy compared to keyword matching
Chat memory allowed context-aware responses across multiple queries
Retrieval-based approach reduced hallucination compared to pure LLM outputs
System successfully demonstrates a complete RAG pipeline
Technologies Used
Python
LangChain
FAISS (Vector Database)
HuggingFace Transformers
Sentence Transformers
Google Colab
Jupyter Notebook / Google Colab
