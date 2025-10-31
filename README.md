# Redis Vector Database – Embedding Cache Project

### 🎯 Objective
Build a vector database using Redis Stack and embeddings to answer semantic queries.

### 🧠 Overview
- Connected Redis Cloud (RediSearch enabled)
- Created vector index (HNSW + Cosine Similarity)
- Stored title, content, and embeddings in Redis
- Queried documents by similarity using `KNN`

### ⚙️ Implementation
Used `sentence-transformers` free model (`all-MiniLM-L6-v2`) for local embeddings  
after hitting OpenAI quota limits (`RateLimitError`).

### ✅ Result
Redis returned correct semantic matches for user prompts,  
proving Redis can cache and query embeddings effectively.
