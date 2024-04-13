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
## PROGRAM:
### CLIENT:
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode()
 ```
### SERVER:
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


## OUTPUT:
### CLIENT:
![WhatsApp Image 2024-04-13 at 11 22 05_c69bf468](https://github.com/sarishvarshan/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/152167665/290508bc-e771-48df-b0e1-e66a851ba0f6)

### SERVER:
![WhatsApp Image 2024-04-13 at 11 22 12_675d9e1d](https://github.com/sarishvarshan/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/152167665/b7848d2a-3b25-4c47-8e71-9bdd019c5de0)



## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
