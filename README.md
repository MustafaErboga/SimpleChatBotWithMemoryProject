# Simple Chatbot with Memory

A minimal **terminal-based chatbot** application using LangChain, OpenAI, and in-memory message history. It remembers previous messages within a session to enable more coherent and context-aware conversations.

## Features

- Conversational chatbot powered by OpenAI's GPT model  
- **Terminal interface** for simple and fast interaction  
- Remembers chat history using `InMemoryChatMessageHistory`  
- Supports session-based memory with `RunnableWithMessageHistory`  
- Secure API key management with `python-dotenv`

## Prerequisites

- Python 3.8+  
- **OpenAI API Key**  
- **LangChain API Key**

## Quick Start

### 1. Clone the repository:

```bash
git clone <your_github_repo_url>
cd simplechatbotwithmemory
```

### 2. Set up the environment and install dependencies:

```bash
python -m venv .venv
# Activate virtual environment
# On Windows:
.venv\Scripts\activate
# On macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
```

### 3. Configure API Keys:

- Copy `.env.example` to `.env`
- Add your API keys:

```env
OPENAI_API_KEY="your-openai-api-key"
LANGCHAIN_API_KEY="your-langchain-api-key"
```

### 4. Run the chatbot:

```bash
python app.py
```

### 5. Start chatting in your terminal:

```bash
> Hello!
Chatbot: Hi there! How can I assist you today?
```

## Key Files

- `app.py`: Main script for running the chatbot in the terminal  
- `.env`: Stores your OpenAI and LangChain API keys (not committed)  
- `.env.example`: Template for environment variables  
- `requirements.txt`: Python dependencies  
- `.gitignore`: Ignores sensitive/local files like `.env` and `.venv/`
