# 🎬 ClipQuoter
Extract transcripts and AI-powered quotes with precise timestamps from YouTube videos.

## 🚀 Overview
**ClipQuoter** is a Streamlit-based web app that takes YouTube video URLs, fetches their transcripts, and uses **Google Gemini AI** (via LangChain) to extract meaningful quotes along with timestamps. The tool is designed for creators, researchers, and analysts who need quick insights and shareable quotes from video content.

## ✨ Features
- 📌 Extract transcripts from multiple YouTube videos  
- 🤖 AI-powered quote extraction with start and end timestamps  
- 🗂️ Results saved as JSON for easy reuse  
- ⚡ Clean and interactive Streamlit interface  
- 🛡️ Error handling for unavailable videos, disabled transcripts, or invalid API keys  

## 🛠️ Tech Stack
- **Streamlit** – Frontend interface  
- **LangChain Core & Community** – AI integration and prompt management  
- **langchain_google_genai** – Google Gemini AI model integration  
- **youtube-transcript-api** – Fetching YouTube transcripts  
- **JSON** – Data formatting and storage  

## 📂 Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/your-username/ClipQuoter.git
cd ClipQuoter
pip install -r requirements.txt
```

Create a `requirements.txt` file with:
```txt
streamlit
langchain-core
langchain-google-genai
youtube-transcript-api
```

## ▶️ Usage
Run the Streamlit app:
```bash
streamlit run app.py
```

1. Enter your **Gemini API key** (kept secure in password field)
2. Paste one or more YouTube video URLs (one per line)
3. Click "Fetch Transcripts and Extract Quotes"
4. View extracted transcripts and AI-generated quotes with timestamps

## 📁 Project Structure
```
ClipQuoter/
├── app.py              # Main Streamlit application
├── transcripts/        # Auto-created folder for JSON transcripts
├── requirements.txt    # Python dependencies
└── README.md          # This file
```

## 🔮 Use Cases
- ✍️ **Content Creation** – Pull quotes for blogs, presentations, and social media
- 🎓 **Research** – Extract important statements from lectures and interviews
- 📑 **Documentation** – Build timestamped quote databases
- 📊 **Analysis** – Study patterns in speeches or discussions

## 🔧 Configuration
### API Setup
1. Get a Google Gemini API key from [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Enter the key in the app's secure input field
3. No additional configuration required

### Supported URL Formats
- `https://www.youtube.com/watch?v=VIDEO_ID`
- `https://youtu.be/VIDEO_ID`
- URLs with additional parameters are automatically parsed

## ⚠️ Limitations
- Requires a valid **Google Gemini API key** (paid service)
- Dependent on transcript availability on YouTube
- Only processes videos with available transcripts
- Internet connection required for API calls
- Transcripts must be in supported languages

## 🤝 Contributing
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🙏 Acknowledgments
- YouTube Transcript API for seamless transcript access
- Google Gemini AI for intelligent quote extraction
- Streamlit team for the amazing web framework
- LangChain for AI integration utilities

---

🚀 **Built with ❤️ by Ujwal**

*Star ⭐ this repository if you found it helpful!*
