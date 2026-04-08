# 🤖 WASM Agent

Browser-based AI Assistant powered by Python WebAssembly.

## Features

- ✅ **Python WASM Runtime** - Full Python 3.11 in browser
- ✅ **Virtual File System** - Create, read, and manage files
- ✅ **Code Execution** - Run Python code directly
- ✅ **Multi-Provider Support** - OpenAI, Anthropic, or Local mode
- ✅ **Tool Logging** - See agent actions in real-time

## Quick Start

1. Open the website
2. Select provider (OpenAI/Anthropic/Local)
3. Enter API key (for API modes)
4. Start chatting!

## Tools

| Tool | Description |
|------|-------------|
| `write_file` | Write content to virtual file |
| `read_file` | Read file content |
| `list_files` | List all files |
| `run_python` | Execute Python code |

## Example Prompts

- "Write a Python function to calculate fibonacci"
- "Create a file called hello.txt"
- "List all files"
- "Help me debug this code"

## Architecture

```
Browser
    ↓
Pyodide (Python WASM)
    ↓
Agent Loop
    ↓
Tool Execution
```

## Local Development

```bash
# Clone
git clone https://github.com/agihub-source/wasm-agent.git

# Serve
python -m http.server 8000
# or
npx serve .
```

## License

MIT