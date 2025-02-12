# LangChain Web Scraper Agent

## Overview
This project is a LangChain-based intelligent agent that can scrape web content, store it in a vector database, and provide answers to user queries. It uses ChromaDB for vector storage and Google's Gemini API for generating responses.

## Features
- Scrapes web pages using BeautifulSoup
- Stores extracted text embeddings in ChromaDB
- Uses LangChain for query processing
- Integrates Google Gemini API for intelligent responses
- Implements a retrieval-augmented generation (RAG) pipeline

## Installation
### Prerequisites
Ensure you have Python 3.8+ installed. Then, install the required dependencies:
```bash
pip install -r requirements.txt
```

### Required Dependencies
```bash
pip install langchain-google-genai beautifulsoup4 chromadb selenium webdriver_manager requests nest_asyncio langchain-community
```

## Usage
1. Replace `Google_api_key` in the code with your Gemini API key.
2. Run the script to scrape a given website and store content in the vector database.
3. Use the agent to ask queries related to the website's content.

## Example
```python
scraper = WebScraper()
data = scraper.scrape_website("https://example.com")
response = query_agent("What is the main topic of the website?")
print(response)
```

## Contributing
Feel free to fork this repository and submit pull requests.


