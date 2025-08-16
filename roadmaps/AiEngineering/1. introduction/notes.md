# Ai Engineer vs ML Engineer
An AI Engineer uses pre-trained models and existing AI tools to improve user experiences. They focus on applying AI in practical ways, without building models from scratch. This is different from AI Researchers and ML Engineers, who focus more on creating new models or developing AI theory.

# AI vs AGI
AI = narrow, task-specific. AGI = broad, human-like intelligence across many domains.

# Inference
Inference in AI is the process of using a trained model to make predictions or decisions on new, unseen data. Unlike training, it applies learned knowledge in real-time, such as a self-driving car recognizing a stop sign it hasn’t seen before. 

# Embeddings

* A vector is a list of numbers.
* An embeddings is a vector numerical representation of a text.

### Types:
- Word embeddings: Represents the words so the words with close meanings looks almost similar(word2vec, fasttext)
- Sentence/document embeddings: Represents the whole sentence or part of text as a vector. It captures the general meaning of the text not just the meaning of words(Sentence-bert)
- Contextual embeddings: Each word has a different representation for a specific context.(Bert, GPT Embeddings)
- Others: Image embeddings, speech embeddings, graph embeddings(recomandation systems.)


1. WORD EMBEDDINGS: king = [0.82,  0.13, 0.44, -0.51]
2. SENTENCE EMBEDDINGS: I LOVE CATS = [0.41, 0.22, -0.56, 0.77, 0.13]
3. CONTEXTUAL EMBEDDING: bank = [0.10, -0.35, 0.82, 0.44, -0.12] for 'He sat by the river bank.' and bank = [-0.66, 0.91, -0.05, -0.33, 0.50] for 'She deposited money in the bank.'

# Vector databases
* Vector databases are specialized systems designed to store, index, and retrieve high-dimensional vectors, often used as embeddings that represent data like text, images, or audio.
* Unlike traditional databases that handle structured data, vector databases excel at managing unstructured data by enabling fast similarity searches, where vectors are compared to find those that are most similar to a query. 
* Vector databases use indexing techniques such as approximate nearest neighbor (ANN) search to efficiently handle large datasets, ensuring quick and accurate retrieval even at scale.
To search, it uses similarity checks. The system represents each item as a mathematical vector in an n-dimensional space. When you search for something, the query is vectorized, and the database finds the closest vectors to it.
* examples: Pinecone, Weaviate, Chroma DB

# AI Agents
## What is an AI Agent?

An **AI agent** is a system that:

- **Perceives** the environment (receives input — text, data, sensors, etc.)  
- **Decides** what actions to take (using rules, AI models, reasoning)  
- **Acts** upon the environment (executes steps, calls APIs, writes code, responds to the user)  

---

### How is it different from a simple AI model?

Unlike a basic AI model (e.g., a chatbot) that only gives responses, an **AI agent has autonomy**:  
- It can **plan tasks**  
- **Choose actions**  
- **Use external tools** to solve a problem end-to-end  

# Rag (Retrieval-Augmented Generation)

Retrieval-Augmented Generation (RAG) is an AI approach that combines information retrieval with language generation to create more accurate, contextually relevant outputs. It works by first retrieving relevant data from a knowledge base or external source, then using a language model to generate a response based on that information.

## RAG Pipeline (short version)

1. **Chunking** – Split large documents into smaller pieces.  
2. **Embedding** – Convert each chunk into a vector using an AI model.  
3. **Storage** – Save vectors + text + metadata in a vector database (e.g., Pinecone, Weaviate, Chroma).  
4. **Query** – User question is also converted into an embedding.  
5. **Retrieval** – Search the vector DB to find the most relevant chunks (top-k).  
6. **Context Assembly** – Combine retrieved chunks into a prompt.  
7. **Generation** – LLM (e.g., GPT, Llama) generates a final answer using the context.  


Why we need storage?

With a vector database, documents are embedded and stored once, and at query time only the user’s sentence is embedded and compared for fast similarity search.  

# Prompt Engineering
Prompt engineering is the process of crafting effective inputs (prompts) to guide AI models, like GPT, to generate desired outputs. It involves strategically designing prompts to optimize the model’s performance by providing clear instructions, context, and examples


