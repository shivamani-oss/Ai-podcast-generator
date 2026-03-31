# Ai-podcast-generator
🎙️ AI PODCAST GENERATOR
Transform any topic into a fully voiced podcast in seconds — powered by Google Gemini, Murf.ai, and N8N automation.
<img width="1920" height="1080" alt="Screenshot (156)" src="https://github.com/user-attachments/assets/6ad27919-7fe5-4c0d-b772-618b2c41c17a" />
<img width="1920" height="1080" alt="Screenshot (157)" src="https://github.com/user-attachments/assets/5e879a1e-69cf-45f0-9b05-091907589f2c" />

🌐 Live Demo
👉 Try it here → https://pastel-pod-pal-83.lovable.app

📖 What is this?
AI Podcast Generator is a fully automated pipeline that takes a text topic as input and returns a ready-to-listen audio podcast — no recording, no editing, no studio required.
Just type a topic like "The future of AI in healthcare" and within seconds you get a natural-sounding, 2-minute podcast episode.

✨ Features

🧠 AI Script Writing — Google Gemini writes a conversational, engaging podcast script
🎤 Text-to-Speech — Murf.ai converts the script into natural human-sounding audio
⚡ Fully Automated — End-to-end pipeline via N8N, triggered by a single webhook
🎨 Clean Frontend — Simple and beautiful UI built with Lovable.dev
🔗 Webhook-based — Easy to integrate with any frontend or tool

🔄 How It Works
User types a topic
       ↓
Webhook receives the request
       ↓
Google Gemini writes a 2-minute podcast script
       ↓
Murf.ai converts the script to audio (Voice: Terrell, en-US)
       ↓
Audio file is downloaded and returned
       ↓
User gets a ready-to-play podcast episode

🚀 Setup & Installation
Prerequisites

N8N account (self-hosted or cloud)
Google Gemini API key
Murf.ai API key

Steps

Clone this repository

bash   git clone https://github.com/shivamani-oss/ai-podcast-generator.git
   cd ai-podcast-generator

Import the N8N workflow

Open your N8N instance
Go to Workflows → Import
Upload AIPodcastwithWebhook.json


Add your credentials in N8N

Add your Google Gemini API key to the Gemini node
Add your Murf.ai API key to the HTTP Request node


Activate the workflow

Click Activate in N8N
Copy your webhook URL

Connect your frontend

Update the webhook URL in your frontend app
Or use the live demo at pastel-pod-pal-83.lovable.app

📡 API Usage
You can also trigger the podcast generator directly via HTTP POST:
bashcurl -X POST https://YOUR_N8N_WEBHOOK_URL \
  -H "Content-Type: application/json" \
  -d '{"text": "The future of space exploration"}'
Response: Returns the generated audio file (binary).

📸 Screenshots
Frontend UI
<img width="1920" height="1080" alt="Screenshot (158)" src="https://github.com/user-attachments/assets/e75ef2ab-7091-416f-bab6-a3eaf0ffc971" />

N8N Workflow

LinkedIn: https://www.linkedin.com/in/sattu-shivamani-4096a1296/
GitHub: https://github.com/shivamani-oss

⭐ If you found this useful, give it a star! It helps others discover the project.
