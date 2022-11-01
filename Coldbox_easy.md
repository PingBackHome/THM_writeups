# TryHackMe | Coldbox: Easy

+++++++++++++++++++++++++++++++++++\
IP: 10.10.238.160\
Date: 01-11-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scan

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199202072-fbc0866b-640e-44b1-ad89-365770e7434b.png">

**Open Ports**

80 - webserver - Apache 2.4.18\
4512 - SSH - OpenSSH 7.2p2


### Webserver Enumeration

**Nikto Output**

<img width="750" alt="image" src="https://user-images.githubusercontent.com/115549820/199203651-a8c455d8-9e99-45f1-b55e-5f3475622ec3.png">

**Dirbuster Output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199202990-c737e025-a651-4ecb-b2de-eb65f7a6aeda.png">

***Homepage***

<img width="750" alt="image" src="https://user-images.githubusercontent.com/115549820/199203119-1f6e710b-7938-4048-aa4c-9a6043448e70.png">

***/hidden***

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/115549820/199203218-38415adf-8d65-4ceb-be23-035e67079af7.png">

***/xmlrpc.php***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199203472-d00ac009-8ac7-4f4a-b561-afdd7c89a648.png">

***/wp-login.php***

<img width="250" alt="image" src="https://user-images.githubusercontent.com/115549820/199203847-eec8494d-ac9f-45b3-9a58-2e098207b0fe.png">

**WPscan Output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/199204768-727f4e55-6f00-497c-a97e-58a3b18404d2.png">



## Fase 2: Getting Access

  
## Fase 3: Intern Enumeration

  
## Fase 4: PrivEsc
  
## TryHackMe Questions

'user.txt'
> 

'root.txt'
> 
