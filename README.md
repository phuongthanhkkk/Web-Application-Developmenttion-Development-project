# Web-Application-Developmenttion-Development-project

These projects were completed in the *Web Application Development (IT093IU)* course. The project—**DrawVoice Meeting**—combines a collaborative drawing board with real-time voice chat, enabling teams to communicate visually and verbally within virtual meeting rooms.

---

## Table of Contents
- [Project Overview](#project-overview)  
- [Contributors](#contributors)
- [Work Breakdown Structure](#work-breakdown-structure)  
- [Use Case Diagram](#use-case-diagram)  
- [Sequence Diagrams](#sequence-diagrams)  
- [MVC Architecture](#mvc-architecture)  
- [Entity-Relationship Diagram (ERD)](#entity-relationship-diagram-erd)  
- [Class Diagram](#class-diagram)  
- [Implementation Highlights](#implementation-highlights)  
- [Security & Session Management](#security--session-management)  
- [Conclusion](#conclusion)

---

## Project Overview

**Project Name:** DrawVoice Meeting  
**Team Name:** We Can Draw  
**Platform:** Real-time collaborative web application  
**Main Project:** check out this repo: https://github.com/huynhtrankhanh/WeCanDraw

**For live demo:** go to this website https://abundant-rambunctious-apple.glitch.me/

**Notice:** This repository is for the main meeting logic. For the UI shown before the meeting page, check out this repo: https://github.com/huynhtrankhanh/WeCanDraw-landing

**Key Features:**
- Voice chat using WebSocket and Jitsi  
- Shared drawing canvas with multiple tools  
- Meeting creation and management  
- Secure login/register system  
- Admin features for user and drawing management

---

## Contributors

| Name                | Responsibilities                                        |
|---------------------|----------------------------------------------------------|
| **Bùi Phương Thanh** | Writing report, drawing diagrams, Frontend (HTML, CSS) |
| **Hồ Tiến Đạt**      | Database connection and integration                    |
| **Huỳnh Trần Khanh** | Frontend (JavaScript), Backend logic and integration    |

---

## Work Breakdown Structure  
📎 **File:** `Work Breakdown Structure_WAD.pdf`  

Main components:
- Login System  
- Create Room  
- Join Room  
- Drawboard  
- Voice Chat  

Each task was further divided into subtasks and managed using Scrum methodology.

---

## Use Case Diagram  
📎 **File:** `USE CASE DIAGRAM.drawio.png`  

Actors:
- **User**: Can register, login, join/create rooms, voice chat, draw  
- **Admin**: Manages users, voice chats, drawings  

Key Use Cases:
- Create/Join Room  
- Send/Receive Voice Chat  
- Control Drawboard  
- Share Room ID  
- Update Room Info  
- Manage Users, Voice Chat, Drawings

---

## Sequence Diagrams  
📎 **Files:**  
- `SequenceDiagram-Create Account.drawio`  
- `SequenceDiagram-Login.drawio`  
- `SequenceDiagram-Create Meeting.drawio`  
- `SequenceDiagram-Delete Meeting.drawio`  
- `SequenceDiagram-Join Meeting.drawio`  
- `SequenceDiagram-DrawVoice.drawio`

---

## MVC Architecture  
📎 **File:** `MVC.drawio.png`  

**Model**: Java classes, DB access (User, Meeting, DrawChat)  
**View**: JSP/HTML/JS (User, Meeting, DrawChat pages)  
**Controller**: Java Servlets (login, registration, meeting logic)

---

## Entity-Relationship Diagram (ERD)  
📎 **File:** `ERD.drawio.png`  

Includes:
- `User`, `Meeting`, `MeetingManager`, `DrawChat`  
- Tool attributes (brushTool, textTool, micControl, canvas, etc.)

---

## Class Diagram  
📎 **File:** `ClassDiagram.drawio.png`  

Object-oriented design using:
- Encapsulation via getters/setters  
- Composition & aggregation relationships  
- Classes representing core app logic

---

## Implementation Highlights  

### 🟦 Frontend
- **HTML/CSS** for layout and structure  
- **JavaScript** for real-time interactivity  
- **Canvas API** for drawing features  

### 🟩 Backend
- **Java Servlets** for business logic  
- **MySQL** for persistent storage  
- **Node.js & WebSocket** for drawing & voice features  
- **Jitsi Meet API** for audio conferencing

### 🔁 Real-Time Features
- Live drawing sync via WebSocket  
- Secure meeting links with SHA-256  
- Dynamic room and tool interaction  

---

## Security & Session Management

- Password hashing: PBKDF2 (client-side) + SHA-256 (server-side)  
- Cookies: `HttpOnly`, `Secure`, `SameSite=Strict`  
- Session IDs stored server-side  
- Rate-limiting: Lockout after 5 failed logins

---

## Conclusion

**DrawVoice Meeting** is a powerful collaborative web platform that merges real-time drawing and voice communication. This project challenged us to integrate multiple technologies while following Agile practices and the MVC model. Our solution is secure, interactive, and ready for creative teamwork—paving the way for future development and enhancements.

---

Let me know if you'd like this turned into a GitHub README, printable PDF, or portfolio template!
