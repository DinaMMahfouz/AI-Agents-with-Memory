# AI Agents with Memory

This project demonstrates how to build AI agents with memory using Python, Ollama, the OpenAI Agents SDK, and SQLiteSession.

The notebook compares two approaches:

1. Running an AI agent without memory.
2. Running an AI agent with session-based memory.

The goal is to show how an AI agent can remember previous user inputs and use that context in follow-up questions.

---

## Project Overview

This project includes examples of AI agents that can respond to user input and maintain conversation context.

The main examples are:

- A Finance Advisor Agent that analyzes spending.
- A Wellness Coach Agent that suggests weekly health habits.
- A memory-enabled conversation using SQLiteSession.
- A comparison between stateless and memory-enabled agent behavior.

---

## Technologies Used

- Python
- Jupyter Notebook
- Google Colab
- Ollama
- Llama 3.2
- OpenAI Agents SDK
- SQLiteSession
- AsyncOpenAI

---

## Main Features

- Create AI agents with custom instructions.
- Run agents using a local Ollama model.
- Use an OpenAI-compatible client with Ollama.
- Add memory to conversations using SQLiteSession.
- Compare responses with and without memory.
- Test follow-up questions that depend on earlier conversation context.

---

## Project Files

```text
AI_Agents_with_Memory.ipynb   # Main notebook for the project
README.md                    # Project documentation
.gitignore                   # Files and folders ignored by Git
```

---

## How the Project Works

The notebook starts by configuring the model through Ollama.

Then, it creates an AI agent and runs user questions through it.

Without memory, the agent treats each question as a new conversation.

With SQLiteSession, the agent remembers previous messages in the same session and uses them to answer follow-up questions more accurately.

Example:

```text
User: I spent $120 on groceries, $40 on Uber, and $60 on restaurants this week.
```

Follow-up question:

```text
User: My weekly budget is $250. Based on everything I told you so far, where can I cut spending next week?
```

With memory enabled, the agent can use the earlier spending details to provide a more useful answer.

---

## Example Use Cases

This project can be useful for building:

- Personal finance assistants
- Wellness coaching assistants
- AI chatbots with memory
- Customer support assistants
- Local AI workflows using Ollama
- AI agents that need to remember conversation context

---

## Security Note

This project uses Ollama locally and does not require a real OpenAI API key for the main implementation.

The value below is only a placeholder used for the Ollama-compatible client setup:

```python
api_key="ollama"
```

Do not upload real API keys, passwords, tokens, customer data, or private information to GitHub.

---

## How to Run

1. Clone this repository or download the notebook.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Install the required libraries.
4. Start the Ollama server.
5. Pull the required model, such as Llama 3.2.
6. Run the notebook cells step by step.
7. Test the agent with and without memory.

---

## What I Learned

Through this project, I practiced:

- Creating AI agents using Python.
- Connecting agents to a local LLM through Ollama.
- Using SQLiteSession for conversation memory.
- Understanding the difference between stateless and memory-enabled agents.
- Writing structured agent instructions.
- Building practical AI workflows.

---

## Future Improvements

Possible future improvements include:

- Add a Streamlit web interface.
- Store finance data in a structured database.
- Add charts for spending analysis.
- Add more agent examples.
- Improve error handling.
- Convert the notebook into a Python application.
- Add a `requirements.txt` file for easier setup.

---

## Author

**Dina Mahfouz**

Technical Support Engineer interested in AI, automation, cloud, identity, and practical AI agents.
