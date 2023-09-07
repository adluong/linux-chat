# linux-chat
Linux chat test

A simple chat application for Linux (Ubuntu).
The application comprises two programs:
1. Server.c: Must be run first to initialize the protocol (IP address, port number).
2. Client.c: Run by multiple clients. They connect and send messages to the server. The server will display messages on a blackboard associated with the sender's name.

To compile:

gcc server.c -o server -lpthread -lncurses

./server

gcc client-official.c -o client -lpthread -lncurses

./client
