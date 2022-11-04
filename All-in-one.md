# TryHackMe | All in one

+++++++++++++++++++++++++++++++++++\
IP: 10.10.211.23\
Date: 01-11-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scan

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199254565-571afee0-df87-43b5-b383-3ecb29b92798.png">

**Open Ports**

21 - FTP - vsftpd 3.0.3\
22 - SSH - OpenSSH 7.6p1\
80 - Webserver - Apache 2.4.29

### FTP Enumeration

<img width="350" alt="image" src="https://user-images.githubusercontent.com/115549820/199951387-fe7db85f-ebab-4449-ad98-3c3648d1dcb1.png">

### Webserver Enumeration

**Nikto Output**

<img width="750" alt="image" src="https://user-images.githubusercontent.com/115549820/199948803-db84a1f4-2107-42b7-aa9b-051e539f05bd.png">

**Dirbuster Output**

<img width="759" alt="image" src="https://user-images.githubusercontent.com/115549820/199948930-6cff5d1e-c9f7-4cb5-8a6d-90d25140ed1c.png">

**Homepage**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199949038-edc9dcc6-f364-407f-bcf4-c5f2bd1697f9.png">

**WordPress**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199949204-30eaea03-6bb8-440b-b26a-546783fe86f2.png">

***WP-login***

<img width="407" alt="image" src="https://user-images.githubusercontent.com/115549820/199952141-7462129f-c415-4a55-870f-519f216688f8.png">

***Possible username***

> elyana

**Wpscan**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199950233-4b5cffd8-7300-499b-8d30-05d80d427ad3.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199950341-14bf3095-15ec-4a40-8ee8-000d71a18cfb.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199950417-ba9575e2-e722-402c-a242-1843e00ca643.png">


## Fase 2: Getting Access

  
## Fase 3: Intern Enumeration

  
## Fase 4: PrivEsc
  
## TryHackMe Questions
