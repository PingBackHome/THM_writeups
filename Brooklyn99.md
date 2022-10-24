# TryHackMe | {name}

+++++++++++++++++++++++++++++++++++\
IP: 10.10.96.181\
Date: 24-10-2022\
+++++++++++++++++++++++++++++++++++

##  Fase 1: Recon

### Nmap scan

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197545238-e3c950a7-17d5-4b99-a5de-87578d10890b.png">
  
**Open Ports**

21 - FTP -Vsftpd 3.0.3\
22 - SSH -OpenSSH 7.6p1\
80 - Webserver - Apache 2.4.29

### Webserver Enumeration

**Homepage**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197545966-4266c709-0e11-45fc-a392-6f65849aee81.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197546054-e43daa0d-c963-4f92-a9bb-f63b78c3f6f3.png">

**Nikto results**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197548684-7f5542b2-a636-4d6d-83db-a634f79d02fb.png">

**Dirbuster results**



**Steganography**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197547241-c2f4107f-8b60-4acd-9478-25142c25119f.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197547307-5c9d5904-7022-4c8f-a782-64926e3a050e.png">

### FTP Enumeration

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197547979-62cf6f20-5a9b-4474-a0c0-69efc1a9db06.png">

**Note to Jake**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197548334-9873ce64-f7fd-441f-aaae-c35746ad0434.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197548437-c60e84d1-724e-48e9-b0b2-168a32ddedb0.png">



## Fase 2: Getting Access

**Cracking Jake's SSH password w/ Hydra**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/197549569-8c11c445-c3da-4c50-871e-c6577bfc51aa.png">

Credentials
> jake::987654321

**Cracking Amy's SSH password w/ Hydra**


  
## Fase 3: Intern Enumeration

  
## Fase 4: PrivEsc
  
## TryHackMe Questions
