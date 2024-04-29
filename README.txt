An End-to-End LLM project that uses the technologies 
1. LangChain
2. Hugging Face
3. Streamlit
4. Chroma
5. MySQL
6. Google PaLm

Description:
Happy Tees is a T-shirt store where they maintain their inventory, sales and discounts data in MySQL database. A store manager will may ask questions such as,

How many white color Adidas t shirts do we have left in the stock?

Output:
Build a system similar to ChatGPT where I can ask a question in natural human language. It'll convert the question into a SQL query and execute it on the database.

##### Project requirements: 
1. Happy_Tees database in MySQL
   a. t_shirts(Database): maintains the inventory count that includes price per each unit.
   b. discounts(Database): Discount for each piece in t_shirts database.

##### Technical Architecture:
1. Google PaLm(LLM) available in LangChain framework: Responsible for converting natural language question to a SQL Query.
2. SQLDatabaseChain class in LangChain framework.
3. Few short learning: To handle complex questions
       Preparing a training dataset where we have same question and corresponding SQL query.
4. Hugging Face library: To convert the training dataset into embedding vectors.
5. ChromaDB(open source vector database): To store the embedded vectors.
