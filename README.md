# Bot-A-News-Research-Tool🤖

Bot is a user-friendly news research tool designed for effortless information retrieval. Users can input article URLs and ask questions to receive relevant insights from the stock market and financial domain.

<img width="725" alt="researchtool" src="https://github.com/user-attachments/assets/96f3bc13-cd2f-40ec-bf63-b1ef1a334ac5" />




# 🚀 Features....
1) Load URLs or upload text files containing URLs to fetch article content.
2) Process article content through LangChain's UnstructuredURL Loader
3) Construct an embedding vector using OpenAI's embeddings and leverage FAISS, a powerful similarity search library, to
   enable swift and effective retrieval of relevant information
4) Interact with the LLM's (Chatgpt) by inputting queries and receiving answers along with source URLs.


# 🧠 Usage/Examples

## Run the Streamlit app by executing:

-> streamlit run main.py

## 🛠️The web app will open in your browser.

-> On the sidebar, you can input URLs directly.

-> Initiate the data loading and processing by clicking "Process URLs."

-> Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.

-> The embeddings will be stored and indexed using FAISS, enhancing retrieval speed.

-> The FAISS index will be saved in a local file path in pickle format for future use.

-> One can now ask a question and get the answer based on those news articles

## we used following news articles

1) https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html

2) https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html

3) https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html

# Project Structure
main.py: The main Streamlit application script.
requirements.txt: A list of required Python packages for the project.
faiss_store_openai.pkl: A pickle file to store the FAISS index.
.env: Configuration file for storing your OpenAI API key.
