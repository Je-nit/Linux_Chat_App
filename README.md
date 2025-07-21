# Linux_Chat_App

## 👨‍💻 Project Title
Chatting Application Using FIFO (Named Pipes) and IPC in C

## 🎯 Objective
To design and implement a two-way communication system between two users using FIFO (Named Pipes), enabling them to chat in real-time through inter-process communication in a Linux environment.

## 📝 Project Information:

Communication Type: Inter-process communication (IPC) using named pipes (FIFOs).
Users: Two users (User 1 and User 2), each running the application in separate terminals.
Processes:
Parent process: Sends messages.
Child process: Receives messages (created using fork()).
FIFOs used:
/tmp/user1_fifo: For User 1 to receive messages.
/tmp/user2_fifo: For User 2 to receive messages.
Graceful Exit: Handles SIGINT (Ctrl+C) for proper cleanup of resources.
Duplex Communication: Each user writes to the other’s FIFO and reads from their own.
