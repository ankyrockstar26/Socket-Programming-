# Socket-Programming-
Python Socket Programming
Socket programming is a way of connecting two nodes on a network to communicate with each other. 
One socket(node) listens on a particular port at an IP, while other socket reaches out to the other to form a connection. Server forms the listener socket while client reaches out to the server.
They are the real backbones behind web browsing. In simpler terms there is a server and a client.

Client
======
First of all we make a socket object.
Then we connect to localhost on port 12345 (the port on which our server runs) and lastly we receive data from the server and close the connection.
Now save this file as client.py and run it from the terminal after starting the server script.

Server
======
First of all we import socket which is necessary.
Then we made a socket object and reserved a port on our pc.
After that we binded our server to the specified port. 
Passing an empty string means that the server can listen to incoming connections from other computers as well. 
If we would have passed 127.0.0.1 then it would have listened to only those calls made within the local computer.
After that we put the server into listen mode.5 here means that 5 connections are kept waiting if the server is busy and if a 6th socket trys to connect then the connection is refused.
At last we make a while loop and start to accept all incoming connections and close those connections after a thank you message to all connected sockets.
