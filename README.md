# 🤖 Multi-Agent AI Research Assistant

An automated, end-to-end multi-agent research pipeline built with **LangChain**, **LangGraph**, and **Mistral AI**.

Given a user-defined research topic, this system orchestrates specialized AI agents and chains to query search engines, extract detailed web page contents, synthesize comprehensive reports, and perform an automated quality critique.

---

## 🏗 System Architecture

The pipeline processes research requests sequentially through four dedicated nodes:

```text
               ┌───────────────────────┐
               │    User Research Topic│
               └───────────┬───────────┘
                           │
                           ▼
               ┌───────────────────────┐
               │  1. Search Agent      │
               │  (Gathers web info)   │
               └───────────┬───────────┘
                           │
                           ▼
               ┌───────────────────────┐
               │  2. Reader Agent      │
               │  (Scrapes target URL) │
               └───────────┬───────────┘
                           │
                           ▼
               ┌───────────────────────┐
               │  3. Writer Chain      │
               │  (Drafts main report) │
               └───────────┬───────────┘
                           │
                           ▼
               ┌───────────────────────┐
               │  4. Critic Chain      │
               │  (Reviews & evaluates)│
               └───────────────────────┘



---

## 🚀 Features

- 🔍 Intelligent web search using Tavily Search API
- 🌐 Automatic webpage scraping with BeautifulSoup
- 🤖 Multi-Agent architecture powered by LangChain
- 📝 AI-generated structured research reports
- 📊 AI-based report evaluation and feedback
- 🎨 Interactive Streamlit web interface
- ⚡ Fast and modular pipeline design

---

## 🏗️ Architecture

```
                 User Query
                      │
                      ▼
             🔎 Search Agent
          (Finds Relevant Sources)
                      │
                      ▼
             📖 Reader Agent
      (Scrapes the Best Webpage)
                      │
                      ▼
             ✍️ Writer Agent
    (Generates Research Report)
                      │
                      ▼
             🧐 Critic Agent
    (Reviews & Scores the Report)
                      │
                      ▼
               Final Response
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Core Programming |
| LangChain | AI Agent Framework |
| Mistral AI | Large Language Model |
| Tavily API | Web Search |
| BeautifulSoup | Web Scraping |
| Requests | HTTP Requests |
| Streamlit | User Interface |
| dotenv | Environment Variable Management |

---

## 📂 Project Structure

```
multiAgentModule/
│
├── app.py                 # Streamlit Application
├── pipeline.py            # Multi-Agent Pipeline
├── agents.py              # Search & Reader Agents
├── tools.py               # Tavily Search & Web Scraper
├── requirements.txt
├── README.md
├── .env
├── .gitignore
└── venv/
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/your-username/multi-agent-research-assistant.git
cd multi-agent-research-assistant
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Virtual Environment

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory.

```env
MISTRAL_API_KEY=your_mistral_api_key
TAVILY_API_KEY=your_tavily_api_key
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

---

## 📸 Demo

> Add screenshots or a GIF of your application here.

Example:

```
images/demo.png
```

---

## 💡 How It Works

1. User enters a research topic.
2. The Search Agent searches the web using Tavily.
3. The Reader Agent selects the most relevant webpage and extracts clean content.
4. The Writer Agent generates a detailed research report.
5. The Critic Agent reviews the report, provides a score, and suggests improvements.
6. The final report and feedback are displayed in the Streamlit interface.

---

## 🎯 Future Improvements

- PDF report export
- Citation management
- Multiple webpage summarization
- Memory-enabled AI agents
- Local LLM support (Ollama)
- Multi-language research
- Source credibility scoring

---

## 📚 Skills Demonstrated

- Agentic AI
- Generative AI
- LangChain
- Prompt Engineering
- Retrieval-Augmented Generation (RAG)
- AI Agent Design
- API Integration
- Web Scraping
- Python Development
- Streamlit Application Development

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Puneet Hiremath**

- 💼 Aspiring AI Engineer
- 🤖 Passionate about Generative AI & Agentic AI
- 🌐 Open to collaboration on AI projects

If you found this project useful, consider giving it a ⭐ on GitHub!