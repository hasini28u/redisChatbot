# 🤖 Redis-Powered Chatbot with LangChain & Google Gemini

This project demonstrates how to build a **stateful AI chatbot** using:
- **LangChain** for managing LLM chains
- **Google Gemini (via LangChain)** for responses
- **Redis** to store and retrieve chat history across sessions

It’s built as part of my Deep Learning & NLP training to explore how real-world LLM-based chatbots are structured.

---

## 📌 Key Features

- 🔄 **Session Persistence**: Redis stores conversation history using unique session IDs.
- 🧠 **LLM Integration**: Uses Google Gemini (`gemini-2.5-pro`) to generate responses.
- 🧰 **LangChain Runnables**: Chains built using `RunnableLambda`, `RunnableWithMessageHistory`.
- 🧾 **Secure Redis Usage**: Connects to a remote Redis instance with authentication.

---

## 📁 File Structure

- `redisChatbot.ipynb`: Main Jupyter Notebook that walks through setup, implementation, and testing.
- No external UI – interaction is demonstrated directly through code cells.

---

## 🚀 How to Run

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
Install Required Packages
Most are handled in the notebook via:

bash
Copy
Edit
!pip install langchain langchain_community langchain_google_genai redis sentence-transformers openai
Setup Redis Server

Local: Install and run Redis (apt install redis-server)

Cloud: Use a service like Redis Cloud

Add API Keys
Set the GOOGLE_API_KEY as an environment variable inside the notebook.

Run All Cells
Use a Jupyter-compatible environment like Google Colab or VSCode.

🔐 Note on Security
Avoid hardcoding API keys or Redis credentials in public notebooks.

Store secrets using environment variables or secret managers.

📬 Contact
Feel free to reach out if you want to collaborate or discuss improvements:

🔗 LinkedIn: www.linkedin.com/in/hasini-uppaluri-387a592a2

📧 hasiniuppaluri@gmail.com
