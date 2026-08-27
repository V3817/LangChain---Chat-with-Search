 LangChain - Chat with Search

## Overview

This project demonstrates an interactive chatbot built using **Streamlit** and **LangChain**. The chatbot is capable of performing searches on Arxiv, Wikipedia, and DuckDuckGo to provide users with accurate and concise responses. It leverages the `StreamlitCallbackHandler` to visualize the agent's thoughts and actions in real-time.

## Features

- **Web Search**: Query DuckDuckGo for general web information.
- **Arxiv API Integration**: Retrieve academic papers with summaries.
- **Wikipedia API Integration**: Extract summarized information from Wikipedia.
- **Real-Time Interaction**: Display chat interactions dynamically using Streamlit.

## How It Works

1. Users interact with the chatbot by entering queries.
2. The chatbot processes queries and utilizes integrated tools (Arxiv, Wikipedia, DuckDuckGo) for responses.
3. Results and the agent's internal thought process are displayed in the Streamlit interface.

## Setup Instructions

1. Clone this repository.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your environment variables in a `.env` file:
   ```env
   GROQ_API_KEY=<your_groq_api_key>
   ```
4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## Usage

- **API Key**: Enter your Groq API key in the sidebar settings.
- **Chat Interaction**: Ask questions or request information, e.g., *"What is machine learning?"*.
- **Dynamic Responses**: View real-time responses along with insights into the agent's decision-making process.

## Dependencies

- [Streamlit](https://streamlit.io/)
- [LangChain](https://langchain.com/)
- [Arxiv API](https://arxiv.org/help/api/index)
- [Wikipedia API](https://www.mediawiki.org/wiki/API:Main_page)
- [DuckDuckGo Search](https://duckduckgo.com)

## Example Query

```text
What is the latest research on deep learning?
```

The chatbot will fetch a concise summary from Arxiv, Wikipedia, and DuckDuckGo.

