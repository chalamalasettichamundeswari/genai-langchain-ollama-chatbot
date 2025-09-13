# LangChain Ollama Streamlit Demo

This project demonstrates a simple GenAI application using LangChain, Ollama, and Streamlit. The app allows users to interact with the Gemma LLM model via a web interface, with prompt chaining and tracing enabled through LangSmith.

---

## 🚀 Features
- Streamlit UI for interactive Q&A
- Uses Ollama's `gemma:2b` model for LLM responses
- LangChain prompt chaining for structured queries
- LangSmith tracing for observability and debugging

---

## 📄 How It Works
1. Loads environment variables for API keys and tracing configuration
2. Sets up LangSmith tracing (if enabled)
3. Defines a prompt template for the assistant
4. Uses Ollama's Gemma model via LangChain
5. Displays a Streamlit UI for user questions
6. Chains prompt → LLM → output parser, and displays the answer

---

## 🛠️ Usage

1. **Install dependencies:**
	```bash
	pip install -r requirements.txt
	# If you need to manually install missing packages:
	pip install streamlit langchain langchain-community ollama langsmith python-dotenv
	```

2. **Configure environment variables:**
	- Create a `.env` file in the project root with the following content:
	```env
	LANGCHAIN_API_KEY=your-langsmith-api-key
	LANGCHAIN_PROJECT=your-project-name
	LANGCHAIN_TRACING_V2=true
	```
	- Make sure your Ollama server is running and the `gemma:2b` model is available. You can pull the model with:
	```bash
	ollama pull gemma:2b
	```

3. **Run the Streamlit app:**
	```bash
	streamlit run GenAIAppUsingOllama.py
	```

4. **Open the app in your browser:**
	- Streamlit will provide a local URL (e.g., http://localhost:8501) to access the app.

---

## 🔎 Tracing with LangSmith
LangSmith enables tracing and observability for LangChain applications. With the environment variables set, all chain executions are traced and can be viewed in your LangSmith dashboard.

---

## 🛠️ Tech Stack
- Python 3.10+
- LangChain
- Ollama (Gemma model)
- Streamlit
- LangSmith (tracing)
- dotenv (environment management)

---

## 🚀 Progress
- [x] Environment setup and dependencies installed<br/>
- [x] LangChain and Ollama integration tested<br/>
- [x] Streamlit UI implemented for LLM Q&A<br/>
- [x] LangSmith tracing enabled and verified<br/>

---

## ✍️ Author
Chamundeswari – Software Engineer exploring AI/ML + LLM frameworks.
