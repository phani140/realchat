# 📡 Real-Time Chat Application

This is a simple real-time chat application built with **Spring Boot**, **WebSockets (STOMP over SockJS)**, and **Vanilla JavaScript** on the frontend. It demonstrates how to set up full-duplex communication between clients through a Spring WebSocket server.

---

## 🚀 Features

- Real-time bi-directional messaging
- Broadcast messages to all connected clients
- Uses SockJS and STOMP for fallback support and messaging abstraction
- Basic user interface built with HTML and Bootstrap

---

## 🛠️ Technologies Used

- Java 17+ / Spring Boot
- Spring WebSocket / STOMP Protocol
- SockJS client
- STOMP.js client
- Bootstrap 5

---

## 📁 Project Structure

├── src
│ └── main
│ ├── java
│ │ └── com.chat.app
│ │ ├── controller
│ │ │ └── ChatController.java
│ │ ├── config
│ │ │ └── WebsocketConfig.java
│ │ └── model
│ │ └── ChatMessage.java
│ └── resources
│ ├── templates
│ │ └── chat.html
│ └── application.properties
├── pom.xml
└── README.md

yaml
Copy
Edit

---

## ⚙️ Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/real-time-chat-app.git
cd real-time-chat-app
2. Build and Run the Application
Make sure you have Java and Maven installed.

bash
Copy
Edit
mvn spring-boot:run
The application will start on:
http://localhost:8080/chat

3. Open in Browser
Access the chat UI:

bash
Copy
Edit
http://localhost:8080/chat
Open multiple tabs or browsers to test real-time communication.

🧪 Testing the Application
Enter your name.

Type a message.

Click Send or press Enter.

Messages appear in all connected browser windows.

📝 Notes
The WebSocket endpoint is registered at /chat.

Application destination prefix is /app.

Messages are published to /topic/messages.

📌 Future Enhancements (Optional)
Private chat rooms

User list and typing indicators

Message persistence using a database (e.g., PostgreSQL, MongoDB)

Authentication (JWT)

