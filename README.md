# Career Pages Watchdog

## Overview

Career Pages Watchdog is a tool designed to monitor company career pages and extract job-related information. It uses a combination of web scraping and AI language models to automatically detect career pages and count published jobs.

## Components

The system consists of two main components:

1. **Career Pages Extractor**: Uses Selenium and LLMs to automatically detect a company's career page URL where job listings can be found.
2. **Job Count Extractor**: Estimates the number of jobs published on a given career page.

## Setup

### Prerequisites

- Python 3.8+
- Chrome/Chromium browser
- Ollama (for local LLM deployment)
- OpenAI API key (for GPT model access)
- Poetry (for dependency management)

### Installation

1. Clone the repository:
   ```bash
   git clone [repository-url]
   cd careerPagesWatchdog
   ```

2. Install and configure Poetry:
   ```bash
   # Install Poetry using Homebrew
   brew install poetry

   # Alternatively, install using the official installer
   curl -sSL https://install.python-poetry.org | python3 -

   # Initialize a new Poetry project (if starting from scratch)
   poetry init

   # Install project dependencies
   poetry install
   
   # Activate the virtual environment
   poetry shell
   ```

3. Create a `.env` file with your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

4. Start Ollama service for local LLM support:
   ```bash
   ollama serve
   ```

## Usage

The project includes a Jupyter notebook (`notebook.ipynb`) for development and testing. You can use it to:

- Test career page extraction for individual companies
- Process lists of companies from CSV files
- Compare results between different LLM models (Qwen, Llama, GPT)

## License

This project is property of Xing and authored by Eduardo Escartí and shall not be copied.
