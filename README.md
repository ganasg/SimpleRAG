# SimpleRAG
A simple LLM RAG python notebook leveraging open source llm models on a FAQ doc leveraging Amazon Sagemaker
# Two notebooks:
1. 01-deploy-text-embedding-model.ipynb - Deploy Text Embedding Model (GPT-J 6B FP-16) on ml.g4dn.2xlarge. This model will be used to generate a numerical representation of the textual documents.
2. 02-km-question-answering-rag.ipynb - Three key components

   a. LLM (Large Language Model): Llama-2-7b model will be used to understand the document chunks and provide an answer in human friendly manner.

   b. Vector Store: FAISS available through LangChainIn this notebook we are using this in-memory vector-store to store both the embeddings and the documents. 

   c. Index: VectorIndex The index helps to compare the input embedding and the document embeddings to find relevant document

Make the following changes to have this notebook work on your document of interest 
create a folder in home directory as src_doc and your text file. Update the name of the text file inside "02-km-question-answering-rag.ipynb". Good to go!
