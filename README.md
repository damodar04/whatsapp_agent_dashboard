🤖 WhatsApp Agent – AI-Powered Communication System
🎯 Overview

The WhatsApp Agent automates communication between customers and businesses using AI and Twilio WhatsApp API.
It provides real-time chat automation, maintains logs, and visualizes insights in a live dashboard.

✨ Key Highlights

✅ Real-time WhatsApp Automation
✅ AI-driven Message Responses
✅ Handles Orders and Customer Queries
✅ Live Dashboard (Streamlit)
✅ Analytics and Order History
✅ Secure Deployment via Render

🏗️ Architecture

1️⃣ Flask Backend (app.py)

Connects with Twilio WhatsApp Webhook

Handles incoming and outgoing messages

Stores conversation and order data

2️⃣ Streamlit Dashboard (dashboard.py)

Displays chats in a WhatsApp-style UI

Shows user stats, analytics, and order history

Monitors bot performance in real time

🌐 Deployment

Flask API: https://whatsapp-agent-api.onrender.com

Dashboard: https://whatsapp-agent-dashboard.onrender.com

⚙️ Setup
git clone https://github.com/yourusername/whatsapp-agent.git
cd whatsapp-agent
pip install -r requirements.txt


Create a .env file with your Twilio and API keys 👇

TWILIO_ACCOUNT_SID=your_sid
TWILIO_AUTH_TOKEN=your_token
TWILIO_PHONE_NUMBER=your_number
OPENAI_API_KEY=your_api_key


Run Flask server:

python app.py


Run Dashboard:

streamlit run dashboard.py

📊 Dashboard Sections

💬 Live Conversations
🛒 Order History
📈 Analytics & Insights

👤 Author

Damodar Bhawsar
📧 damodar.pr04@gmail.com

🔗 LinkedIn

✅ To Fix Your GitHub README:

Rename your file → README.md (not .txt or .docx)

Copy-paste the above markdown content into it

Commit and push to GitHub

GitHub will automatically render it with icons, colors, and styling ✨

