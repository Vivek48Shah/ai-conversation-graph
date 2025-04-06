# Chatbot with Memory and External Summary using LangGraph



This project demonstrates a **stateful chatbot** built with `LangGraph`, designed to persist conversations, summarize interactions, and route dynamically based on context. It showcases how to structure conversational flows using a graph-based approach and persistent memory.

---
 ## What is Persistent Memory?

Normally, when you run a chatbot and stop it (or close your notebook), it forgets everything — like a whiteboard getting wiped clean.

But with persistent memory, we save the chatbot’s brain — like writing on a notebook instead of a whiteboard.

In this project, we use SQLite, a tiny built-in database, to save:
	•	The full chat history
	•	Summaries
	•	State of the conversation

So even if you stop and restart the chatbot later, it remembers where things left off — no need to start the chat from scratch!



---

##  Tech Stack

- **LangGraph** – Graph-based LLM workflow orchestration  
- **OpenAI API** – For chat response and summarization  
- **SQLite** – Persistent local memory for conversation state  

---

##  High-Level Architecture

The chatbot is defined as a **stateful graph**, where each node represents a stage in the conversation, and edges define transitions based on logic or user input.






