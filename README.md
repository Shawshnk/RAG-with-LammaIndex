# RAG-with-LammaIndex


In short, the RAG (Retrieval-Augmented Generation) workflow using LlamaIndex involves these core steps:

**Load Data**: Ingest your raw data (PDFs, text files, databases, etc.) into LlamaIndex Documents.
**Index Data**: Transform these Documents into an Index, typically by splitting them into smaller "nodes" (chunks) and generating numerical vector embeddings for each node. These embeddings are stored in a VectorStore.
**Query**: When a user asks a question, the query is also converted into an embedding.
**Retrieve**: LlamaIndex uses the query embedding to perform a semantic search in the VectorStore, finding the most relevant data "nodes" (chunks) from your ingested knowledge base.
**Synthesize**: These retrieved relevant chunks are then provided as context to a Large Language Model (LLM) along with the original user query. The LLM uses this context to generate a more accurate and grounded answer, minimizing "hallucinations."


#Requirement:-
llama-index,
llama-index-embeddings-huggingface,
Chromadb,
llama-index-vector-stores-chroma,
llama_index.llms.huggingface_api
