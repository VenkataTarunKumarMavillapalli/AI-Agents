## 💻 Web Scrapping AI Agent
This Streamlit app allows you to scrape a website using OpenAI API and the scrapegraphai library. Simply provide your OpenAI API key, enter the URL of the website you want to scrape, and specify what you want the AI agent to extract from the website.

### Features
- Scrape any website by providing the URL
- Utilize OpenAI's LLMs (GPT-3.5-turbo or GPT-4) for intelligent scraping
- Customize the scraping task by specifying what you want the AI agent to extract

### How it Works?

- The app prompts you to enter your OpenAI API key, which is used to authenticate and access the OpenAI language models.
- You can select the desired language model (GPT-3.5-turbo or GPT-4) for the scraping task.
- Enter the URL of the website you want to scrape in the provided text input field.
- Specify what you want the AI agent to extract from the website by entering a user prompt.
- The app creates a SmartScraperGraph object using the provided URL, user prompt, and OpenAI configuration.
- The SmartScraperGraph object scrapes the website and extracts the requested information using the specified language model.
- The scraped results are displayed in the app for you to view
