# INTERFACING WITH THE RASPBERRY PI

## ALMAAS ZAFAR

## SSH

* Firewall: block some internet ports

* Secure Shell (SSH): Program that allow you to access machine remotely

* Telnet: SSH not secure

* Linus has an SSH client

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
