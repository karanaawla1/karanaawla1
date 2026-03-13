<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=32&duration=3000&pause=1000&color=A855F7&center=true&vCenter=true&width=500&lines=🤖+SmartAssist;AI+Chatbot+System;Built+with+Spring+Boot;Powered+by+Groq+LLM" alt="Typing SVG" />

<br/>

<p>
  <img src="https://img.shields.io/badge/Java-17-orange?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-4.0-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Groq-LLaMA%203-6E40C9?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Deployed-Render-46E3B7?style=for-the-badge&logo=render&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"/>
</p>

<p>
  <a href="https://smartassist-ai-chatbot.onrender.com">
    <img src="https://img.shields.io/badge/🌐 Live Demo-Click Here-A855F7?style=for-the-badge"/>
  </a>
  &nbsp;
  <a href="https://github.com/karanaawla1/SmartAssist-AI-Chatbot">
    <img src="https://img.shields.io/badge/💻 GitHub-Source Code-181717?style=for-the-badge&logo=github"/>
  </a>
</p>

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

</div>

<br/>

## 🧠 What is SmartAssist?

**SmartAssist** is a production-ready AI-powered chatbot system built from scratch using **Java & Spring Boot**. It integrates with the **Groq LLM API (LLaMA 3)** to generate intelligent, real-time responses to any question a user asks.

Every conversation is stored in a database with full session history support. A clean, animated frontend chat UI is served directly from the Spring Boot backend — no separate frontend server needed.

> Think of it as a lightweight ChatGPT — designed and built entirely by a Java backend developer. 🚀

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

## ✨ Features

<img align="right" src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="280"/>

- 🤖 &nbsp; **AI-Powered Chat** — Real-time answers via Groq LLaMA 3
- 💬 &nbsp; **Conversation History** — All chats stored with session ID & timestamp
- 🌐 &nbsp; **Integrated Frontend** — Animated chat UI built into Spring Boot
- 🏗️ &nbsp; **Clean MVC Architecture** — Controller → Service → Repository
- ⚠️ &nbsp; **Global Exception Handling** — Clean, structured error responses
- 🔐 &nbsp; **Secure Config** — API keys via environment variables, never hardcoded
- 🐳 &nbsp; **Dockerized** — Containerized for easy deployment anywhere
- ☁️ &nbsp; **Cloud Deployed** — Live on Render, auto-deploys on every push

<br/>
<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|:---:|:---:|:---:|
| 💻 Language | Java 17 | Core backend language |
| ⚙️ Framework | Spring Boot 4.0 | Application framework |
| 🗄️ ORM | Spring Data JPA + Hibernate | Database interaction |
| 💾 Database | H2 (File Mode) | Persistent chat storage |
| 🤖 AI | Groq API — LLaMA 3 | Intelligent responses |
| 🌐 Frontend | HTML + CSS + JavaScript | Animated chat UI |
| 🔨 Build Tool | Maven | Dependency management |
| 🐳 Container | Docker | Deployment packaging |
| ☁️ Cloud | Render | Hosting & auto-deploy |
| 🧪 Testing | Postman | API validation |
| 📁 Version Control | Git + GitHub | Source management |

</div>

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

## 🏗️ System Architecture

```
┌──────────────────────────────────────────────────┐
│               Client (Browser)                    │
│         https://smartassist-ai-chatbot.onrender.com│
└─────────────────────┬────────────────────────────┘
                      │  HTTP Request (JSON)
                      ▼
┌──────────────────────────────────────────────────┐
│             ChatController.java                   │
│          @RestController  /api/chat               │
│    POST /api/chat  |  GET /api/chat/history/{id}  │
└─────────────────────┬────────────────────────────┘
                      │
                      ▼
┌──────────────────────────────────────────────────┐
│              ChatService.java                     │
│        Business Logic + Groq API Integration      │
└────────────┬─────────────────────┬───────────────┘
             │                     │
             ▼                     ▼
┌────────────────────┐   ┌─────────────────────────┐
│  ChatRepository    │   │     Groq LLM API         │
│  Spring Data JPA   │   │    LLaMA 3 Model         │
└────────┬───────────┘   └─────────────────────────┘
         │
         ▼
┌────────────────────┐
│    H2 Database     │
│   chat_messages    │
│  (session history) │
└────────────────────┘
```

