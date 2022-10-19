# TryHackMe | Agent Sudo

+++++++++++++++++++++++++++++++++++\
IP: 10.10.191.235\
Date: 19-10-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scanning

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196645543-b5c95102-a68d-4b08-b929-449fddc41afa.png">

**Open Ports:**

21  -- FTP        -- vsftp 3.0.3\
22  -- SSH        -- OpenSSH 7.6p1\
80  -- Webserver  -- Apache 2.4.29


### Webserver Enumeration

**Home Pages**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196646679-6bf2e288-b5ce-4ad4-96b1-78429baaee8c.png">

**Change user-agent**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196658918-b0af44e7-9fd7-4fad-8420-8042979a4708.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196658989-17d07ad9-2369-4de3-9858-b41e37957c4b.png">

***Payload letters a-z***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196659428-b1fc8b45-249e-4454-a40c-ba98fbb228d3.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196659591-54022182-96d4-4aac-b7a8-819d931b93fc.png">

***Payload letters A-Z***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196660063-ce711f14-b6c1-4703-a0b9-48522c0f2f3a.png">

***Result agent: C***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196660473-1144276e-9eb4-43e0-b665-70f3bcc5905d.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196660577-3f9a96a0-65e2-4088-83f3-ae5d9db09b2f.png">


***Result agent: R***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/196660777-1c97e252-7459-4e5c-921a-a9086c8740d2.png">

**Nikto Scan**

<img width="646" alt="image" src="https://user-images.githubusercontent.com/115549820/196661142-2da4727f-4ccc-4799-ba84-c496b4871e74.png">

**Dirbuster Scan**

<img width="646" alt="image" src="https://user-images.githubusercontent.com/115549820/196661255-c170f2b9-dbf2-4f7f-902b-8386fb27dd4e.png">

### FTP Enumeration


## Fase 2: Getting Access
