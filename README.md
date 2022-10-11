# TryHackMe | Basic Pentesting

##  Fase 1: Recon

### Nmap scanning

<img width="797" alt="image" src="https://user-images.githubusercontent.com/115549820/195089832-0544726d-91cd-4c09-8301-2b024b6cf2f2.png">

Open ports:
22        SSH         - OpenSSH 7.2p2\n
80        Webserver   - Apache httpd 2.4.18
139       Samba       - smbd 3.x
445       Samba       - smbd 4.3.11
8009      Ajp13       - Apache Jserv (protocol v1.3)
8080      Webserver   - Apache Tomcat 9.0.7

### SMB enumeration