<br/>

### 📁 Project Structure

```
src/
├── main/
│   ├── java/com/smartassist/
│   │   ├── SmartassistApplication.java         ← Entry point
│   │   ├── controller/
│   │   │   └── ChatController.java             ← REST endpoints
│   │   ├── service/
│   │   │   └── ChatService.java                ← Core logic + AI call
│   │   ├── repository/
│   │   │   └── ChatRepository.java             ← DB queries
│   │   ├── model/
│   │   │   └── ChatMessage.java                ← JPA entity
│   │   ├── dto/
│   │   │   ├── ChatRequest.java                ← Input DTO
│   │   │   └── ChatResponse.java               ← Output DTO
│   │   └── exception/
│   │       └── GlobalExceptionHandler.java     ← Error handling
│   └── resources/
│       ├── static/
│       │   └── index.html                      ← Chat UI (Frontend)
│       └── application.properties              ← Config
```

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

## 📡 API Reference

### `POST /api/chat` — Send a Message

**Request Body**
```json
{
  "sessionId": "user123",
  "message": "What is Spring Boot?"
}
```

**Response**
```json
{
  "sessionId": "user123",
  "reply": "Spring Boot is an open-source Java framework that simplifies building and deploying applications...",
  "timestamp": "2026-03-13T06:44:51.068914700"
}
```

---

### `GET /api/chat/history/{sessionId}` — Get Chat History

**Response**
```json
[
  {
    "id": 1,
    "sessionId": "user123",
    "userMessage": "What is Spring Boot?",
    "botResponse": "Spring Boot is an open-source Java framework...",
    "timestamp": "2026-03-13T06:44:51"
  }
]
```

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

## 🚀 Getting Started

### Prerequisites
- Java 17+
- Maven 3.6+
- Groq API Key — [Get it free here](https://console.groq.com)

### 1. Clone the Repository
```bash
git clone https://github.com/karanaawla1/SmartAssist-AI-Chatbot.git
cd SmartAssist-AI-Chatbot
```

### 2. Configure Environment
Create `src/main/resources/application.properties`:
```properties
spring.application.name=smartassist

spring.datasource.url=jdbc:h2:file:./smartassist-db
spring.datasource.driver-class-name=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.h2.console.enabled=true

GROQ_API_KEY=YOUR_GROQ_API_KEY_HERE
GROQ_API_URL=https://api.groq.com/openai/v1/chat/completions
```

### 3. Run the Application
```bash
./mvnw spring-boot:run
```

### 4. Open in Browser
```
http://localhost:8080
```

<br/>

## 🐳 Docker

```bash
# Build image
docker build -t smartassist .

# Run container
docker run -p 8080:8080 \
  -e GROQ_API_KEY=your_key_here \
  smartassist
```

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

## 🔮 Future Improvements

- [ ] Switch to PostgreSQL for production
- [ ] Add JWT-based user authentication
- [ ] Implement multi-turn conversation memory
- [ ] React frontend for richer UX
- [ ] Rate limiting per session
- [ ] Unit & Integration tests

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

## 👨‍💻 Author

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=A855F7&center=true&vCenter=true&width=400&lines=Karan+Aawla;Java+Backend+Developer;Open+To+Work+🚀" alt="Author Typing SVG" />

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-karanaawla1-181717?style=for-the-badge&logo=github)](https://github.com/karanaawla1)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/karanaawla)

</div>

<br/>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"/>

<br/>

<div align="center">

### ⭐ If you found this helpful, please star the repository! ⭐

<img src="https://forthebadge.com/images/badges/built-with-love.svg"/>
&nbsp;
<img src="https://forthebadge.com/images/badges/made-with-java.svg"/>

</div>
