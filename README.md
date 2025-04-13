# 🤖 AI Interview Bot

An interactive, multilingual, voice-enabled interview simulation platform powered by OpenAI, AWS, and Gradio. This tool helps candidates practice real-world technical, behavioral, and situational questions based on their resume and job description — with instant GPT feedback and voice analysis.

---

## 🚀 Features

- 📄 Upload Resume (PDF/DOCX) + Job Description
- 🔍 Skill extraction using AWS Comprehend
- 🧠 Dynamic question generation from curated dataset
- 🎙️ Answer using voice or text
- 🌍 Supports 5 languages: English, French, Spanish, Hindi, German
- 🗣️ Whisper-based transcription of voice input
- 🔎 Confidence analyzer for voice input (clear, hesitant, unsure)
- 💬 GPT-powered structured feedback
- 🔁 Session history retrieval using Session ID
- 🔊 Text-to-speech for questions (AWS Polly)
- 🧾 Clean, Chatbot-like interface via Gradio

---

## 🛠️ Setup Instructions (Ubuntu / WSL)

### 1. Clone the repository
```bash
git clone https://github.com/Harsh-Subhash-Sharma/AI-Interview-bot.git
cd AI-Interview-bot

### 2. Create a virtual environment
python3 -m venv venv
source venv/bin/activate

### 3. Install dependencies
pip install -r requirements.txt

🛑 Do NOT commit this .env file to GitHub.
Create a .env file in the project root (this is excluded from Git).
OPENAI_API_KEY=your_openai_key_here
AWS_ACCESS_KEY_ID=your_aws_access_key_id
AWS_SECRET_ACCESS_KEY=your_aws_secret_key
AWS_REGION=your_aws_region (e.g. us-east-1)

▶️ Running the App
python gradio_ui.py

✅ Tests & Coverage
pytest --cov=utils tests/





