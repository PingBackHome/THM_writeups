# TryHackMe | Tech_Supp0rt: 1

+++++++++++++++++++++++++++++++++++\
IP: 10.10.148.163\
Date: 11-11-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scan

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201313475-6d329c2a-29a1-4d7f-b814-36fe8b61cb07.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201314084-c987de5e-0ce2-476b-8a38-cad4b7ccfb86.png">

**Open Ports**

22 - SSH - OpenSSH 7.2p2\
80 - Webserver - Apache 2.4.18\
139 - SMB - Samba\
445 - SMB - Samba

### Webserver Enumeration

**Nikto Output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201315997-1da04460-6769-4bc3-9c63-833eddc4503f.png">

**Dirbuster output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201316118-a3b5680a-9fad-4037-85ea-e556c6fdd8a8.png">

***Dirbuster /subrion***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201323878-5f6af11f-0152-4609-a7af-fde5e260fc6d.png">

**wpscan output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201321722-1c956e7f-9c6a-4557-ac8a-a24f83324b44.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201321582-a0d87b9c-cc83-463d-89db-e04ced23c1c5.png">

**/subrion/panel**




### SMB Enumeration

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201317738-d7f81fbc-355d-43b7-bbb5-0ef14b91b5ef.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201317868-6a756e15-d9e4-4afc-b97f-cc8638d81d4c.png">

**enter.txt**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/201318407-1a2ff939-fee8-4f05-a3fa-d0e8ff86e105.png">


## Fase 2: Getting Access

  
## Fase 3: Intern Enumeration

  
## Fase 4: PrivEsc
  
## TryHackMe Questions
