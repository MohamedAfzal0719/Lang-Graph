# Lang-Graph
AI-powered Question Answering web app built with FastAPI, LangGraph, and Gemini LLM. Features structured workflows, validation logic, and retry handling for reliable AI responses.

# LangGraph AI Question Answering Web App

A simple AI-powered question answering web application built using **FastAPI**, **LangGraph**, and **Gemini LLM**.  
The project demonstrates how to combine AI generation with rule-based validation and controlled workflows.
---
## 🚀 Features
- Ask questions through a web interface
- AI-generated answers using Gemini LLM
- Structured workflow using LangGraph
- Rule-based answer validation
- Retry mechanism for better responses
- Clean frontend–backend separation
---
## 🧠 Tech Stack
- **Backend:** FastAPI (Python)
- **Workflow Engine:** LangGraph
- **LLM:** Google Gemini
- **Frontend:** HTML, CSS, JavaScript
- **Environment Management:** Python virtual environment
---
## 📂 Project Structure
Langraph/
├── app.py
├── backend/
│ ├── init.py
│ ├── graph.py
│ ├── nodes.py
│ └── state.py
├── frontend/
│ ├── index.html
│ ├── style.css
├── .env
├── requirements.txt
---
## ⚙️ How It Works
1. User submits a question from the frontend
2. FastAPI receives the request
3. LangGraph initializes a workflow state
4. Gemini generates an answer
5. The answer is validated using rule-based logic
6. If invalid, the workflow retries once
7. Final response is returned to the UI
---
## 🧪 Validation Logic
- Answer must not be empty  
- Answer length must be at least 50 characters  
- Maximum of one retry is allowed  
This ensures controlled and predictable AI behavior.
---
## ▶️ How to Run Locally
### 1️⃣ Create and activate virtual environment
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
###2️⃣Add Gemini API key
```bash
Create a .env file in the project root:
GOOGLE_API_KEY=your_gemini_api_key_here

###3️⃣ Run the application
python app.py

