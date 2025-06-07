# MCP Web Automation Agent

A powerful AI-driven web automation agent that lets users control browser actions using natural language commands. Built with **Streamlit**, **OpenAI**, and **Puppeteer**.

## Features

- Parse and execute web automation instructions using LLMs
- Dynamic command interpretation (e.g., "Search for flights to New York")
- Interface built with Streamlit for easy interaction
- Headless browser automation powered by Puppeteer

## Tech Stack

- **Python 3.9+** – Application logic and LLM integration
- **Streamlit** – Frontend UI for user interaction
- **OpenAI API** – Natural language understanding and command generation
- **Node.js + Puppeteer** – Browser automation layer
- **YAML** – Configuration management
- **Logging** – Local logging for troubleshooting and audit

## How It Works

1. **User Input**: A natural language instruction is provided through the Streamlit interface.
2. **LLM Parsing**: The input is processed using OpenAI's API to generate a structured response.
3. **Browser Automation**: The agent sends this structured command to a Puppeteer-powered backend to simulate browser activity.

## Project Structure

```
MCP--WebAutomation-Agent/
│
├── main.py                  # Core logic and Streamlit interface
├── requirements.txt         # Required Python packages
├── mcp_agent.config.yaml    # Configurations for the agent
└── logs/                    # Runtime logs
```

## Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/rijul21/MCP--WebAutomation-Agent.git
   cd MCP--WebAutomation-Agent
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the app:
   ```bash
   streamlit run main.py
   ```

## Requirements

- Python 3.9+
- Node.js (for Puppeteer)
- OpenAI API Key

## Notes

- Puppeteer should be configured separately to interact with the automation commands.
- All outputs and errors are logged under the `logs/` directory.

## License

This project is licensed under the MIT License.
