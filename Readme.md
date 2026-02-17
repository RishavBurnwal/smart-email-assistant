# 📧 Smart Email Assistant – AI-Powered Email Reply Generator

A full-stack web application that generates intelligent, context-aware email replies using **Google Gemini API**.  
Built with **Spring Boot (Backend)** and **React + Material UI (Frontend)**.

---

## 🚀 Overview

Smart Email Assistant allows users to input an email and generate a professional AI-powered reply with selectable tone options such as **Professional**, **Casual**, or **Friendly**.

This project demonstrates full-stack development, REST API design, asynchronous handling, AI integration, and clean UI implementation.

---

## 🛠 Tech Stack

### Frontend
- React
- Material UI
- Axios

### Backend
- Spring Boot
- WebClient (Spring WebFlux)
- Maven

### AI Integration
- Google Gemini API

---

## ✨ Key Features

- AI-generated contextual email replies  
- Tone-based customization (Professional, Casual, Friendly)  
- Loading state management  
- Proper error handling  
- Copy-to-clipboard functionality  
- Secure backend API key configuration  
- Clean and responsive UI  

---

## 🏗 Architecture Flow

React Frontend  
→ REST API Call (Axios)  
→ Spring Boot Backend  
→ WebClient → Gemini API  
→ Response returned to frontend  

---

## 🔌 API Endpoint

### POST `/api/email/generate`

### Request
```json
{
  "emailContent": "Original email text",
  "tone": "professional"
}
```

### Response
```
Generated email reply (String)
```

---

## ⚙️ Local Setup

### 🔹 Backend Setup

```bash
cd email-writer-sb
mvn spring-boot:run
```

Configure in `application.properties`:

```
gemini.api.url=YOUR_API_URL
gemini.api.key=YOUR_API_KEY
```

---

### 🔹 Frontend Setup

```bash
cd email-writer-react
npm install
npm run dev
```

---

## 📌 Future Improvements

- Deployment (Render / Vercel)
- Email history storage (Database integration)
- Authentication (JWT)
- More tone variations

---

## 👨‍💻 Author

**Rishav**  
Full Stack Developer (Java + React)
