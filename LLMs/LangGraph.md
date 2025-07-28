# LangGraph

`LangGraph is like LangChain, but for building flexible AI workflows that act like a flowchart or a state machine.`

## LangGraph is:
* A library built on top of LangChain.
* Lets you define multi-step, branching, stateful workflows for LLMs using a graph-based structure.

## What Can LangGraph Do?

### Imagine building a chatbot like this:
* User asks a question.
* LangGraph decides: Is this a math question, a document lookup, or a joke?
* It routes the flow to the right “node” (tool or logic).
* It keeps conversation state between turns.
* It loops or ends based on LLM output.