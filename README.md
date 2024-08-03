
# ChatBuzz - Online Chat Application

## Introduction
ChatBuzz is a simple online chat application developed using Java. It allows multiple users to connect to a central server, send messages, and receive messages from other users. This project assesses skills in socket programming, client-server communication, and user interface design.

## Prerequisites
- Java Development Kit (JDK) installed on your machine.
- A terminal or command prompt for running the application.

## How to Compile and Run

### Server
1. Open a terminal or command prompt.
2. Navigate to the directory containing the `ChatServer.java` file.
3. Compile the server code using the following command:
   ```bash
   javac server/ChatServer.java
   ```
4. Run the server using the following command:
   ```bash
   java server.ChatServer
   ```

### Client
1. Open a terminal or command prompt.
2. Navigate to the directory containing the `ChatClient.java` file.
3. Compile the client code using the following command:
   ```bash
   javac client/ChatClient.java
   ```
4. Run the client using the following command:
   ```bash
   java client.ChatClient
   ```
5. Repeat steps 1-4 in separate terminal or command prompt windows to simulate multiple clients.

## Architecture
The application consists of two main components:
1. **Server (`ChatServer`)**: Manages connections from multiple clients and broadcasts messages to all connected clients.
2. **Client (`ChatClient`)**: Connects to the server, sends messages to the server, and receives messages from other clients.

## Assumptions
- The server runs on `127.0.0.1` and listens on port `12345`.
- The client connects to the server using the same IP and port.

## Usage
- After starting the server, open multiple clients.
- Type messages in one client and press Enter to send the message.
- Messages will be broadcasted to all connected clients.
- Close a client window to simulate client disconnection.
