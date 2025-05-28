# AI Research Assistant Agent

This project is an AI-powered research assistant that leverages large language models and web tools to help generate research papers, summaries, and source lists for any topic. It uses LangChain, Google Gemini, DuckDuckGo, and Wikipedia APIs to gather and process information.

## Features
- **Automated Research**: Answers user queries and generates structured research responses.
- **Web Search Integration**: Uses DuckDuckGo and Wikipedia to find up-to-date and relevant information.
- **Output Saving**: Saves research outputs to a timestamped text file (`research_output.txt`).
- **Extensible Tools**: Easily add more tools for additional data sources or actions.

## How It Works
1. The user enters a research question.
2. The agent uses LLMs and web tools to gather and summarize information.
3. The response is parsed into a structured format and printed.
4. The output is saved to `research_output.txt` with a timestamp.

## Requirements
- Python 3.8+
- API keys for Google Gemini and any other LLMs you wish to use

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
1. Set up your environment variables (e.g., API keys) in a `.env` file.
2. Run the main script:
```bash
python main.py
```
3. Enter your research question when prompted.
4. The answer will be printed and saved to `research_output.txt`.

## File Overview
- `main.py`: Main entry point, agent setup, and execution logic.
- `tools.py`: Custom tools for web search, Wikipedia, and saving output.
- `research_output.txt`: Stores all research outputs with timestamps.
- `requirements.txt`: Python dependencies.

## Example
```
How can I help you? What is the impact of climate change on polar bear populations?
# Output (printed and saved):
ResearchResponse(topic='Climate Change and Polar Bears', summary='...', sources=['...'], tools_used=['search', 'wiki'])
```

## License
MIT License
