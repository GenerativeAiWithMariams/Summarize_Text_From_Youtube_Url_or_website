# 🧠 OmniBrief – AI Summarizer

AI-powered content summarization application built with **Streamlit**, **LangChain**, and **Groq LLM**. OmniBrief can summarize content from **YouTube videos, websites, and PDF documents** into clear, concise, and customizable summaries.

---

## ✨ Features

- 🎥 Summarize YouTube videos using transcripts
- 🌐 Summarize articles and websites
- 📄 Upload and summarize PDF documents
- 🤖 Powered by Groq LLMs via LangChain
- 🌍 Multiple output languages
  - English
  - Urdu
  - Roman Urdu
  - Auto Detect
- ✍️ Multiple writing styles
  - Bullet Points
  - Paragraph
  - Both
- 🎯 Adjustable summary length
- 🎭 Multiple tones
  - Neutral
  - Formal
  - Casual
  - Executive Brief
- ⚡ Fast AI responses using Groq
- 📥 Download generated summaries
- 📑 Optional outline generation
- 👀 Source preview before summarization

---

## 🛠️ Tech Stack

### Frontend
- Streamlit

### AI & LLM
- LangChain
- Groq API
- ChatGroq

### Document Loaders
- YouTube Loader
- WebBaseLoader
- PyPDFLoader

### Python Libraries
- Requests
- Validators
- yt-dlp
- youtube-transcript-api

---

## 📂 Project Structure

```
.
├── summarize.py          # Main Streamlit application
├── requirements.txt      # Python dependencies
├── youtube.txt           # Sample URLs
├── summarizer_img.png    # Project screenshot
└── README.md
```

---

## 🚀 Installation

### Clone Repository

```bash
git clone https://github.com/your-username/OmniBrief.git
cd OmniBrief
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Configure Groq API

Create a `.env` file or set your environment variable.

```env
GROQ_API_KEY=your_groq_api_key
```

Get your API Key from:

https://console.groq.com/keys

---

## ▶️ Run the Application

```bash
streamlit run summarize.py
```

---

## 💡 How It Works

1. Enter a YouTube URL, Website URL, or upload a PDF.
2. Select your preferred:
   - Language
   - Tone
   - Summary Style
   - Target Length
3. Click **Generate Summary**.
4. AI processes the content using LangChain and Groq.
5. Download your generated summary instantly.

---

## 📸 Application Preview

> Add your project screenshot here.

```
summarizer_img.png
```

---

## 🎯 Supported Inputs

| Input | Supported |
|--------|-----------|
| YouTube Videos | ✅ |
| Websites | ✅ |
| PDF Files | ✅ |

---

## 🌐 Supported Languages

- English
- Urdu
- Roman Urdu
- Auto Detect

---

## 📌 Future Improvements

- Speech-to-Text Support
- Audio File Summarization
- DOCX Support
- PPT Summarization
- Translation Feature
- Chat with PDF
- AI Notes Generator
- Share Summary via Link
- History Dashboard

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Added new feature"
```

4. Push your branch

```bash
git push origin feature-name
```

5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👩‍💻 Author

**Maryam Faiz**

**Generative AI Engineer | Python Developer | LangChain | Agentic AI | RAG | LLM Applications**

GitHub: https://github.com/GenerativeAiWithMariams

---

### ⭐ If you found this project helpful, don't forget to give it a Star!
