# linux-chat
This is a simple message exchanging program.
It runs on Linux terminal using pthread and ncurses library.

A simple chat application for Linux (Ubuntu).
The application comprises two programs:
1. Server.c: Must be run first to initialize the protocol (IP address, port number).
2. Client.c: Run by multiple clients. They connect and send messages to the server. The server will display messages on a blackboard associated with the sender's name.

**1. Install ncurses**
```
sudo apt-get install libncurses5-dev libncursesw5-dev
```
**2. Compile**
On the server side:
```
gcc server.c -o server -lpthread -lncurses
```
On the client side:
```
gcc client-official.c -o client -lpthread -lncurses
```
**3.Run**
On the server side:
```
./server
```
Each client runs:
```
./client
```
**For more information, please contact: adluong11@korea.ac.kr**
