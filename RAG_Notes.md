# RAG

1. RAG -> Retrieval Augmented Generation.
2. Since LLMs are already trained on vast volumes of data, RAG extends the already powerful capabilities of LLMs to specific domains or an organization's internal knowledge base, all without the need to retrain the model.
3. It is a cost-effective approach to improving LLM output so that it remains relevant, accurate, and useful in various contexts.
4. Disadvantages of LLM outputs: 
  1. Hallucinating when answers are not known.
  2. No fine-tuning
5. Data stored in a vector database goes through these stages:
Any data (structured or unstructured) -> Parsing (creating chunks) -> Embedding (generating text to vectors) -> storage (This whole pipeline is called Data Ingestion Pipeline)
6. Once the knowledge base is formed, the query is embedded and sent to the vector DB (Knowledge Base), and the related information (context) + prompt is sent to the LLM for the output. This is the traditional RAG retrieval pipeline.
7. Even in these situations, hallucination cannot be completely eliminated, but it is way less than before.

# LangChain
1. LangChain Document is a type of data structure that has 2 core components: page_content(str) and metadata(dict).
2. LangChain has different document loaders. Example: PDF Loader, CSV Loader, Web Base Loader, Directory Loader.
