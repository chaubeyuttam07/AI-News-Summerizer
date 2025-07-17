# 📰 AI News Summarizer

AI-powered tool that fetches trending news articles and generates concise summaries using state-of-the-art LLMs like OpenAI's GPT. Designed for developers, journalists, and researchers who want quick, readable overviews of the news.

---

## 🚀 Features

- **Fetches recent news** via public RSS feeds or APIs (e.g. NewsAPI).
- **Generates concise summaries** using large language models (OpenAI GPT, etc.).
- **Batch processing support** for multiple articles.
- **Flexible architecture** allowing custom prompts and summarization styles.
- **Command-line interface** for easy integration and automation.
- **(Optional)** LangGraph orchestration for multi-stage processing / pipeline workflows.

---

## 🔧 Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/chaubeyuttam07/AI-News-Summerizer.git
    cd AI-News-Summerizer
    ```

2. Create a Python virtual environment and activate it:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Set your OpenAI API key (and NewsAPI key if used):
    ```bash
    export OPENAI_API_KEY="your_openai_api_key"
    export NEWSAPI_KEY="your_newsapi_key"  # optional
    ```

---

## 🧩 Usage

### 📰 Summarize from RSS/URL
```bash
python summarize.py --source rss --url https://rss.nytimes.com/services/xml/rss/nyt/HomePage.xml
