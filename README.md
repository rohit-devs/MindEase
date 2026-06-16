# 🧠 MindEase — AI-Powered Mental Wellness Platform

> Supporting emotional well-being through AI-driven sentiment analysis, crisis detection, and real-time mental health insights.

---

## 🌟 Overview

MindEase is an AI-powered mental wellness platform designed to help users monitor and understand their emotional state through intelligent conversations.

The platform analyzes user messages in real time, visualizes emotional trends using the unique **Sentiment Wave**, and provides immediate support resources when signs of emotional distress or crisis are detected.

Whether users want to track their mental wellness, express their thoughts safely, or seek guidance during difficult moments, MindEase offers a simple, accessible, and supportive experience.

---

## 🚀 Key Features

### 🌊 Sentiment Wave (Unique Innovation)

* Real-time sentiment analysis for every message
* Scores emotions from **-100 (Crisis)** to **+100 (Positive)**
* Live animated emotional trend graph
* Dynamic color transitions:

  * 🟢 Positive
  * 🟡 Neutral
  * 🟠 Concern
  * 🔴 Crisis
* Visual danger-zone indicators

### 💬 Intelligent Wellness Chat

* AI-powered conversational support
* Emotion-aware responses
* Personalized interaction based on sentiment level
* Guest mode available

### 🚨 Crisis Detection System

* Detects high-risk emotional patterns
* Automatic crisis event logging
* Instant display of mental health helplines
* Emergency support recommendations

### 🔐 Secure Authentication

* JWT-based authentication
* Password hashing with bcrypt
* Secure login and registration
* Protected user data

### ☁️ Firebase Integration

* Cloud-based storage
* User-specific chat history
* Crisis log management
* Automatic fallback to Demo Mode

---

## 🏗️ System Architecture

Frontend (HTML/CSS/JavaScript)

⬇️

FastAPI Backend

⬇️

Sentiment Analysis Engine

⬇️

Firebase Firestore / Mock Database

---

## 📂 Project Structure

```text
MindEase/
├── backend/
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   ├── auth_utils.py
│   ├── sentiment.py
│   ├── requirements.txt
│   ├── .env.example
│   └── routers/
│       ├── auth.py
│       ├── chat.py
│       └── crisis.py
│
├── frontend/
│   └── templates/
│       └── index.html
│
├── assets/
│   ├── screenshots/
│   └── demo-video.mp4
│
└── README.md
```

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend

* Python
* FastAPI

### Database

* Firebase Firestore
* In-Memory Mock Database

### Authentication

* JWT Tokens
* bcrypt

### AI & Analytics

* Custom Sentiment Analysis Engine
* Emotional Trend Tracking
* Crisis Detection System

---

## ⚡ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/MindEase.git
cd MindEase
```

### Install Dependencies

```bash
cd backend
pip install -r requirements.txt
```

### Configure Environment

```bash
cp .env.example .env
```

Update values inside `.env`.

---

## 🔥 Firebase Setup (Optional)

1. Create a Firebase project.
2. Open Project Settings.
3. Navigate to Service Accounts.
4. Generate a Private Key.
5. Download the JSON file.
6. Rename it:

```text
firebase_credentials.json
```

7. Place it inside:

```text
backend/
```

---

## ▶️ Running the Application

```bash
cd backend
python main.py
```

Open:

```text
http://localhost:8000
```

---

## 📡 API Endpoints

### Authentication

| Method | Endpoint           | Description   |
| ------ | ------------------ | ------------- |
| POST   | /api/auth/register | Register user |
| POST   | /api/auth/login    | Login         |
| GET    | /api/auth/me       | Current user  |

### Chat

| Method | Endpoint          | Description      |
| ------ | ----------------- | ---------------- |
| POST   | /api/chat/send    | Send message     |
| GET    | /api/chat/history | Get chat history |
| DELETE | /api/chat/history | Clear history    |

### Crisis

| Method | Endpoint                      | Description    |
| ------ | ----------------------------- | -------------- |
| GET    | /api/crisis/logs              | Crisis records |
| PATCH  | /api/crisis/logs/{id}/resolve | Resolve crisis |
| GET    | /api/crisis/helplines         | Helpline list  |

---

## 📚 API Documentation

Swagger UI:

```text
http://localhost:8000/docs
```

ReDoc:

```text
http://localhost:8000/redoc
```

---

## 🧪 Demo Mode

MindEase automatically switches to Demo Mode if Firebase credentials are unavailable.

Features supported:

* Authentication
* Chat
* Sentiment Analysis
* Crisis Detection
* Emotional Trend Visualization

No additional setup required.

---

## ☎️ Mental Health Helplines (India)

| Organization          | Contact       |
| --------------------- | ------------- |
| iCall                 | 9152987821    |
| Vandrevala Foundation | 1860-2662-345 |
| NIMHANS               | 080-46110007  |
| Snehi                 | 044-24640050  |

---

## 🎥 Demo Video

Add your project demonstration video here:

[Watch Demo Video](https://your-demo-link.com)

---

## 📸 Screenshots

### Home Dashboard

![Uploading image.png…]()


### Sentiment Wave

![Sentiment Wave](assets/screenshots/sentiment-wave.png)

### Crisis Detection

![Crisis Detection](assets/screenshots/crisis-alert.png)

---

## 🎯 Problem Statement

Mental health support remains inaccessible for millions due to cost, stigma, and limited availability of professional resources.

---

## 💡 Our Solution

MindEase bridges this gap through an AI-powered platform that provides:

* Emotional awareness
* Mental wellness tracking
* Crisis identification
* Immediate support resources
* Accessible and stigma-free interaction

---

## 🌍 Impact

* Early detection of emotional distress
* Increased mental health awareness
* Accessible support for students and professionals
* Encourages proactive emotional self-care

---

## 🔮 Future Scope

* Multilingual support
* Voice-based sentiment analysis
* AI therapist integration
* Mobile application
* Advanced emotional analytics
* Personalized wellness recommendations

---

## 👥 Team

PS06 Hackathon Team

Building technology that cares about people.

---

## 📜 License

This project is licensed under the MIT License.
