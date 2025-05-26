# ✉️ Email Writer Extension using AI

An intelligent Chrome extension that helps users generate professional email replies using AI. Built with a React-based frontend and a Spring Boot backend.

---

## 📌 Features

- 🧠 AI-generated email replies based on the current email content
- 📩 Detects Gmail compose window automatically
- ⚡ One-click "AI-Reply" button injected into Gmail UI
- 🌐 Frontend built using JavaScript (content script)
- 🚀 Backend built with Spring Boot + Gemini API integration

---

## 🏗️ Project Structure

email-writer/
├── frontend/ # Chrome extension frontend (JS, content-script.js)
├── backend/ # Spring Boot backend server (API for generating replies)
├── README.md # Project documentation
└── .gitignore


## 🛠️ How to Run

### ✅ Prerequisites

- Node.js & npm
- Java 17+ and Maven
- Chrome browser
- IntelliJ IDEA (recommended for backend)
- Visual Studio Code (recommended for frontend)

---

### 🚀 Backend (Spring Boot)

1. Navigate to `backend/`
2. Open in IntelliJ or VS Code
3. Run the application:
   ```bash
   mvn spring-boot:run
The API will run at: http://localhost:8080/api/email/generate

🌐 Frontend (Chrome Extension)
1.Navigate to frontend/
2.In Chrome, go to: chrome://extensions/
3.Enable Developer Mode
4.Click Load Unpacked
5.Select the frontend/ folder
6.Open Gmail — you should see the AI-Reply button in compose window

🔌 API Endpoint
POST /api/email/generate

Request Body:

json
Copy code
{
  "emailContent": "Your email text here",
  "tone": "professional"
}

Response: AI-generated reply (plain text)

