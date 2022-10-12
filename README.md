# TryHackMe | Basic Pentesting
IP: 10.10.62.222\
Date: 11-10-2022

##  Fase 1: Recon

### Nmap scanning

<img width="797" alt="image" src="https://user-images.githubusercontent.com/115549820/195089832-0544726d-91cd-4c09-8301-2b024b6cf2f2.png">

**Open ports:**\
22    SSH         - OpenSSH 7.2p2\
80    Webserver   - Apache httpd 2.4.18\
139   Samba       - smbd 3.x\
445   Samba       - smbd 4.3.11\
8009  Ajp13       - Apache Jserv (protocol v1.3)\
8080  Webserver   - Apache Tomcat 9.0.7

### SMB enumeration

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195094435-14bd0691-f9db-426b-a965-8f2e70dd1b0a.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195094589-73aff069-e8ef-4c9e-ba6d-5030db2614fb.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195094768-b3725819-a2dd-4ad9-b494-f7c461f7d3c7.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195095120-70cab2ab-2d28-4596-b8dd-217b4ec610b5.png">


### Webserver Enumeration

**home pages**

http://10.10.62.222

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195098657-d63aca5a-597f-465f-9bab-cb859329eef5.png">

http://10.10.62.222:8080

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195099003-b031ea43-4c35-434c-8326-361b9abfa4d6.png">

**Nikto scans**

Port: 80

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195101238-eb573760-9dee-4ee8-85a3-e26f3a52a414.png">

Port: 8080

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195105317-30dd7c74-bfcd-4b18-adda-7f3e17c9d18e.png">

**Dirbuster scan**

Port: 80

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195107281-7440c524-a89a-45cf-b2a9-16777d8eae21.png">

Port: 8080

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195108626-1f1955f2-59b5-4406-b8ed-227a41f9f04a.png">

**Results web scan**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195110200-7ae1fbba-ddf1-476f-b9cb-bf4698b267a6.png">
<img width="450" alt="image" src="https://user-images.githubusercontent.com/115549820/195110314-74508b95-8f7b-4059-a2c0-e1eda20064ae.png">
<img width="450" alt="image" src="https://user-images.githubusercontent.com/115549820/195110440-a2415fa3-a9c6-4f1d-b14f-cacf0ae5356b.png">



## Fase 2: Getting Access

**Hydra ssh cracking**

<img width="450" alt="image" src="https://user-images.githubusercontent.com/115549820/195118742-5e190fe0-1da4-4d7e-a72b-eab9855d9b52.png">


## Fase 3: Intern Enumeration


**Uploading LinPeas.sh**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195304662-faa3b39d-b503-4a98-a9ea-72cd458ddb9a.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195304589-1e0c9e99-ebd1-487f-be81-defb5717ddd8.png">

<img width="311" alt="image" src="https://user-images.githubusercontent.com/115549820/195305477-004e9e17-6e41-4353-b574-b4bd38f74c0c.png">

**Scanning Intern Results**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/115549820/195321109-105d1d91-b7aa-491b-99fb-c672b2c54bdd.png">

<img width="300" alt="image" src="https://user-images.githubusercontent.com/115549820/195321833-7f57b127-b762-4e45-a4ab-770d9cdce0a5.png">

<img width="300" alt="image" src="https://user-images.githubusercontent.com/115549820/195322156-f6951bec-4964-4c01-a711-41414465bcb0.png">

<img width="466" alt="image" src="https://user-images.githubusercontent.com/115549820/195322614-c5d4cd99-1c07-4830-849d-802461d889df.png">

## Fase 4: PrivEsc

**SSH-key**


