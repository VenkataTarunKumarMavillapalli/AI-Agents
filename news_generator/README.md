# AI News Generator

The AI News Generator is a web application that utilizes the power of CrewAI and Cohere's Command R7B to automatically generate comprehensive blog posts based on any topic entered by the user. With a streamlined process, the app allows users to generate, review, and download AI-generated articles in Markdown format, making it ideal for content creators, bloggers, and anyone needing quick, high-quality content generation.

---

## Features

- **Topic Input**: Enter any topic, and the app will generate a detailed article based on it.
- **Advanced Settings**: Adjust the creativity of the AI-generated content with a temperature slider.
- **Downloadable Content**: Download the generated content as a markdown file.
- **AI-Powered Workflow**: Utilizes CrewAI to split tasks between two agents:
  - **Senior Research Analyst**: Researches and gathers accurate information from reliable web sources.
  - **Content Writer**: Converts the research findings into a readable, well-organized blog post.
- **Streamlit Interface**: The app has an interactive and user-friendly interface for easy content generation.

---

## Installation

To get started, follow these steps:

## Set up Environment Variables

Ensure you have a `.env` file in the project root containing the necessary API keys or credentials for any third-party services (e.g., Cohere, CrewAI). Example:

```
COHERE_API_KEY=your-cohere-api-key
CREWAI_API_KEY=your-crewai-api-key
```
---

## Usage

1. **Enter Your Topic**: In the sidebar, enter the topic you want to generate content about in the text area.
2. **Adjust Settings**: Use the temperature slider to control the creativity of the generated content (0.0 for more factual, 1.0 for more creative).
3. **Generate Content**: Click on the "Generate Content" button to initiate the content generation process.
4. **Review & Download**: After the content is generated, it will be displayed on the main page. You can then download it as a Markdown file using the "Download Content" button.

---

## Dependencies

- **Streamlit**: For creating the web interface.
- **CrewAI**: Used for creating and managing AI agents.
- **Cohere**: For natural language processing via Cohere's Command R7B.
- **SerperDevTool**: A custom tool for searching and gathering information from web sources.
- **python-dotenv**: For loading environment variables from a `.env` file.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This README provides an overview of how to set up and use the AI News Generator, as well as the technologies used behind the scenes. Let me know if you'd like any changes or additional information!
