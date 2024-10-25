# Search-Agent

Search-Agent is a conversational agent that can perform web searches and answer questions about the weather using Langchain and various language models. This repository contains two main components: 

- `main.py`: Implements a state graph that interacts with an agent to get weather updates.
- `search_agent.py`: Uses a Tavily search tool to answer questions.

## Features

- Conversational interface to retrieve weather information.
- Integration with the Tavily API for enhanced search capabilities.

## Prerequisites

Before running the application, ensure you have the following:

- Python 3.8 or higher
- Poetry for dependency management
- Required API keys (see below)

## API Keys Required

1. **Tavily API Key**: This key is needed for the Tavily search results tool. You can obtain it by signing up at [Tavily](https://www.tavily.com).

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/Search-Agent.git
   cd Search-Agent
   ```

2. **Install Poetry**:
   If you haven't already installed Poetry, follow the installation instructions on the [official website](https://python-poetry.org/docs/#installation).

3. **Install dependencies**:
   Run the following command in the project directory:
   ```bash
   poetry install
   ```

## Setting Up Environment Variables

Create a `.env` file in the project root directory with the following content:

```env
TAVILY_API_KEY=your_tavily_api_key_here
```

Replace `your_tavily_api_key_here` with your actual Tavily API key.

## Running the Application

### Running `main.py`

To execute the weather agent using `main.py`, run the following command:

```bash
poetry run python src/main.py
```

This will initiate the agent, and you should see outputs indicating the weather in San Francisco and New York.

### Running `search_agent.py`

To use the Tavily search functionality in `search_agent.py`, run:

```bash
poetry run python src/search_agent.py
```

You will see a conversational exchange in the console, with the agent responding to predefined messages.

## Project Structure

- `main.py`: Contains the main logic for the weather agent using state graphs and the ChatAnthropic model.
- `search_agent.py`: Implements a conversational agent that streams responses based on user input using Tavily for searches.

## Contributing

If you'd like to contribute to this project, please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Langchain](https://langchain.com/): For providing the tools and framework used in this project.
- [Tavily](https://www.tavily.com): For the search results API.
