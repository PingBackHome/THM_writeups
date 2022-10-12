# TryHackMe | Pickle Rick

+++++++++++++++++++++++++++++++++++\
IP: 10.10.171.24\
Date: 12-10-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scanning

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195342710-e2607866-92fc-43d0-942b-dfc15a857699.png">

**Open Ports:**

22    SSH         - OpenSSH 7.2p2\
80    Webserver   - Apache 2.4.18\

### Webserver Enumeration

**Home Pages**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195343454-0b611152-0ce2-4ce9-8d24-f21dfcb527d7.png">

**Home Page Source Code**

<img width="250" alt="image" src="https://user-images.githubusercontent.com/115549820/195343706-65744c5f-476c-4dee-8018-54bb0de19791.png">

>Username: R1ckRul3s

**Nikto Scan**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195345488-ee1fd010-59b3-41e9-90d7-cebd81ba7a62.png">

**Dirbuster Scan**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195345111-a80855b4-59c4-490f-a5a8-1976588a398d.png">

**Results Web Enumeration**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195345780-a306b3c8-67bf-47db-bedf-d8049eaeb6bf.png">


<img width="522" alt="image" src="https://user-images.githubusercontent.com/115549820/195347190-3f75e059-f166-4962-8b4c-710fa1ff52a4.png">

## Fase 2: Getting Access

**Hydra ssh cracking**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195347763-c71a26dd-286c-41ca-8551-fd1e7f30a115.png">

**Login at webportal**

>Username: R1ckRul3s\
>Password: Wubbalubbadubdub

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195348182-b14ed1b3-27a1-4322-9a23-9eafa44d78e3.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195348386-8e83faa2-01a5-4740-a07a-baf81cc66441.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195348819-b25e638c-e53e-4768-8667-dcd99d6746e3.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195350051-5631c1e9-7e7f-4987-8caf-0e6e09fa6cde.png">

<img width="260" alt="image" src="https://user-images.githubusercontent.com/115549820/195350600-384b633d-355f-4241-8028-b0fc69420586.png">

<img width="293" alt="image" src="https://user-images.githubusercontent.com/115549820/195352009-65f817f3-a6e7-4b8e-86e0-9c37c7040354.png">


