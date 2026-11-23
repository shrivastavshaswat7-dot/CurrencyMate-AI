# CurrencyMate AI 💱

A beginner-friendly currency conversion assistant built using **LangChain, Groq LLM, and ExchangeRate-API**.

## Overview

CurrencyMate AI is a hands-on learning project that demonstrates how an LLM can use external tools to perform real-world tasks such as fetching exchange rates and converting currencies.

## Features

- Fetch exchange rates between currencies.
- Convert currency amounts.
- LLM-based tool selection.
- Natural language responses.
- Handles general questions without unnecessary tool calls.

## Tech Stack

- Python
- Google Colab
- LangChain
- Groq LLM (`openai/gpt-oss-20b`)
- ExchangeRate-API
- Requests

## LangChain Concepts Practiced

- Custom tools using `@tool`
- Toolkits
- Tool binding using `bind_tools()`
- LLM tool calling
- Tool execution using `.invoke()`
- Tool results using `ToolMessage`
- Reusable application workflow

## Project Workflow

1. User submits a query.
2. LLM decides whether a tool is required.
3. LLM generates a tool-call request.
4. Python executes the selected tool.
5. Tool result is returned to the LLM.
6. LLM generates the final response.

## Setup

1. Open the notebook in Google Colab.
2. Install the required dependencies:

   ```bash
   pip install langchain langchain-groq requests
   ```

3. Add the following secrets in Google Colab:

   - `GROQ_API_KEY`
   - `EXCHANGE_RATE_API_KEY`

4. Run the notebook cells sequentially.

## Limitations

- Basic error handling.
- Supports one tool call per request.
- Uses an external exchange-rate API.
- Built for educational purposes, not financial decisions.

## Learning Goal

The main goal of this project was to understand how LLMs interact with custom Python tools using LangChain.

---

**Status:** Completed — Beginner-level learning project.
