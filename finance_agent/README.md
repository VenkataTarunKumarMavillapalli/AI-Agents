## 📊 AI Finance Agent with xAI Grok

## Overview
The **xAI Finance Agent** is an AI-powered financial assistant that leverages **xAI's Grok-beta model** along with **YFinanceTools** and **DuckDuckGo** to provide insightful financial data, stock analysis, and real-time market information. The agent is deployed in an interactive user interface using the **Phi Playground** framework.

## Features
- **Stock Market Data**: Retrieves stock prices, analyst recommendations, and fundamental financial data.
- **Web Search Integration**: Uses DuckDuckGo to fetch relevant financial news and information.
- **xAI Model**: Powered by the `grok-beta` model for intelligent financial analysis.
- **Interactive UI**: Built using Phi's Playground framework for a seamless user experience.
- **Structured Data Representation**: Displays financial and numerical data in tables while presenting text-based insights in bullet points and concise paragraphs.

## Installation
To use the xAI Finance Agent, follow these steps:

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Required dependencies

## Code Breakdown
### Import Necessary Libraries
```python
from phi.agent import Agent
from phi.model.xai import xAI
from phi.tools.yfinance import YFinanceTools
from phi.tools.duckduckgo import DuckDuckGo
from phi.playground import Playground, serve_playground_app
```
These imports bring in essential libraries for:
- Creating the AI agent (`Agent`)
- Using xAI models (`xAI`)
- Fetching financial data (`YFinanceTools`)
- Conducting web searches (`DuckDuckGo`)
- Setting up the user interface (`Playground` and `serve_playground_app`)

### Define the AI Finance Agent
```python
agent = Agent(
    name="xAI Finance Agent",
    model = xAI(id="grok-beta"),
    tools=[DuckDuckGo(), YFinanceTools(stock_price=True, analyst_recommendations=True, stock_fundamentals=True)],
    instructions = ["Always use tables to display financial/numerical data. For text data use bullet points and small paragraphs."],
    show_tool_calls = True,
    markdown = True,
)
```
- **Name**: Sets the agent's name to `xAI Finance Agent`.
- **Model**: Uses `grok-beta`, a powerful xAI model.
- **Tools**: Integrates **DuckDuckGo** for web searches and **YFinanceTools** for stock market data.
- **Instructions**: Defines guidelines for data formatting.
- **Markdown Support**: Ensures rich text formatting.

### Configure the UI
```python
app = Playground(agents=[agent]).get_app()
```
This initializes the **Phi Playground UI** with the finance agent.

### Launch the Application
```python
if __name__ == "__main__":
    serve_playground_app("xai_finance_agent:app", reload=True)
```
- Runs the application using `serve_playground_app`.
- Enables hot-reloading for live updates.

## Acknowledgments
Special thanks to the **Phi** team for providing the framework that powers this project.

## Contact
For any questions or feedback, feel free to reach out:
- [**LinkedIn**](https://www.linkedin.com/in/venkata-tarun-kumar-mavillapalli-967b4613a/)













