# 🧠 OmniBrief — AI Content Summarizer

> **Summarize YouTube videos, websites, and PDF documents with AI — fast, flexible, and in your preferred style.**

**OmniBrief** is an AI-powered content summarization application built with **Streamlit, LangChain, and Groq LLMs**.

It transforms long-form content from **YouTube videos, web pages, and PDF documents** into concise, easy-to-understand summaries with customizable **language, tone, style, and length**.

---

## ✨ Key Features

### 🎥 Multi-Source Summarization

* **YouTube Videos** — Extract and summarize video transcripts
* **Websites & Articles** — Summarize online content directly from URLs
* **PDF Documents** — Upload and summarize PDF files

### 🤖 AI-Powered Summarization

* Powered by **Groq LLMs**
* Integrated using **LangChain**
* Fast AI inference
* Context-aware summaries

### 🌍 Multiple Languages

Generate summaries in:

* 🇬🇧 English
* 🇵🇰 Urdu
* 🔤 Roman Urdu
* 🌐 Auto Detect

### ✍️ Multiple Writing Styles

Choose how your summary should be presented:

* 🔹 Bullet Points
* 📝 Paragraph
* 📋 Both

### 🎭 Customizable Tone

Select the tone that best fits your content:

* Neutral
* Formal
* Casual
* Executive Brief

### 🎯 Adjustable Summary Length

Control how detailed your generated summary should be according to your requirements.

### 📑 Additional Features

* 📌 Optional outline generation
* 👀 Source preview before summarization
* 📥 Download generated summaries
* ⚡ Fast response generation

---

# 🛠️ Tech Stack

## Frontend

* **Streamlit**

## AI & LLM

* **LangChain**
* **Groq API**
* **ChatGroq**

## Content Loaders

* **YouTube Loader**
* **WebBaseLoader**
* **PyPDFLoader**

## Supporting Libraries

* **Requests**
* **Validators**
* **yt-dlp**
* **youtube-transcript-api**

---

# 🧩 How OmniBrief Works

```text
                 ┌──────────────────┐
                 │   User Input     │
                 └────────┬─────────┘
                          │
          ┌───────────────┼────────────────┐
          ↓               ↓                ↓
    YouTube URL      Website URL       PDF Upload
          │               │                │
          └───────────────┼────────────────┘
                          ↓
                 Content Extraction
                          ↓
                    LangChain
                          ↓
                    Groq LLM
                          ↓
              AI Summary Generation
                          ↓
          ┌───────────────┼────────────────┐
          ↓               ↓                ↓
       Language         Tone            Style/Length
                          │
                          ↓
                 Final AI Summary
                          ↓
                    Download
```

---

# 💡 How to Use

### Step 1 — Select Your Content

Provide one of the supported inputs:

* YouTube video URL
* Website/article URL
* PDF document

### Step 2 — Customize Your Summary

Choose your preferred:

* Language
* Tone
* Writing style
* Summary length
* Optional outline

### Step 3 — Generate

Click **Generate Summary**.

OmniBrief extracts the content and sends the relevant context through the LangChain + Groq pipeline.

### Step 4 — Get Your Summary

The generated summary is displayed inside the application and can be downloaded for later use.

---

# 📂 Project Structure

```text
OmniBrief/
│
├── summarize.py
├── requirements.txt
├── youtube.txt
├── summarizer_img.png
└── README.md
```

### File Description

| File                 | Description                |
| -------------------- | -------------------------- |
| `summarize.py`       | Main Streamlit application |
| `requirements.txt`   | Project dependencies       |
| `youtube.txt`        | Sample YouTube URLs        |
| `summarizer_img.png` | Application screenshot     |
| `README.md`          | Project documentation      |

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/GenerativeAiWithMariams/OmniBrief.git
```

```bash
cd OmniBrief
```

---

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv
```

Activate it:

```bash
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Configure Groq API

OmniBrief requires a **Groq API key** to generate AI summaries.

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
```

You can obtain your API key from the [Groq Console](https://console.groq.com/keys?utm_source=chatgpt.com).

> ⚠️ Never commit your `.env` file or expose your API key publicly.

Add `.env` to your `.gitignore`:

```text
.env
venv/
__pycache__/
```

---

# ▶️ Run the Application

Start the Streamlit application with:

```bash
streamlit run summarize.py
```

The application will open in your default browser.

---

# 📊 Supported Inputs

| Content Type      | Support |
| ----------------- | ------: |
| 🎥 YouTube Videos |       ✅ |
| 🌐 Websites       |       ✅ |
| 📄 PDF Documents  |       ✅ |

---

# 🌍 Supported Languages

| Language    | Supported |
| ----------- | --------: |
| English     |         ✅ |
| Urdu        |         ✅ |
| Roman Urdu  |         ✅ |
| Auto Detect |         ✅ |

---

# 🎭 Summary Customization

OmniBrief gives users control over how the final summary is generated.

| Option       | Available Choices                        |
| ------------ | ---------------------------------------- |
| **Language** | English, Urdu, Roman Urdu, Auto Detect   |
| **Style**    | Bullet Points, Paragraph, Both           |
| **Tone**     | Neutral, Formal, Casual, Executive Brief |
| **Length**   | Adjustable                               |
| **Outline**  | Optional                                 |

---

# 📸 Application Preview

Add your application screenshot:

```markdown
![OmniBrief AI Summarizer](summarizer_img.png)
```

---

# 🎯 Use Cases

OmniBrief can be useful for:

* 🎓 Students summarizing lectures and study material
* 📚 Researchers processing lengthy documents
* 💼 Professionals summarizing reports and articles
* 🎥 Content creators summarizing YouTube videos
* 📰 Readers quickly understanding long articles
* 📄 Businesses processing PDF documents
* 🧑‍💻 Developers experimenting with LLM applications

---

# 🔮 Future Improvements

Planned improvements include:

* 🎙️ Speech-to-Text summarization
* 🎵 Audio file summarization
* 📄 DOCX document support
* 📊 PowerPoint summarization
* 🌍 AI-powered translation
* 💬 Chat with PDF
* 📝 AI Notes Generator
* 🔗 Share summaries through links
* 📚 Summary history dashboard
* 🔐 User authentication
* ☁️ Cloud deployment

---

# 🤝 Contributing

Contributions are welcome!

### 1. Fork the repository

### 2. Create a new branch

```bash
git checkout -b feature-name
```

### 3. Make your changes

### 4. Commit your changes

```bash
git commit -m "Add new feature"
```

### 5. Push the branch

```bash
git push origin feature-name
```

### 6. Open a Pull Request

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👩‍💻 Author

## Maryam Faiz

**Generative AI Engineer | AI Developer | Python Developer**

Specializing in:

**Generative AI • RAG • Agentic AI • LLM Applications • LangChain • NLP • Python**

### Connect With Me

🔗 **GitHub:**
https://github.com/GenerativeAiWithMariams

🔗 **LinkedIn:**
https://www.linkedin.com/in/maryam-faiz-7a8259423/

📧 **Email:**
[maryamfaiz.genai@gmail.com](mailto:maryamfaiz.genai@gmail.com)

---

# ⭐ Show Your Support

If you found **OmniBrief** useful or interesting, please consider giving the repository a ⭐ on GitHub!

> **Built with ❤️ using Streamlit, LangChain & Groq**
