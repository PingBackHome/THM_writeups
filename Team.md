# TryHackMe | Team

+++++++++++++++++++++++++++++++++++\
IP: 10.10.168.239\
Date: 07-11-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scan

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200295150-b1d3da41-166f-4c6d-b20b-caf965492076.png">

**Open Ports**

21 - FTP - vsftpd 3.0.3\
22 - SSH - OpenSSH 7.6p1\
80 - Webserver - Apache 2.4.29

### FTP Enumeration

<img width="450" alt="image" src="https://user-images.githubusercontent.com/115549820/200295867-632d7502-6baf-40d1-b1a7-159d1b74b1de.png">

### Webserver Enumeration

**Nikto Output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200297223-cc85ec44-fd0f-475e-bb9c-5d8726192b78.png">


**Dirbuster Output**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200297555-3557adf2-a714-4e96-98b5-d1500c430e95.png">

**Add to host file**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200299255-cad28f1d-9ebf-4e36-86ae-918c23a78d0e.png">


**New try Dirbuster**

<img width="756" alt="image" src="https://user-images.githubusercontent.com/115549820/200301377-7459a183-23c1-4465-beda-0f27ee68e289.png">

***Homepage***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200299472-993a43fe-039d-401b-af74-4a8b7d13cf56.png">

***/robots.txt***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200301725-498ae50a-f0bc-4c1c-9064-08e212bb81e7.png">

***/scripts/scripts.txt***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200302223-759be9a9-f674-4705-99f7-cd421ae7d0c5.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200303373-fed7a0c4-f6b0-4d0b-b4d1-9889a97376c5.png">

***/scripts/script.old***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200303527-c253e9ef-97a0-4f26-84b4-5e577c721f36.png">



## Fase 2: Getting Access

  
## Fase 3: Intern Enumeration

  
## Fase 4: PrivEsc
  
## TryHackMe Questions
