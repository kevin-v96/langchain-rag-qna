This is a simple Question-Answering RAG pipeline written using LangChain, Chroma Vector Database, GPT3.5, and Sentence Transformers.

We first split and embed the source text (in this case a web scrape of marxists.org) and embed it using sentence transformers.
Then, we store these embeddings in a vector database. This allows efficient retrieval by calculating the similarity scores between our question and the vectors in the database.
These retrieved documents are then sent to our LLM (in this case GPT3.5), which uses them to generate a textual answer relevant to us. 
