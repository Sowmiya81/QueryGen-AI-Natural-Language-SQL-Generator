# QueryGen AI: Natural Language SQL Generator

This repository showcases an end-to-end solution for interacting with a MySQL database using natural language queries. Built on top of Google Palm and Langchain, the system translates user-provided questions into SQL queries, executes them on a MySQL database, and returns the results.

# Key Features
1. Natural Language Processing (NLP): Google Palm powers the language model to interpret natural language inputs.
2. SQL Query Generation: The system automatically generates and runs SQL queries based on user input.
3. Hugging Face Embeddings: Enhances the understanding of natural language queries.
4. Langchain Integration: Manages the query-building process from input to execution.
5. Streamlit UI: A user-friendly interface for query submission and result display.
6. ChromaDB: Used for vector storage to support efficient query processing.
7. Few-shot Learning: To fine-tune the LLM for better accuracy.
   
# Installation Steps
1. Clone the repository:
git clone https://github.com/Sowmiya81/QueryGen-AI-Natural-Language-SQL-Generator.git
2. Navigate to the project directory:
cd QueryGen-AI-Natural-Language-SQL-Generator
3. Install the necessary dependencies:
pip install -r requirements.txt
4. Set up your environment variables by adding your Google API key to a .env file:
GOOGLE_API_KEY="your_api_key_here"
5. Initialize the MySQL database by running the provided SQL script in your MySQL environment.

# Usage
To start the application, run the following command:
streamlit run main.py
Once the app is running, open your browser to interact with the system, input natural language questions, and get real-time SQL query results.

# Project Structure
1. main.py: Streamlit application to handle the frontend.
2. langchain_helper.py: Contains the core logic for query generation and execution.
3. few_shots.py: Few-shot learning prompts for improving the LLM’s accuracy.
4. requirements.txt: List of required Python libraries.
5. .env: Configuration file to store your Google API key securely.

This repository provides a practical demonstration of how large language models can simplify database interactions by converting natural language questions into precise SQL queries.
