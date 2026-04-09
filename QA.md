# 📚 RAG Interview Guide (Complete - 40+ Questions)

## 🧠 Overview
Retrieval-Augmented Generation (RAG) combines:
- Retrieval → fetch relevant data  
- Generation → LLM generates answer  

👉 Goal: Improve accuracy and reduce hallucination  

---

## 🔄 RAG Flow
Query → Retrieve → Context → Prompt → LLM → Answer  

---

# 🔹 Basic Questions

### 1. What is RAG?
RAG combines retrieval of relevant data with LLM generation to produce accurate answers.

### 2. Why use RAG?
- Reduces hallucination  
- Uses external/private data  
- Keeps responses up-to-date  
- No retraining required  

### 3. What are the components of RAG?
1. Document loading  
2. Chunking  
3. Embeddings  
4. Vector DB  
5. Retrieval  
6. Context  
7. Prompt  
8. LLM  

### 4. What is an embedding?
A vector representation of text capturing semantic meaning.

### 5. What is a vector database?
A database that stores embeddings and enables similarity search.

### 6. What is similarity search?
Finding most relevant documents using vector similarity.

### 7. What is context?
Retrieved document content passed to the LLM.

### 8. What is hallucination?
When an LLM generates incorrect or fabricated information.

### 9. How does RAG reduce hallucination?
By grounding responses in retrieved data.

### 10. Explain RAG in one line
Retrieves relevant data and uses it as context for LLM.

---

# 🔹 Intermediate Questions

### 11. Why split documents into chunks?
- Fit token limits  
- Improve retrieval accuracy  

### 12. What is chunk size?
Length of each text chunk.

### 13. What is chunk overlap?
Shared text between chunks.

### 14. What is top-k retrieval?
Fetching top K relevant documents.

### 15. What is a retriever?
An abstraction to fetch documents.

### 16. similarity_search vs retriever?
- similarity_search → direct  
- retriever → flexible  

### 17. What is metadata?
Extra info like source, page.

### 18. What is prompt engineering?
Designing prompts for LLM.

### 19. Why is prompt important?
Ensures correct usage of context.

### 20. What if context is too large?
Token overflow and higher cost.

---

# 🔹 Advanced Questions

### 21. How to improve retrieval?
- Better chunking  
- Better embeddings  
- Re-ranking  

### 22. What is re-ranking?
Reordering results for better relevance.

### 23. What is hybrid search?
Keyword + vector search.

### 24. How to evaluate RAG?
- Accuracy  
- Relevance  

### 25. Common RAG challenges?
- Poor retrieval  
- Token limits  

### 26. How to scale RAG?
- Distributed DB  
- Caching  

### 27. What is conversational RAG?
RAG with chat history.

### 28. RAG vs Fine-tuning?
RAG uses external data, fine-tuning updates model.

### 29. What is latency?
Delay in retrieval + LLM.

### 30. How to reduce latency?
Reduce chunk size, limit top-k.

---

# 🔹 Scenario-Based Questions

### 31. Retrieved docs irrelevant?
Improve embeddings and chunking.

### 32. Answer incorrect?
Improve prompt and retrieval.

### 33. No data found?
Return "I don't know".

### 34. Large documents?
Use chunking.

### 35. Add citations?
Use metadata.

---

# 🔹 Coding Questions

### 36. Retrieve documents
docs = vectorstore.similarity_search(query, k=3)

### 37. Build context
context = "\n\n".join([doc.page_content for doc in docs])

### 38. Create prompt
prompt = f"""Context:\n{context}\nQuestion:\n{query}\nAnswer:"""

### 39. Call LLM
response = llm.invoke(prompt)

### 40. Create retriever
retriever = vectorstore.as_retriever()

---

# 🏁 Summary
RAG = Retrieval + Context + LLM → Accurate Answer
