# TryHackMe | Mustacchio

+++++++++++++++++++++++++++++++++++\
IP: 10.10.42.99\
Date: 07-11-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scan

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200340040-806100f0-6210-498d-8347-a7fa7eefa517.png">

**Open Ports**

22 - SSH - OpenSSH 7.2p2\
80 - Webserever - Apache 2.4.18

### Webserver Enumeration

**Dirbuster Output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200342368-9cc68390-2205-431f-8c74-0adfac23ceb9.png">

***Homepage***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200342516-352272ab-55c5-4d61-b8bb-d411d0796213.png">

***/custom/js/users.bak**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200343128-30834348-da36-45e2-845a-1aa12bad9f8a.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200343515-e80d084c-b2da-4e90-a808-fae17aad5514.png">

<img width="45005" alt="image" src="https://user-images.githubusercontent.com/115549820/200343857-fa496484-0e0f-4f6c-8c85-fbb0bc8a0823.png">

Possible cred:
> admin::bulldog19

**Nikto Output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200342329-02cda31b-386f-48e2-9c68-99a945772c34.png">


## Fase 2: Getting Access

  
## Fase 3: Intern Enumeration

  
## Fase 4: PrivEsc
  
## TryHackMe Questions
