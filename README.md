# Building-Agentic-AI-Systems-Second-Edition
Building Agentic AI Systems, Second Edition, Published by Packt

## Setup

This project uses `uv` for package management to ensure reproducible environments.

### Installing uv

If you don't have `uv` installed:

```bash
# macOS/Linux
curl -LsSf https://astral.sh/uv/install.sh | sh

# Windows
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### Setting up the Environment

```bash
# Navigate to this directory
cd code/chapter-01

# Create a virtual environment and install dependencies
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install required packages
uv add -r requirements.txt
```

## Environment Variables

Create a `.env` file in this directory with your API keys:

```
OPENAI_API_KEY=your_openai_api_key_here
ANTHROPIC_API_KEY=your_anthropic_api_key_here  # Optional, for Anthropic examples
```

## Running the Notebooks

```bash
# Install Jupyter if not already installed
uv add jupyter

# Launch Jupyter
jupyter notebook chapter_01_foundations.ipynb
```