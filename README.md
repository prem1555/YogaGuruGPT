# YogaGuruGPT

### A Specialized LLM-Based Yoga Education Assistant Using Retrieval-Augmented Generation (RAG)

## Project Overview

YogaGuruGPT is a domain-specific AI chatbot developed for the **Education and Training industry**. The project leverages Retrieval-Augmented Generation (RAG) to provide accurate and context-aware responses to yoga-related questions.

Instead of relying solely on the knowledge stored within a pre-trained language model, YogaGuruGPT retrieves relevant information from a curated collection of authentic yoga literature and uses that information to generate responses. This approach improves factual accuracy and ensures that answers are grounded in trusted yoga sources.

The chatbot is capable of answering questions related to:

* Yoga Philosophy
* Pranayama
* Meditation
* Yoga Anatomy
* Asanas
* Patanjali Yoga Sutras
* Bhagavad Gita
* Hatha Yoga Practices
* Traditional Yogic Concepts

---

## Problem Statement

Yoga students and practitioners often need to consult multiple books and resources to understand various concepts related to yoga. Information is distributed across different texts, making learning time-consuming and inefficient.

The objective of this project is to develop an intelligent yoga education assistant that can retrieve relevant information from authoritative yoga texts and generate meaningful responses to user queries.

---

## Project Objectives

* Build a domain-specific LLM chatbot for yoga education.
* Utilize authentic yoga literature as the knowledge base.
* Implement Retrieval-Augmented Generation (RAG).
* Enable semantic search using vector embeddings.
* Generate context-aware responses using a pre-trained language model.
* Provide an interactive chatbot interface for users.

---

## Knowledge Base

The chatbot uses the following yoga texts as its primary knowledge source:

1. Yoga Anatomy
2. Bhagavad Gita
3. Hatha Yoga Pradipika
4. Prana and Pranayama
5. Inside the Yoga Sutras
6. Shiva Samhita

These books provide comprehensive coverage of yoga anatomy, breathing techniques, meditation, philosophy, and traditional yoga practices.

---

## Technology Stack

### Programming Language

* Python

### Frameworks & Libraries

* LangChain
* Hugging Face Transformers
* Sentence Transformers
* FAISS
* Gradio

### Embedding Model

* all-MiniLM-L6-v2

### Language Model

* TinyLlama-1.1B-Chat-v1.0

### Vector Database

* FAISS (Facebook AI Similarity Search)

### Interface

* Gradio

---

## System Architecture

```text
Yoga Books (PDFs)
        │
        ▼
PDF Loading
        │
        ▼
Text Extraction
        │
        ▼
Document Chunking
        │
        ▼
Embedding Generation
        │
        ▼
FAISS Vector Database
        │
        ▼
Retriever
        │
        ▼
TinyLlama LLM
        │
        ▼
YogaGuruGPT Chatbot
```

---

## Methodology

### 1. Data Collection

A collection of yoga books was gathered to create a domain-specific knowledge base.

### 2. PDF Processing

The PDF documents were loaded using LangChain's PyPDFLoader.

### 3. Text Chunking

Large documents were divided into smaller overlapping chunks to improve retrieval performance.

### 4. Embedding Generation

Each chunk was converted into semantic vector embeddings using the Sentence Transformers model.

### 5. Vector Database Creation

The embeddings were stored in a FAISS vector database for efficient similarity search.

### 6. Retrieval-Augmented Generation

Relevant document chunks are retrieved based on the user's query and supplied to the language model as context for response generation.

### 7. Chatbot Interface

A Gradio interface was developed to allow users to interact with the chatbot.

---

## Project Workflow

### User Query

Example:

```text
What is Pranayama?
```

### Retrieval Phase

The retriever identifies the most relevant chunks from the yoga books.

### Generation Phase

The retrieved context is passed to TinyLlama, which generates a response grounded in the retrieved information.

### Final Response

The chatbot returns an informative answer to the user.

---

## Sample Questions

Users can ask questions such as:

* What is Pranayama?
* Explain Nadi Shodhana.
* What are the benefits of Kapalbhati?
* What is Karma Yoga?
* Who was Patanjali?
* Explain the Eight Limbs of Yoga.
* What is the significance of meditation in yoga?
* What are the benefits of Surya Namaskar?

---

## Results

The developed system successfully:

* Loaded and processed multiple yoga texts.
* Created semantic embeddings for knowledge retrieval.
* Built a FAISS vector database for efficient search.
* Generated context-aware responses using TinyLlama.
* Delivered an interactive chatbot experience through Gradio.

The chatbot demonstrated the ability to answer yoga-related questions using information derived from the uploaded literature.

---

## Advantages of the RAG Approach

* No expensive model fine-tuning required.
* Easy knowledge base updates.
* Improved factual grounding.
* Reduced hallucinations.
* Efficient use of computational resources.

---

## Limitations

* Performance depends on the quality of retrieved documents.
* Answers are limited to information available in the knowledge base.
* TinyLlama may occasionally generate incomplete responses for highly complex philosophical questions.
* The chatbot does not maintain long-term conversational memory.

---

## Future Improvements

* Add conversational memory.
* Support multilingual interactions.
* Integrate voice-based interaction.
* Use larger language models.
* Deploy the application on cloud platforms.
* Add citation-based responses showing source documents.

---

## Conclusion

YogaGuruGPT demonstrates how Retrieval-Augmented Generation can be used to build a specialized educational assistant using authentic yoga literature. By combining semantic retrieval, vector databases, and large language models, the system provides an accessible and intelligent platform for yoga learning and knowledge exploration.

The project highlights the practical application of AI and LLM technologies within the Education and Training industry and showcases the effectiveness of domain-specific conversational systems.

---

## Author

Premsagar Palled

**Project Title:** YogaGuruGPT | **Industry:** Education and Training
