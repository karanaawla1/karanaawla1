<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0d1117,100:0d1117&height=20&section=header" width="100%"/>

</div>

```
╔═══════════════════════════════════════════════════════════════════════╗
║                                                                       ║
║        ██╗  ██╗ █████╗ ██████╗  █████╗ ███╗  ██╗   █████╗ ██████╗  ║
║        ██║ ██╔╝██╔══██╗██╔══██╗██╔══██╗████╗ ██║  ██╔══██╗██╔══██╗ ║
║        █████╔╝ ███████║██████╔╝███████║██╔██╗██║  ███████║██████╔╝ ║
║        ██╔═██╗ ██╔══██║██╔══██╗██╔══██║██║╚████║  ██╔══██║██╔═══╝  ║
║        ██║  ██╗██║  ██║██║  ██║██║  ██║██║  ███║  ██║  ██║██║      ║
║        ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚══╝  ╚═╝  ╚═╝╚═╝      ║
║                                                                       ║
║              [ Java Backend Developer  •  v1.0.0-SNAPSHOT ]          ║
║                    [ Status: 🟢 RUNNING • Open To Work ]             ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=16&duration=2000&pause=500&color=00FF88&center=true&vCenter=true&width=700&lines=Welcome+to+KARAN.API+—+Developer+Documentation+v1.0;Base+URL%3A+https%3A%2F%2Flinkedin.com%2Fin%2Fkaranaawla;All+endpoints+return+JSON+%7C+Auth%3A+DM+on+LinkedIn;GET+%2Fkaran%2Fhire+→+200+OK+%F0%9F%9A%80)](https://git.io/typing-svg)

<br/>

![](https://img.shields.io/badge/API_VERSION-v1.0.0--SNAPSHOT-00FF88?style=for-the-badge&labelColor=0d1117&color=00FF88)
&nbsp;
![](https://img.shields.io/badge/STATUS-200_OK_🟢-00FF88?style=for-the-badge&labelColor=0d1117)
&nbsp;
![](https://img.shields.io/badge/CONTENT__TYPE-application%2Fjson-00BFFF?style=for-the-badge&labelColor=0d1117)
&nbsp;
<img src="https://komarev.com/ghpvc/?username=karanaawla1&style=for-the-badge&color=FF6B6B&label=API+CALLS&labelColor=0d1117"/>

</div>

---

<div align="center">

## 📡 &nbsp; `BASE URL`

```
https://github.com/karanaawla1
```

| Method | Endpoint | Description | Auth |
|:------:|:---------|:------------|:----:|
| `GET` | [`/karan/info`](#-get-karaninfo) | Who is this guy? | None |
| `GET` | [`/karan/stack`](#-get-karanstack) | Tech skills | None |
| `GET` | [`/karan/projects`](#-get-karanprojects) | Things I built | None |
| `GET` | [`/karan/journey`](#-get-karanjourney) | My story | None |
| `GET` | [`/karan/status`](#-get-karanstatus) | Current availability | None |
| `POST` | [`/karan/hire`](#-post-karanhire) | **Hire me** 🚀 | **Required** |

</div>

---

## 🟢 `GET` &nbsp;`/karan/info`

> Returns developer profile information

**Response `200 OK`:**

```json
{
  "name"       : "Karan Aawla",
  "role"       : "Java Backend Developer",
  "location"   : "Hyderabad, India 🇮🇳",
  "education"  : "B.Tech ECE — LNCTS Bhopal (2025)",
  "training"   : "Java Full Stack @ Ashok IT",
  "available"  : true,
  "response_time" : "Fast — I check LinkedIn obsessively 😅",

  "personality" : {
    "type"      : "Builder",
    "trait"     : "Ships things to cloud, not just localhost",
    "weakness"  : "CSS (please don't ask)",
    "superpower": "Turning caffeine into Spring Boot APIs"
  },

  "fun_facts" : [
    "ECE grad who opened Java docs by accident and never closed the tab",
    "My first Spring Boot app had 47 StackOverflow tabs open",
    "I consider a successful deployment a personal victory 🏆",
    "404: Work-Life Balance Not Found"
  ],

  "contact" : {
    "linkedin" : "linkedin.com/in/karanaawla",
    "github"   : "github.com/karanaawla1",
    "email"    : "karanaawla1@gmail.com"
  }
}
```

<div align="right">
<a href="https://linkedin.com/in/karanaawla"><img src="https://img.shields.io/badge/Try_it_→_LinkedIn-0A66C2?style=flat-square&logo=linkedin"/></a>
<a href="mailto:karanaawla1@gmail.com"><img src="https://img.shields.io/badge/Try_it_→_Gmail-EA4335?style=flat-square&logo=gmail"/></a>
</div>

---

## 🟢 `GET` &nbsp;`/karan/stack`

> Returns complete technology stack with proficiency metadata

**Response `200 OK`:**

```json
{
  "backend": {
    "primary"  : ["Java 17", "Spring Boot 3", "Spring Security", "Hibernate/JPA"],
    "secondary": ["Python", "Flask"],
    "expertise": "⭐⭐⭐⭐☆",
    "note"     : "This is where I live"
  },

  "database": {
    "relational"  : ["MySQL", "PostgreSQL", "H2"],
    "tools"       : ["Spring Data JPA", "Hibernate ORM"],
    "expertise"   : "⭐⭐⭐⭐☆"
  },

  "security": {
    "auth"        : ["JWT", "Spring Security", "BCrypt"],
    "patterns"    : ["RBAC", "Stateless Sessions", "Token Refresh"],
    "expertise"   : "⭐⭐⭐⭐☆"
  },

  "devops": {
    "containerization" : ["Docker", "Docker Hub"],
    "orchestration"    : ["Red Hat OpenShift", "Kubernetes (learning)"],
    "cicd"             : ["GitHub Actions"],
    "cloud"            : ["Render", "Microsoft Azure", "Supabase"],
    "expertise"        : "⭐⭐⭐☆☆",
    "note"             : "Growing fast — currently on OpenShift"
  },

  "build_tools" : ["Maven", "Git", "Postman"],
  "frontend"    : ["React (basic)", "HTML", "CSS (reluctantly 😭)"]
}
```

<div align="center">
<br/>

[![Skills](https://skillicons.dev/icons?i=java,spring,hibernate,maven,mysql,postgresql,docker,kubernetes,githubactions,azure,git,react&theme=dark&perline=12)](https://skillicons.dev)

</div>

---

## 🟢 `GET` &nbsp;`/karan/projects`

> Returns list of projects with metadata, status, and live URLs

**Response `200 OK`:**

```json
{
  "total": 4,
  "all_deployed": true,
  "projects": [
```

<br/>

<table width="100%">
<tr>
<td width="50%" valign="top">

```json
{
  "id"      : "PROJECT_001",
  "name"    : "SmartAssist",
  "type"    : "AI Chatbot Backend",
  "status"  : "🟢 LIVE",

  "highlights": [
    "Groq LLaMA 3 AI integration",
    "Real-time responses + history",
    "JWT secured endpoints",
    "Dockerized + cloud deployed",
    "Animated React frontend"
  ],

  "stack": ["Java", "Spring Boot",
    "Groq API", "JWT", "Docker",
    "H2", "React"],

  "urls": {
    "github": "github.com/karanaawla1/
              SmartAssist-AI-Chatbot",
    "live"  : "smartassist-ai-chatbot
              .onrender.com"
  }
}
```

<p align="center">
<a href="https://github.com/karanaawla1/SmartAssist-AI-Chatbot"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github"/></a>&nbsp;
<a href="https://smartassist-ai-chatbot.onrender.com"><img src="https://img.shields.io/badge/LIVE-00FF88?style=for-the-badge"/></a>
</p>

</td>
<td width="50%" valign="top">

```json
{
  "id"      : "PROJECT_002",
  "name"    : "SmartDesk",
  "type"    : "Helpdesk Ticketing System",
  "status"  : "✅ COMPLETE",

  "highlights": [
    "JWT + RBAC (Admin / User)",
    "Full ticket lifecycle mgmt",
    "Open→InProgress→Resolved",
    "Spring Security patterns",
    "Production-grade structure"
  ],

  "stack": ["Java", "Spring Boot",
    "Spring Security", "JWT",
    "MySQL", "Hibernate"],

  "urls": {
    "github": "github.com/karanaawla1/
              SmartDesk-Helpdesk-System"
  }
}
```

<p align="center">
<a href="https://github.com/karanaawla1/SmartDesk-Helpdesk-System"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github"/></a>
</p>

</td>
</tr>
<tr>
<td width="50%" valign="top">

```json
{
  "id"      : "PROJECT_003",
  "name"    : "StudentResultSystem",
  "type"    : "OpenShift REST API",
  "status"  : "🔄 IN PROGRESS",

  "highlights": [
    "Red Hat OpenShift deploy",
    "Supabase PostgreSQL cloud",
    "Pass/Fail auto-calculation",
    "GitHub Actions CI/CD",
    "Zero-downtime rolling deploy"
  ],

  "stack": ["Java", "Spring Boot",
    "PostgreSQL", "OpenShift",
    "Docker", "GitHub Actions"],

  "urls": {
    "github": "coming soon..."
  }
}
```

<p align="center">
<a href="https://github.com/karanaawla1"><img src="https://img.shields.io/badge/COMING_SOON-FFE66D?style=for-the-badge"/></a>
</p>

</td>
<td width="50%" valign="top">

```json
{
  "id"      : "PROJECT_004",
  "name"    : "ExpenseTrackerAPI",
  "type"    : "Python Flask REST API",
  "status"  : "🟢 LIVE",

  "highlights": [
    "JWT auth + CRUD endpoints",
    "Analytics routes",
    "Flask Blueprint structure",
    "SQLAlchemy + SQLite",
    "Live on Render"
  ],

  "stack": ["Python", "Flask",
    "JWT", "SQLite",
    "SQLAlchemy", "Render"],

  "urls": {
    "live": "expense-tracker-api-
            wqp5.onrender.com"
  }
}
```

<p align="center">
<a href="https://expense-tracker-api-wqp5.onrender.com"><img src="https://img.shields.io/badge/LIVE-00FF88?style=for-the-badge"/></a>
</p>

</td>
</tr>
</table>

```json
  ] // end projects array
}
```

---

## 🟢 `GET` &nbsp;`/karan/journey`

> Returns developer timeline and growth story

**Response `200 OK`:**

```json
{
  "started_from" : "ECE Engineering (not even CS 💀)",
  "current_level": "Production-grade backend developer",
  "time_taken"   : "~12 months",

  "timeline": [
    {
      "period": "Early 2025",
      "event" : "Opened Java docs for the first time",
      "result": "Hello World printed. Life changed. 😭"
    },
    {
      "period": "Mid 2025",
      "event" : "Discovered Spring Boot",
      "result": "SmartDesk — full JWT + RBAC ticketing system"
    },
    {
      "period": "Late 2025",
      "event" : "Added AI integration",
      "result": "SmartAssist — live AI chatbot on Render"
    },
    {
      "period": "Feb 2026",
      "event" : "Got Docker certification",
      "result": "Docker Foundations Professional ✅"
    },
    {
      "period": "Mar 2026",
      "event" : "Discovered OpenShift",
      "result": "StudentResultSystem — CI/CD, rolling deploys"
    },
    {
      "period": "NOW",
      "event" : "Looking for first job",
      "result": "Please help. DM me. 🙏"
    }
  ],

  "summary": "ECE grad. No CS degree. No internship.
              Just 4 deployed projects and a ton of hope. 🚀"
}
```

---

## 🟢 `GET` &nbsp;`/karan/status`

> Returns real-time availability and current focus

**Response `200 OK`:**

```json
{
  "available"       : true,
  "response_time"   : "< 24 hours (usually in minutes)",
  "preferred_mode"  : "LinkedIn DM or Email",

  "seeking": {
    "roles"  : ["Associate Software Engineer",
                "Java Backend Developer",
                "Backend Developer"],
    "cities" : ["Hyderabad (preferred ⭐)",
                "Pune", "Noida"],
    "type"   : "Full-time"
  },

  "currently_learning": [
    "Microservices Architecture",
    "OpenShift + Kubernetes",
    "System Design Fundamentals"
  ],

  "currently_building": [
    "StudentResultSystem → OpenShift (in progress)",
    "NexTalk → Real-time Chat App (planned)"
  ],

  "certifications": [
    "🐳 Docker Foundations Professional — 2026 ✅",
    "☁️  Microsoft Azure AI Essentials  — 2025 ✅",
    "🟨  HackerRank SQL Basic           — 2025 ✅"
  ]
}
```

---

## 🔴 `POST` &nbsp;`/karan/hire`

> Initiates hiring process. **This is the most important endpoint.**

**Request Body:**

```json
{
  "company"  : "YOUR_COMPANY_NAME",
  "role"     : "Java Backend Developer (or similar)",
  "location" : "Hyderabad | Pune | Noida | Remote",
  "message"  : "Hey Karan, we'd like to talk..."
}
```

**Response `200 OK`:**

```json
{
  "status"  : "APPLICATION_RECEIVED",
  "message" : "Karan has been notified and is doing a happy dance 💃",
  "eta"     : "Will reply within 24 hours. Probably less.",
  "next"    : "Interview → Offer → Dream Job 🚀"
}
```

**Response `404 Not Found`:**

```json
{
  "error"   : "OPPORTUNITY_NOT_FOUND",
  "message" : "That's okay. Karan will keep building. 💪"
}
```

<div align="center">

<br/>

<a href="https://linkedin.com/in/karanaawla">
<img src="https://img.shields.io/badge/POST_/karan/hire_→_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0d1117"/>
</a>
&nbsp;
<a href="mailto:karanaawla1@gmail.com">
<img src="https://img.shields.io/badge/POST_/karan/hire_→_Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0d1117"/>
</a>

</div>

---

<div align="center">

```
╔══════════════════════════════════════════════════════════╗
║                                                          ║
║   KARAN.API  •  v1.0.0-SNAPSHOT  •  © 2026              ║
║                                                          ║
║   All endpoints are free to call.                        ║
║   POST /karan/hire is highly encouraged.                 ║
║                                                          ║
║   Built with: Java ☕ + Spring Boot 🍃 + Hope 🙏         ║
║   Deployed on: Cloud (not localhost, I promise)  🚀      ║
║                                                          ║
╚══════════════════════════════════════════════════════════╝
```

<br/>

![](https://img.shields.io/badge/Made_with_☕_by-Karan_Aawla-00FF88?style=flat-square&labelColor=0d1117)
&nbsp;
![](https://img.shields.io/badge/404-Unemployment_Not_Found-FF6B6B?style=flat-square&labelColor=0d1117)
&nbsp;
<img src="https://komarev.com/ghpvc/?username=karanaawla1&style=flat-square&color=00FF88&label=API+CALLS&labelColor=0d1117"/>

</div>
