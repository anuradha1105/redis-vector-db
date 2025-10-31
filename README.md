# 🧠 Redis Vector Database with Embedding Cache

### 🎯 Objective
To create a **Redis Vector Database** and demonstrate how embeddings can
be stored, cached, and queried to answer semantic search queries
efficiently.

------------------------------------------------------------------------

### ⚙️ Project Overview
This notebook implements a **vector search system** using Redis Stack
and text embeddings.
The project covers:
- Connecting to Redis Cloud\
- Creating a **vector index** using RediSearch
- Generating and caching embeddings for text documents
- Performing **semantic queries** using vector similarity (KNN)

Initially, the project used **OpenAI's `text-embedding-3-small`**
model however, due to an API quota limit, it was replaced with a **free, local
model**`SentenceTransformer('all-MiniLM-L6-v2')`.\

------------------------------------------------------------------------

### 🧩 Key Steps

1.  Install dependencies

    ``` bash
    pip install redis sentence-transformers numpy
    ```

2.  Connect to Redis Cloud or local Redis Stack instance\

3.  Create a vector index (`FT.CREATE`) for 384-dimensional vectors\

4.  Generate embeddings using SentenceTransformers\

5.  Store documents and embeddings in Redis hashes\

6.  Run semantic queries using KNN vector search


------------------------------------------------------------------------

### ✅ Results
-   Redis successfully stored and indexed embeddings.\
-   Semantic queries returned correct results based on meaning, not
    keywords.\
-   The project shows Redis can act as both a **cache** and **vector
    database** for AI search.

------------------------------------------------------------------------

### 💡 Tools Used
-   **Redis Stack / Redis Cloud**\
-   **SentenceTransformers** (all-MiniLM-L6-v2)\
-   **Python / Google Colab**

------------------------------------------------------------------------

### 🧾 Credits
Developed as part of a learning exercise on **vector databases and
caching**.\
Demonstrates Redis as a real-time store for AI embeddings.
