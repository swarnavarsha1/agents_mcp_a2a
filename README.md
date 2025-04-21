# MCP Chat Agent with Memory

## 🛠 Setup Instructions

### 1. Create and activate a virtual environment

```bash
uv venv
.venv/Scripts/Activate   # For Windows
# source .venv/bin/activate  # For macOS/Linux
```

### 2. Install dependencies

```bash
uv add langchain_openai
uv add mcp-use
uv pip install mcp-use
```

### 3. Add your OpenAI API key

Create a `.env` file in the root of your project:

```
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

> ✅ Ensure this file is added to `.gitignore` to avoid committing secrets.

### 4. Configure your MCP servers

Add or modify the `tools.json`(if needed to add new tools) file to define your MCP-compatible servers (example included):


## 🚀 Running the App

Start the chat application:

```bash
uv run app.py
```

### Features

- Built-in conversation memory for more natural interactions
- `exit` or `quit` to end the chat
- `clear` to reset memory
