# Project: Mini-chat on FastAPI

This project is a mini-chat using **FastAPI** to create an API, **SQLAlchemy** to work with a database, and a simple frontend to interact with users. The app contains two main models: a user model and a message model, which allows users to send and receive messages in real time.

## Technology Stack:
- **Backend**: FastAPI
- **Frontend**: HTML/JavaScript
- **ORM**: SQLAlchemy
- Database: Any database supported by SQLAlchemy (e.g., PostgreSQL or SQLite). The example uses SQLite.

## Main components:
1. User Model: Contains user information, including username, email and password.
2. Message Model: Stores messages sent by users, including the time they were sent, the sender, and the body of the message.

## Functionality:
It is a web-based messaging application where users can send and receive real-time messages. Key features include:

1. Authentication: Register and authorize users through HTML and JavaScript forms. APIs are used for data processing and validation.
2. **Chat**: Users can select interlocutors from the list and chat with them. Messages are displayed in the chat window.
3. Sending Messages: Users can send text messages. WebSocket is used for instant message delivery. Old messages are loaded using server polling.
4. Interface: A modern and responsive interface using CSS that provides a seamless experience across devices.
5. **User Management**: Ability to select interlocutors, log out and work with "Favorites" like "Favorites" from telegrams.

## GIF Animation Example

Below is an animation that demonstrates the process of the application:

<img src="demo.gif" width="600" alt="Демонстрация работы мини-чата" />

---

## How to launch a project

### Installing Dependencies:

```bash
pip install -r requirements.txt
```

### Performing Alembic Migrations:

```bash
alembic upgrade head
```
### Project launch:
```bash
uvicorn app.main:app
```