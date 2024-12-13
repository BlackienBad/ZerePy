# ZerePy

We're building ZerePy, an open-source Python framework designed to let you deploy your own agents on X, powered by 
OpenAI or Anthropic LLMs.

ZerePy is built from a modularized version of the Zerebro backend. With ZerePy, you can launch your own agent with 
similar core functionality as Zerebro. For creative outputs, you'll need to fine-tune your own model.

## Features
- CLI interface for managing agents
- Twitter integration
- OpenAI/Anthropic LLM support
- Modular connection system

## Installation

This project uses Poetry for dependency management. Here's how to get started:

1. First, install Poetry if you haven't already:
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

2. Clone the repository:
```bash
git clone https://github.com/blorm-network/ZerePy.git
cd ZerePy
```

3. Install dependencies:
```bash
poetry install --no-root
```

This will create a virtual environment and install all required dependencies.

## Requirements

- Python 3.10 or higher
- Poetry 1.5 or higher

## Usage

1. Activate the virtual environment:
```bash
poetry shell
```

2. Run the application:
```bash
poetry run python main.py
```

## Getting Started

1. Fork this template
2. Install dependencies by clicking Run
3. Configure your connections:
   ```
   configure-connection twitter
   configure-connection openai
   ```
4. Load the example agent:
   ```
   load-agent example
   ```
5. Start your agent:
   ```
   agent-loop
   ```
## Creating Your Own Agent

Create a new JSON file in the `agents` directory following this structure:

```json
{
  "name": "YourAgent",
  "model": "gpt-3.5-turbo",
  "bio": "Your agent's description",
  "moderated": true
}
```

---
Made with ♥ @Blorm.xyz
