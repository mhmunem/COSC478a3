<!-- # COSC 478 - Assignmnet 03 -->

# RAG System for LLM (Ollama)

# Overview

This project focuses on summarizing website data using large language models (LLMs) and creating a model taht answers questions specific to the websites. 
The primary objective is to explore and implement methods for effectively summarizing the vast amount of information processed by LLMs, making it more accessible and useful for specific applications.

The project includes the following key components:
1. Web scarping: Scraping the specific websites listed in links.csv
1. Data Preprocessing: Preparing the input data for summarization, including cleaning, tokenization, and formatting.
2. Model Selection: Choosing appropriate LLMs for the summarization task, such as GPT-3, BERT, or other state-of-the-art models. For this instance the open source (Ollama)[https://ollama.com/library/llama2:7b] model have been used.
3. Summarization Techniques: Implementing different summarization techniques, including extractive and abstractive methods.
5. Applications: Demonstrating the practical applications of the summarization of the website by crating a question answering section using Gradio


The notebook summarised_LLM.ipynb likely contains code and explanations for each of these components, providing a comprehensive guide to summarizing large language models. 

## File Structure
```
├── .venv
├── .evn
├── chroma.vdb
│   ├── dbfiles ...
│   └── chroma.sqlite3
├── example.env
├── LICENSE
├── links.csv
├── README.md
├── requirements.txt
└── summarised_LLM.ipynb
```

## Files and Directories
<!-- app.py: The main application script.   -->
chroma.vdb/: Directory containing vector database files.  
<!-- 5db4487b-0cea-4c4d-9ad0-81f31386f8e6/: Subdirectory with binary data files.   -->
<!-- 87b09e2d-922a-4606-aead-766c9035c846/: Another subdirectory with binary data files.   -->
chroma.sqlite3: SQLite database file for the vector database.  
example.env: Example environment variables file.  
LICENSE: License file for the project.  
links.csv: CSV file containing links of the website to scrap.  
README.md: This README file.  
requirements.txt: List of Python dependencies required for the project.  
summarised_LLM.ipynb: Jupyter notebook for summarizing large language models.  


# Installation
- Clone the repository:
git clone https://github.com/mhmunem/cosc478a3.git

Navigate to the project directory:
cd cosc478a3

- Install the required dependencies:
run the following commands
```python
python3 -m venv .venv
. .venv/bin/activate
pip install -r requirements.txt
```
# Usage
Set up your environment variables by copying example.env to .env and modifying it as needed.
Run the main application:
python app.py

# Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

# License
This project is licensed under the terms of the LICENSE file.



(OpenGPT4.o)[https://huggingface.co/spaces/KingNish/OpenGPT-4o]