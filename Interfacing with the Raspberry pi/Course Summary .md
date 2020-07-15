# INTERFACING WITH THE RASPBERRY PI

## ALMAAS ZAFAR

## SSH

* Firewall: block some internet ports

* Secure Shell (SSH): Program that allow you to access machine remotely

* Telnet: SSH not secure

* Linux has an SSH client

* RPie has an SSH server

* ssh userName@IPAddress #Of server machine #Run SSH Client

* SSHDeamon: A process that waits a client to request a connection (not enabled by default)

* ifconfig #Get RPie IP address (wlan0) #Because it doesn’t have a DN

* PS: IP address changes every time we reboot the RPie


## PROTOCOLS

■ Protocol: Set of rules defining:

  – How data should be transferred

  – What data contained in each packet

■ Every packet contains a header (destination, source) and payload (data)

 – IP: Internet Protocol (Host to host)

 – UDP: Unreliable Datagram Protocol (Complicated, process to process)

 – TCP: Transmission Control Protocol (Simple)

** Port + IP = Internet

■ IPv6 (128 bit) vs IPv4 (32 bit)

■ Ports: (Example: HTTP-80; SSH-22)

■ nslookup domainName #Give IP@ of domainName

■ Domain Name System: Determine between host name (@IP) and domain name (URL)


## SOCKETS

■ Socket: End point of a connection

■ Socket interface: Programming interface to perform network connection  Based on C/S programming

#### Socket client:

  ■ import socket #Socket python library

  ■ ms = socket.socket(sock.AF_INET,socket.SOCK_STREAM) #Create a socket #Arg1: Internet, Arg2: TCP

  ■ host = socket.gethostbyname(“URL”) #Convert URL to IP@

  ■ ms.connect((host,80)) #Create connection to host on port 80

  ■ message = “GET / HTTP/1.1\r\n\r\n” #/: Directory, 1.1: Version, \r\n\r\n: End of session

  ■ ms.sendall(message) #Send data

  ■ data = ms.recv(maxNumberOfBytes) #Recieve HTML data on a blocking wait

  ■ ms.close()
  
 ■  Errors are common with sockets

   try:
      /* code with possible error*/
      except errorType:
      /* executed when error occurs */
    socket.error #Error type that contains all socket errors
    gai.error #Get address info error (when DNS operation occurs)
    Import sys; sys.exit() #To quit the program in case of error
    
■  Socket server: Server need to wait for a request to come in

■ ms.bind(“”,port) #“” to receive from any host, port=1234 for example

■ ms.listen(backLog=numberOfClientsWaitingInLine) #Get ready to accept requests

■ conn, IPaddr = ms.accept() #Accept request to receive and send data

■ conn.sendall() ; conn.recv() ; conn.close() ; ms.close()

■ resp = conn.getresponse(); content = resp.read() #Read content

■ Live server: Server that continues its life (after a request)

■ if data==b’message’ #Convert to byte array because data’s type is a byte array

■ PuTTY: SSH program for Windows

■ NetCat: Program that sends and receives requests

■ nc IP@ Port #Send a request

■ nc –l Port #Listen for a request


#### code_1

    import socket

    import sys

    my sock = socket.socket(socket.AF_INET,socket.SOCK_STREAM)

     try:

     mysock.bind("",1234)

    except socket.error:
    
     print("Failed to bind")
    
     sys.exit()
 
     mysock.listen(5)

    while True:
  
     conn,addr = mysock.accept()
  
     data = conn.recv(1000)
  
     if not data:
  
        break
  
     conn.sendall(data)

     conn.close()

     mysock.close()


####  code_2

    import socket

    import sys

    my sock = socket.socket(socket.AF_INET,socket.SOCK_STREAM)

    except socket.error :
     
     print("Failed to create socket")
         
     sys.exit()
      
      try:
       
       host = socket.gethostbyname("www.google.com")
       
       except  socket.gaierror:
       
       print("failed to get host")
       
       sys.exit()
     
     mysock.connect(host, 80)
     
     message="GET /  HTTP / 1:1\r\n\r\n"
     
     try:
        
        mysock.sendall(message)
     
     except socket.error:
         
         print("failed to send")
      
          sys.exit()
      
      data = mysock.recv(1000)
      
      print(data)
      
      mysock.close()
       
