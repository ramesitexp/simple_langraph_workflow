# Agent From Scratch

A Python project exploring the fundamentals of building AI agents from scratch using [LangGraph](https://python.langchain.com/docs/langgraph) and [LangChain](https://python.langchain.com/docs/get_started/introduction). 

## Project Overview

This project is set up using `uv` for modern, fast dependency management. It contains experimental Jupyter Notebooks demonstrating various LLM workflows and state graphs.

### Current Experiments
- **`simple_llm_workflow.ipynb`**: Demonstrates a basic LangGraph `StateGraph` implementation. It uses a single node to handle question-answering with a stateless Language Model. The example utilizes the `ChatOpenAI` interface to connect to Groq's high-speed API.
- **`sentiment_review_reply_workflow.ipynb`**: (Work in Progress)

## Setup & Installation

This project uses `uv` for environment management. 

1. Ensure you have [uv](https://github.com/astral-sh/uv) installed.
2. Clone the repository:
   ```bash
   git clone https://github.com/ramesitexp/simple_langraph_workflow.git
   cd simple_langraph_workflow
   ```
3. Sync the dependencies and create the virtual environment:
   ```bash
   uv sync
   ```
4. Configure your environment variables:
   Create a `.env` file in the root directory and add your API key (the simple workflow uses Groq):
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

## Dependencies
- `langgraph`
- `langchain-openai`
- `python-dotenv`
- `ipykernel`

*Requires Python >= 3.14*
