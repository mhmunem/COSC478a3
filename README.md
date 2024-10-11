# Retrieval Augmented Generation (RAG) Architecture for LLM (Ollama)

Retrieval Augmented Generation (RAG) enhances LLMs by retrieving relevant data and using it as augmented context, enabling static LLMs to access real-time information. This approach improves the accuracy of chatbot answers, making them more precise by incorporating company documents and knowledge bases. Ideal for customer support and lead follow-up.

## Key Components
1. Web Scraping: Scraping specific websites listed in links.csv. This file can also include other organizational data such as purchase history.

2. Data Preprocessing: Preparing the input data, including cleaning, tokenization, and formatting.

3. Model Selection: Choosing appropriate LLMs, such as GPT-3, BERT, or Llama2.

4. Applications: Demonstrating practical applications by creating a question-answering section using Gradio.

The notebook `RAG_Chatbot.ipynb` provides detailed code and explanations for these components.

## File Structure
```
├── .venv
├── .evn
├── chroma.vdb
│   ├── extra dbfiles ...
│   └── chroma.sqlite3
├── example.env
├── LICENSE
├── links.csv
├── README.md
├── requirements.txt
└── RAG_Chatbot.ipynb
```

## Files and Directories
chroma.vdb/: Directory containing vector database files.  
chroma.sqlite3: SQLite database file for the vector database.  
example.env: Example environment variables file.  
LICENSE: License file for the project.  
links.csv: CSV file containing links of the website to scrap.  
README.md: This README file.  
requirements.txt: List of Python dependencies required for the project.  
`RAG_Chatbot.ipynb`: Jupyter notebook for summarizing large language models.  


# Installation
- Clone the repository:
```bash
git clone https://github.com/mhmunem/cosc478a3.git
cd cosc478a3
```
- Set up the environment and install the required dependencies:
```bash
python3 -m venv .venv
. .venv/bin/activate
pip install -r requirements.txt
```
# Usage
Set up the Pinecone vector database. Sign up for Pinecone, create an index, and add the API key to the .env file. Set up your environment variables by copying example.env to .env and modifying as needed.

# Contribution
Contributions are welcome! Please fork the repository and submit a pull request.