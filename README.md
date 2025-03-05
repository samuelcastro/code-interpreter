# LangChain Code Interpreter

A Python project that leverages LangChain and OpenAI's models to create intelligent agents capable of interpreting and executing code to answer questions.

## Overview

This project demonstrates the power of AI agents that can:

- Write and execute Python code to solve problems
- Analyze CSV data using pandas
- Generate files (like QR codes) based on natural language instructions
- Chain multiple specialized agents together for complex tasks

## Features

- **Python REPL Agent**: Converts natural language to Python code and executes it
- **CSV Agent**: Analyzes CSV data using pandas to answer questions
- **Grand Agent**: Orchestrates the specialized agents to handle complex queries

## Project Structure

- `main.py`: Core application logic and agent definitions
- `episode_info.csv`: Sample dataset for CSV agent demonstrations
- `.env`: Environment variables for API keys (not tracked in git)

## Requirements

This project uses Pipenv for dependency management. Key dependencies include:

- langchain
- langchain_openai
- langchain_experimental
- python-dotenv
- pandas

## Setup

1. Clone this repository
2. Install dependencies:
   ```
   pipenv install
   ```
3. Create a `.env` file with your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

## Usage

Run the main script:

```bash
python main.py
```

The default example generates a QR code pointing to https://samsilvas.com and saves it to the current directory.

## Examples

The project demonstrates several capabilities:

1. **Code Generation & Execution**:

   - The Python agent can write and execute code based on natural language instructions

2. **Data Analysis**:

   - The CSV agent can analyze the episode_info.csv file to answer questions like "Print the seasons by ascending order of the number of episodes they have"

3. **File Generation**:
   - The agents can generate files like QR codes based on instructions

## License

[MIT License](LICENSE)

## Author

Samuel Silva
