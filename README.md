# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
**CLIENT**
```
Developed by: RISHI CHANDRAN R
Reg no: 212223233005
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
**SEVER**
```
import socket 
s=socket.socket() 
s.bind(('localhost',8000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
    ClientMessage=c.recv(1024).decode() 
    c.send(ClientMessage.encode())
```
## OUPUT
![383516917-99eb79b4-01ba-49c4-9b70-ee4c28127ef8](https://github.com/user-attachments/assets/ee733a9f-5d7d-459a-acec-378323b98316)

![383517010-63aedec1-5e08-4603-9a97-a7fe09beb383](https://github.com/user-attachments/assets/45df0fc1-ac60-4ea2-a354-e6bb25b93b7f)


## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
