# SQL Exercises Repository

Welcome to the SQL Exercises repository! This collection of Jupyter notebooks contains a variety of SQL exercises designed to showcase different aspects of SQL querying and problem-solving.
All those excercises are made by Explore AI for thier Data Science Course, however those are my answers for the excersices
## Important Note

**Do not execute the database connection line in the exercises!** The connection line often contains sensitive information, including the database password. It is included for illustrative purposes only and should not be executed. The primary goal is to highlight the SQL queries and solutions within each exercise.

For learning purposes, it's crucial to understand that exposing sensitive information, such as database credentials, in code is a bad practice in real-world scenarios. In professional settings, proper security measures should be implemented.

## Usage

1. Clone the repository to your local machine.
2. Open the Jupyter notebooks using your preferred environment (e.g., Jupyter Notebook, JupyterLab).
3. Review the exercises and solutions provided in each notebook.
4. Feel free to modify and experiment with the queries to deepen your understanding.

## Better Practice: Using Environment Variables

In a real-world scenario, it's recommended to use environment variables for storing sensitive information like database credentials. Here's a basic example in Python:

```python
import os
import psycopg2

# Set your environment variables
DB_HOST = os.environ.get('DB_HOST')
DB_PORT = os.environ.get('DB_PORT')
DB_NAME = os.environ.get('DB_NAME')
DB_USER = os.environ.get('DB_USER')
DB_PASSWORD = os.environ.get('DB_PASSWORD')

# Establish a database connection
conn = psycopg2.connect(
    host=DB_HOST,
    port=DB_PORT,
    database=DB_NAME,
    user=DB_USER,
    password=DB_PASSWORD
)
