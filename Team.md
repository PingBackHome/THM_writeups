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

Creds for FTP:
> ftpuser::T3@m$h@r3

**FTP login**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200311912-470de99d-d4ce-4cf8-8550-75ddff8eeef0.png">

***FTP: workshare/New_site.txt***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200312109-15a20898-83c0-4e04-8732-73ea3fc13725.png">

Possible usernames:
> gyles::??
> dale::??

**Adding .dev to host**

<img width="250" alt="image" src="https://user-images.githubusercontent.com/115549820/200313031-4210a9d9-3a60-4fa2-b6e2-9f5add3767d5.png">

**dev.team.thm**

<img width="350" alt="image" src="https://user-images.githubusercontent.com/115549820/200313199-98454362-2de5-4d15-accb-654f99bb66c5.png">

***/../../../etc/passwd***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200313792-72a8bc7a-4b9e-44db-b3cd-c72a88429234.png">

***/../../../home/dale/user.txt***

<img width="833" alt="image" src="https://user-images.githubusercontent.com/115549820/200314417-cb9f9141-82ee-4e7b-8b8d-bf42782432b3.png">

**Searching for interesting LF-locations w/ Burpsuite**

<img width="750" alt="image" src="https://user-images.githubusercontent.com/115549820/200319621-1bc6e0b0-831f-4957-9875-98b7d3c6a726.png">

***../etc/ssh/sshd_config***

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200319940-155715f5-4665-400b-87e7-b229f14addce.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200319996-a957b3fb-bd51-4020-8454-0237ef135e7a.png">

**Copy id_rsa privkey**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200320402-c20501d7-e33b-478c-b221-e2366c547caf.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200320458-75483b04-1d73-4859-baac-335abeb1d485.png">

<img width="200" alt="image" src="https://user-images.githubusercontent.com/115549820/200320577-1b409729-6e15-480b-81a5-5a63bc76ee0e.png">

## Fase 2: Getting Access

<img width="300" alt="image" src="https://user-images.githubusercontent.com/115549820/200324660-c7e072d8-408d-42ff-b3c1-c56bf834ff1a.png">
  
## Fase 3: Intern Enumeration

<img width="478" alt="image" src="https://user-images.githubusercontent.com/115549820/200325459-3af30c7f-0ec9-4af2-a2d0-ef90d6a6023e.png">

**Uploading linpeas.sh**

<img width="478" alt="image" src="https://user-images.githubusercontent.com/115549820/200325657-83670b61-87cb-4b7c-88a0-10562d50689c.png">

<img width="992" alt="image" src="https://user-images.githubusercontent.com/115549820/200325840-0934a17e-c678-4ef9-bc2a-4356f8c9d949.png">

***Output linpeas.sh***

<img width="231" alt="image" src="https://user-images.githubusercontent.com/115549820/200327613-21ca7ffc-fa3c-4d52-8686-3ca8b3e54bce.png">

<img width="735" alt="image" src="https://user-images.githubusercontent.com/115549820/200327887-cfbb4feb-54b9-4796-bf1e-090625f0e3b6.png">

  
## Fase 4: PrivEsc

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200329397-04694bbc-848f-4833-9243-f08f674144b3.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200330694-9857ca58-0c9b-4fb8-8dcf-ccac0ae6ba34.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/200330755-7880127b-a94d-4aa8-a5d6-1af9a9728e27.png">

<img width="450" alt="image" src="https://user-images.githubusercontent.com/115549820/200332697-aded4394-2068-41eb-8f8e-3b44d8d785de.png">

<img width="465" alt="image" src="https://user-images.githubusercontent.com/115549820/200332840-9eaea07d-26c3-44cc-a8f6-137409791a9e.png">

<img width="465" alt="image" src="https://user-images.githubusercontent.com/115549820/200332944-8e2594d3-883b-4694-a137-a5f45a19af88.png">

<img width="526" alt="image" src="https://user-images.githubusercontent.com/115549820/200333066-276b131f-0de0-46b7-a48e-98a061b3509c.png">

<img width="526" alt="image" src="https://user-images.githubusercontent.com/115549820/200333216-220643fd-f6ae-45f8-9ab5-39c5bb7ca903.png">


## TryHackMe Questions

user.txt
> THM{6Y0TXHz7c2d}

root.txt
> THM{fhqbznavfonq}
