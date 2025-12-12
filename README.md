# Datalynx-Implementation-of-conversional-interface-for-database-using-NLP

This project converts plain English questions into accurate SQL SELECT queries using a local AI engine, executes them on a SQLite student database, auto-fixes SQL errors with the model, and shows results in a Streamlit chat UI with a schema-viewer sidebar. Designed for non-technical users without SQL knowledge.

## About
This project is an intelligent database query assistant that enables users to fetch information from a structured database using simple English questions, without needing any SQL knowledge. The application uses a local large language model running on standard CPU hardware to translate natural language into accurate SQL SELECT queries. The generated SQL is executed securely on a lightweight embedded relational database containing student records. If the model produces an invalid query, the system sends the error and schema context back to the model to automatically correct and re-generate a working SQL statement, ensuring higher accuracy and reliability. The results are displayed in a conversational chat-style interface built with a Python-based UI framework, while a sidebar visually shows the database schema (tables and columns) for user clarity. The design focuses on simplicity, accuracy, and usability, making database access seamless for non-technical users and suitable for academic demos, presentations, and future enhancements.

## Features
-Natural Language → SQL using local LLM -SQL auto-fix loop on database errors -SQLite database integration -Interactive chat UI via Streamlit -Schema viewer sidebar for DB structure visibility -Data access without SQL knowledge -No GPU, CPU-based model execution

## Requirements

Operating System: Requires a 64-bit OS such as Windows 10 or Ubuntu for compatibility with the local LLM runtime.
Development Environment: Python 3 (version 3.8 or later recommended) is required for backend logic and database interaction.
LLM Runtime: Ollama to download and run AI language models on CPU without GPU dependency.
SQL Generation Model: Mistral model for converting natural language into accurate SQL queries.
Database System: SQLite to store structured student data and execute generated SQL queries.
User Interface Framework: Streamlit for creating an interactive chat-based dashboard and schema viewer sidebar.
Data Processing Library: pandas for reading SQL results and displaying them in table format.
Version Control: Git for collaborative development and project source code management.
IDE: Use of Visual Studio Code as the main coding and debugging environment with terminal and version control integration.
Additional Dependencies: Installable packages include streamlit, pandas, and ollama for local natural language to SQL processing.

## System Architecture

<img width="776" height="773" alt="image" src="https://github.com/user-attachments/assets/568c4dc1-158d-489b-bd76-6c11c677d8ce" />

## Output

### Output1 - User Interface

<img width="774" height="408" alt="image" src="https://github.com/user-attachments/assets/0d9d04ba-d3d8-41ee-8586-a3167840b8bb" />


### Output2 - Project output

<img width="766" height="384" alt="image" src="https://github.com/user-attachments/assets/cf42e09d-12ed-49d2-a61c-5b0e58b96673" />

## Results and Impact
The Natural Language–Based Database Query System significantly improves data accessibility by allowing users to interact with databases without requiring SQL knowledge. By integrating a local large language model with a dynamic schema-aware SQL generator, the system enables intuitive, human-like interaction with structured data. Users can perform complex operations—including reading, updating, and modifying database structures—simply through natural language, making data management more efficient and user-friendly.

This project demonstrates the potential of AI-driven automation in database systems, showcasing how natural language processing can simplify technical tasks traditionally reserved for trained professionals. The ability to automatically interpret user intent, generate precise SQL, and correct errors enhances reliability and usability.

Serving as a foundation for intelligent database assistants, this project paves the way for advanced enterprise tools, multilingual support, voice-based interfaces, and scalable real-world data management solutions, contributing toward more accessible and intelligent human–computer interaction.

## Articles published / References

```
[1]  Y. Li and H. Jagadish, “Constructing SQL queries from natural language expressions,” in Proc. 19th IEEE Int. Conf. Data Eng. (ICDE), Bangalore, India, Mar. 2003, pp. 1–10.
[2] J. Zhang, R. Li, and M. Zhang, “NL2SQL: A generic natural language interface for querying relational databases,” in Proc. 33rd AAAI Conf. Artif. Intell., Honolulu, HI, USA, Jan. 2019, pp. 5515–5522.
[3] J. Wang, S. Xu, and Q. Chen, “Text-to-SQL generation using neural networks: A comprehensive review,” IEEE Access, vol. 8, pp. 43636–43652, Mar. 2020.
```
