# AI Web Scraper

This project is a web scraping application that uses **Selenium**, **BeautifulSoup**, and **LangChain** to scrape and analyze the content of web pages. The app is built with **Streamlit** for a user-friendly interface, allowing users to scrape websites and extract specific information using the **Ollama** language model.

## Features

- **Web Scraping**: Users can enter a URL, and the app will scrape the website's content using Selenium.
- **DOM Content Extraction**: The application extracts and cleans the body content of the web page using BeautifulSoup.
- **Content Parsing**: Users can describe specific information they want to extract from the page, and the app will use LangChain with the Ollama language model to parse the content and provide relevant results.
- **Interactive UI**: Built with Streamlit, offering an easy-to-use interface for web scraping and content parsing.

## Installation

### Prerequisites

- Python 3.8+
- [Streamlit](https://streamlit.io/)
- [Selenium](https://www.selenium.dev/)
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- [LangChain](https://langchain.com/)
- Chrome WebDriver (for Selenium)
- Ollama language model

### Environment Variables

Create a `.env` file in the project root and define the following environment variable:

```
SBR_WEBDRIVER=<your_webdriver_url>
```

### Setup

1. Clone this repository:

   ```bash
   git clone <repo-url>
   cd <project-folder>
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Streamlit app:

   ```bash
   streamlit run main.py
   ```

## Usage

1. **Scraping a Website**:

   - Enter the URL of the website you want to scrape.
   - Click on the **Scrape Website** button.
   - The app will display the scraped DOM content in an expandable text box.

2. **Parsing the Content**:
   - After scraping, enter a description of what information you want to extract.
   - Click on **Parse Content**, and the app will return the parsed information.

## File Structure

- `main.py`: Contains the Streamlit UI and handles the workflow for scraping and parsing content.
- `scrape.py`: Handles the web scraping process using Selenium and extracts/cleans the DOM content with BeautifulSoup.
- `parse.py`: Uses LangChain and the Ollama language model to parse the DOM content based on user input.

## Dependencies

- `streamlit`
- `selenium`
- `beautifulsoup4`
- `langchain`
- `dotenv`

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
