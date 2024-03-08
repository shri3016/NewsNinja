
# NewsNinja: News Research Tool 

NewsNinja is an easy-to-use news Research tool developed for hassle-free data retrieval. Users can enter URLs of articles and ask questions gather meaningful insights from the financial and stock market domains.

![](NewsNinja.jpg)

# Tools/Technologies Used:
This project involves implementing an end-to-end solution using **Large Language Models (LLM)** and **Natural Language Processing (NLP)** techniques like:

- Langchain

- OpenAI API

- FAISS

- Streamlit

## Features

- Load URLs or upload text files that contain URLs to extract article content.
- Utilize LangChain's UnstructuredURL Loader to process article content.
- Generate an embedding vector utilizing OpenAI's embeddings and utilize FAISS, a robust similarity search library, to facilitate rapid and efficient retrieval of pertinent information.
- Engage with the LLM's by inputting queries and receiving answers alongside source URLs.


## Installation

1. You can clone this repository to your local machine using:

```bash
  git clone <repository_url>
```

2. To install the required dependencies using pip use the following command:

```bash
  pip install -r requirements.txt
```
4.You can enter your OpenAI API key in the .env file:

```bash
  OPENAI_API_KEY=your_api_key_here
```
## Usage

1. To run the Streamlit app use:
```bash
streamlit run main.py

```

2. The web app will open in your browser.

-  You can enter URLs directly on the sidebar.

-  You can start the data loading and processing by clicking "Process URLs."

-  You can watch the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.

-  The embeddings will be stored and indexed using FAISS, improving retrieval speed.

-  The FAISS index will be stored in your local file path in pickle format.

-  You can now ask a question to the NewsNinja and get the answer based on the news article urls you entered.

- In the screenshot, I used following news articles:
  - https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html
  - https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html
  - https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html

## Project Directory Structure

- main.py: The main application script of Streamlit.
- requirements.txt: Python packages required for the project.
- faiss_store_openai.pkl: A pickle file which stores the FAISS index.
- .env: Configuration file which will store your OpenAI API key.
