# 🤖 WhatsApp Agent – AI-Powered Communication System

A comprehensive AI-driven communication and automation system designed to handle customer queries, process product orders, and maintain real-time interaction logs directly through WhatsApp. This project integrates a **Flask** backend with **Twilio APIs** and features a **Streamlit Dashboard** for live monitoring and analytics.

> 🔴 **Live Demo Sites:**
> * [API Endpoint (Flask)](https://whatsapp-agent-api.onrender.com)
> * [Admin Dashboard (Streamlit)](https://whatsapp-agent-dashboard.onrender.com)

---

## 🎯 Overview

This system acts as an intelligent intermediary between your business and customers on WhatsApp. It autonomously handles conversations while providing administrators with a complete view of operations through a dedicated dashboard.

### Key Highlights

✅ **Real-time Automation**: Instant AI responses on WhatsApp
✅ **Dual Capability**: Handles both general user queries & product orders
✅ **Secure Infrastructure**: Verified connection via Twilio Webhooks
✅ **Live Dashboard**: Built with Streamlit for real-time monitoring
✅ **Interactive Analytics**: Visual insights into user traffic and orders
✅ **Cloud Native**: Fully deployed and running on Render

---

## 🏗️ Architecture

The project is divided into two core services working in tandem:

### 1️⃣ Flask Backend (`app.py`)
The communication hub of the system.
* Manages the webhook connection with WhatsApp (via Twilio API).
* Processes incoming messages and generates AI-driven responses.
* Logs chat history and order data to the database/CSV.

### 2️⃣ Streamlit Dashboard (`dashboard.py`)
The administrative control center.
* **Real-time Feed**: Displays active conversations as they happen.
* **Order History**: Tracks completed and in-progress transactions.
* **Analytics Engine**: Visualizes active users, total message volume, and bot performance.

---

## 💬 How It Works

1.  **User Interaction**: Customer sends a message to the Twilio WhatsApp sandbox number.
2.  **Webhook Trigger**: Twilio forwards the message to the Flask backend.
3.  **AI Processing**: The agent interprets the intent and generates a relevant response.
4.  **Data Logging**: Interaction details and orders are saved for analysis.
5.  **Live Monitoring**: The Streamlit dashboard instantly reflects the new interaction.

---

## 📊 Dashboard Features

The Streamlit dashboard provides three main views:

| Section | Description |
| :--- | :--- |
| **💬 Live Conversations** | WhatsApp-style UI for viewing real-time user-agent chats |
| **🛒 Order History** | Detailed logs of all completed and pending product orders |
| **📈 Analytics** | Charts showing user activity, message distribution, and trends |

---

## ⚙️ Setup & Installation

### Prerequisites
* Python 3.9+
* Twilio Account (for WhatsApp Sandbox API)
* Render Account (optional, for deployment)

### Installation Steps

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/yourusername/whatsapp-agent.git](https://github.com/yourusername/whatsapp-agent.git)
    cd whatsapp-agent
    ```

2.  **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Environment Setup**
    Create a `.env` file in the root directory and add your credentials:
    ```env
    TWILIO_ACCOUNT_SID=your_account_sid
    TWILIO_AUTH_TOKEN=your_auth_token
    TWILIO_PHONE_NUMBER=your_twilio_number
    OPENAI_API_KEY=your_api_key
    ```

4.  **Run the Application**
    * *Terminal 1 - Start Backend:*
        ```bash
        python app.py
        ```
    * *Terminal 2 - Start Dashboard:*
        ```bash
        streamlit run dashboard.py
        ```

---

## 🧠 Future Enhancements

* [ ] Connect with a verified Business WhatsApp Number (non-sandbox).
* [ ] Migrate data storage to a real-time database (MongoDB / PostgreSQL).
* [ ] Implement AI-driven personalized product recommendations.
* [ ] Integrate support for voice notes and image-based interactions.

---

## 👤 Author

**Damodar Bhawsar**

* 📧 Email: [damodar.pr04@gmail.com](mailto:damodar.pr04@gmail.com)
* 🔗 LinkedIn: [linkedin.com/in/damodar-bhawsar](https://www.linkedin.com/in/damodar-bhawsar)
