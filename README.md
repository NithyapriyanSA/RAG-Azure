**Azure AI Search uses HNSW to efficiently retrieve nearest embedding vectors during semantic search. Text-embedding-3-small converts text into dense semantic vectors. During hybrid search, Azure combines BM25 keyword matching with vector similarity scores to retrieve the most relevant chunks, which are then passed to the LLM for grounded responses.**

“During indexing, documents are embedded and stored in an HNSW vector index; during querying, BM25 and vector search run independently and results are re-ranked via score fusion.”

“HNSW builds a multi-layer proximity graph where upper layers provide sparse long-range links for fast navigation, and lower layers provide dense local connections for precise nearest-neighbor search.”
