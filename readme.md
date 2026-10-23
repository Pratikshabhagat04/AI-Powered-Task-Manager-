# 🤖 AI-Powered Task Manager

An AI-powered task management application built using **Python, LangChain, AI Agents, Database Tools, and Streamlit**. The application allows users to manage their todos through CRUD operations and uses an AI agent to interact with database tools for task-related operations.

## ✨ Features

- 🤖 **AI Agent:** Uses LangChain to process user requests and interact with available tools.
- ➕ **Create Tasks:** Add new todos to the database.
- 📋 **Read Tasks:** Retrieve and view existing todos.
- ✏️ **Update Tasks:** Modify task details as needed.
- 🗑️ **Delete Tasks:** Remove tasks from the database.
- 🗄️ **Database Integration:** Store and manage todo records.
- 💬 **Interactive UI:** Use Streamlit to interact with the application.
- 🔗 **Tool-Based Architecture:** Connect the AI agent with database operations through tools.

## 🛠️ Tech Stack

- **Language:** Python
- **LLM Framework:** LangChain
- **AI Architecture:** Tool-using AI Agent
- **Frontend:** Streamlit
- **Database:** Database configured in the project
- **Environment Management:** python-dotenv
- **LLM Provider:** The provider configured in the project

## 🏗️ Architecture

```text
        User
         |
         v
   Streamlit UI
      app.py
         |
         v
    LangChain Agent
         |
         v
     Database Tools
         |
         v
      Database
         |
         v
   CRUD Operations
 Create | Read | Update | Delete
```

## 📂 Project Structure

```text
AI-Powered-Task-Manager/
│
├── app.py              # Streamlit application
├── agent.py            # AI agent configuration, if separated
├── tools.py            # Database CRUD tools, if separated
├── .env                # Environment variables
├── .gitignore          # Excluded files and secrets
├── requirements.txt    # Project dependencies
└── README.md           # Project documentation
```

*Adjust the filenames to match your actual repository.*

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Pratikshabhagat04/AI-Powered-Task-Manager-.git
cd AI-Powered-Task-Manager-
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

Ensure `requirements.txt` includes the packages actually used by your project, such as LangChain, your model-provider integration, Streamlit, and your database driver.

### 4. Configure Environment Variables

Create a `.env` file if your application requires API keys or database configuration.

Example:

```env
MODEL=your_model_name
GROQ_API_KEY=your_groq_api_key
DATABASE_URL=your_database_connection_string
```

Use only the variables required by your code. Replace the example values with your actual configuration.

**Security:** Never commit API keys, database passwords, or other secrets to GitHub.

### 5. Run the Application

```bash
streamlit run app.py
```

Open the local URL displayed in the terminal, usually:

`http://localhost:8501`

## 🔄 CRUD Operations

| Operation | Description                      |
| --------- | -------------------------------- |
| Create    | Add a new todo to the database.  |
| Read      | Retrieve existing todos.         |
| Update    | Modify an existing todo.         |
| Delete    | Remove a todo from the database. |

These operations are exposed through database tools that the LangChain agent can use according to the application's implementation.

## 🧠 How It Works

1. The user enters a task-related request through the Streamlit interface.
2. The LangChain agent processes the request using the configured language model.
3. The agent selects an appropriate database tool when needed.
4. The selected tool performs the corresponding CRUD operation.
5. The result is returned and displayed in the Streamlit application.

## 🎯 Learning Outcomes

This project provides practical experience with:

- Building AI agents using LangChain.
- Integrating language models with custom tools.
- Connecting AI applications to databases.
- Implementing CRUD operations in Python.
- Building interactive interfaces with Streamlit.
- Designing tool-based AI application workflows.

## 🔮 Future Enhancements

- Task prioritization and deadline management.
- Task search and filtering.
- Task completion status tracking.
- AI-generated task suggestions.
- Due-date reminders and productivity reports.
- User authentication and personalized task lists.

## 👩‍💻 Author

**Pratiksha Bhagat**

AI Developer | Python | LangChain | AI Agents | Database Integration | Generative AI

## 🔗 GitHub Repository&#x20;

[View AI-Powered Task Manager on GitHub](https://github.com/Pratikshabhagat04/AI-Powered-Task-Manager-)

