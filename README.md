# HealthAI 🏥

> Revolutionizing Healthcare with AI — Quick, accurate and effortless patient record analysis & monitoring.

![HealthAI Banner](images/image_1.png)

---

## 📌 Overview

HealthAI is a full-stack web application that combines AI-powered symptom analysis with real-time patient monitoring. Users can chat with an AI health assistant, maintain their medical profile, and track health trends through an interactive dashboard.

---

## ✨ Features

- **AI Assistant** — Describe symptoms and get instant AI-powered health guidance powered by Google Gemini
- **Patient Records** — Manage your medical profile (age, gender, blood group, height) and track disease history
- **Real-time Dashboard** — Monitor patient vitals, view health trends, and track records on an interactive calendar
- **User Monitoring** — Search and add users to monitor their health data
- **Authentication** — Secure login with JWT + Google OAuth2
- **Real-time Updates** — Socket.IO for live data sync

---

## 🖼️ Screenshots

| Home | AI Assistant |
|------|-------------|
| ![Home](images/image_1.png) | ![AI Assistant](images/image_2.png) |

| Patient Records | Dashboard |
|----------------|-----------|
| ![Records](images/image_3.png) | ![Dashboard](images/image_4.png) |

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS, Tailwind CSS |
| Backend | Node.js, Express.js |
| Database | MongoDB (Mongoose) |
| AI | Google Gemini API (`@google/genai`) |
| Auth | JWT, Passport.js, Google OAuth2 |
| Real-time | Socket.IO |
| File Uploads | Multer |
| Email | Nodemailer |

---

## 📁 Project Structure

```
healthai/
├── config/           # DB and passport config
├── controllers/      # Route logic
├── middleware/       # Auth middleware
├── models/           # Mongoose schemas
├── routes/           # Express routes
├── script/           # Frontend JS scripts
├── services/         # Business logic / AI services
├── style/            # CSS files
├── uploads/          # User uploaded files
├── index.html        # Landing page
├── ai-assistant.html # AI chat page
├── record.html       # Patient records page
├── dashbord.html     # Dashboard page
├── about.html        # About page
├── contact.html      # Contact page
├── server.js         # Entry point
└── .env              # Environment variables
```

---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js v18+
- MongoDB (local or Atlas)
- Google Gemini API key
- Google OAuth credentials

### Steps

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/healthai.git
cd healthai

# 2. Install dependencies
npm install

# 3. Configure environment variables
# Create a .env file and fill in the values (see below)

# 4. Start the server
npm start
```

### Environment Variables

Create a `.env` file in the root directory:

```env
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GEMINI_API_KEY=your_gemini_api_key
EMAIL_USER=your_email
EMAIL_PASS=your_email_password
```

---

## 🚀 Usage

1. Visit `http://localhost:3000`
2. Sign up / Sign in (email or Google OAuth)
3. Fill in your Patient Profile under **Record**
4. Chat with the **AI Assistant** about your symptoms
5. Monitor health trends from the **Dashboard**

---

## 👥 Team

Built with ❤️ at a Hackathon.

---

## 📄 License

This project is for educational/hackathon purposes.
