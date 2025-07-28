# Langchain
`LangChain is like LEGO blocks for building apps with chatbots or large language models.`

* It's a python and js framework that help developer build applications powered by LLMs.

## Core concepts:
* LLMs – The brain.
* Chains – Sequences of steps, like a recipe for reasoning.
* Agents – Smart bots that can choose what to do next using tools.
* Tools – External things agents can use (search, code interpreter, calculator).
* Memory – For retaining conversation history.


# Rag
`RAG is like giving your chatbot a smart notebook it can read from, but it doesn’t memorize the whole thing.`
* RAG = Retrieval-Augmented Generation
- Is a python library
* It solves a key problem: LLMs forget things they weren’t trained on.
* Instead of training the model again, RAG fetches the right info at query time from external sources (like PDFs, databases, websites).

## How it works?
1. You ask a question
2. A retriever finds the most relevant chunks of knowledge from documents.
3. Those chunks are fed into the LLM along with your question.
4. The LLM uses both to generate an answer.