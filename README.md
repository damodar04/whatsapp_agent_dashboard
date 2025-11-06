🤖 WhatsApp Agent – AI-Powered Communication System
🎯 Overview

The WhatsApp Agent is an AI-driven communication and automation system designed to handle customer queries, process product orders, and maintain real-time interaction logs — all through WhatsApp.

It integrates a Flask backend (connected with Twilio APIs) and a Streamlit Dashboard for live monitoring, analytics, and order management.

✨ Key Highlights

✅ Real-time WhatsApp Automation
✅ Handles User Queries & Product Orders
✅ Secure Connection via Twilio Webhook
✅ Live Conversation Dashboard (Streamlit)
✅ Interactive Analytics & Order Tracking
✅ Fully Deployed on Render

🏗️ Architecture

The project is divided into two core services:

1️⃣ Flask Backend (app.py)

Manages communication between WhatsApp (via Twilio API) and the AI agent

Receives incoming messages through a webhook

Processes messages and sends AI-based responses

Stores chat and order data into CSV or database

2️⃣ Streamlit Dashboard (dashboard.py)

Displays real-time conversations and order history

Shows statistics like active users, total messages, completed orders, and bot responses

Provides analytics with charts and recent activity logs

Allows admins to visualize user-agent interactions in a WhatsApp-style UI

🌐 Deployment

Both services are deployed on Render:

Flask API: https://whatsapp-agent-api.onrender.com

Streamlit Dashboard: https://whatsapp-agent-dashboard.onrender.com

⚙️ Setup & Installation

Prerequisites:

Python 3.9+

Twilio Account (for WhatsApp Sandbox)

Render Account (for deployment)

1️⃣ Clone the Repository:

git clone https://github.com/yourusername/whatsapp-agent.git
cd whatsapp-agent


2️⃣ Install Dependencies:

pip install -r requirements.txt


3️⃣ Environment Setup (.env):
Create a .env file and add your credentials (this file should not be pushed to GitHub):

TWILIO_ACCOUNT_SID=your_account_sid
TWILIO_AUTH_TOKEN=your_auth_token
TWILIO_PHONE_NUMBER=your_twilio_number
OPENAI_API_KEY=your_api_key


4️⃣ Run the Flask Server:

python app.py


5️⃣ Run the Dashboard:

streamlit run dashboard.py

💬 How It Works

1️⃣ User sends a message to the Twilio WhatsApp sandbox number.
2️⃣ Flask app receives the message via webhook and processes it.
3️⃣ The AI agent generates a response and sends it back through Twilio.
4️⃣ Chat data and order info are stored for analytics.
5️⃣ The Streamlit dashboard shows all these interactions in real time.

📊 Dashboard Sections

💬 Live Conversations: Real-time WhatsApp-style chats

🛒 Order History: Displays completed or in-progress orders

📈 Analytics: Insights on user activity, message distribution, and payment trends

🧠 Future Enhancements

Connect with company’s verified WhatsApp number

Migrate to a real-time database (MongoDB / PostgreSQL)

Add AI-driven product recommendations

Integrate voice & image-based customer interactions

👤 Author

Damodar Bhawsar
📧 Email: damodar.pr04@gmail.com

🔗 LinkedIn: linkedin.com/in/damodar-bhawsar
