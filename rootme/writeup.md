#R00tme thm Machine 
____________________
![Screenshot (51)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/3e224239-03e1-4c76-aced-b3e73ecafcfa)
*R00tme thm Machine 

![Screenshot (52)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/a1d8597e-133e-4260-989f-63a4ee7fd116) 
##### хаяг дээр 22 болон 80р портууд асаалттай байсан
*$sudo nmap -sC -sV -Pn 10.10.246.111

![Screenshot (53)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/fa49db43-3010-4aec-87e7-2ff44e3f0908)
Дээрх үр дүнгээс харахад сонирхолтой зүйл байхгүй байсан тул веб буюу 80 порт рүү хандалт хийн ухсан ч сэжиг бүхий зүйлүүд байхгүй байсан. Тиймээс вебийн нөөцрүү хандалт хийхийн тулд directory enumeration хийсэн ба panel болон uploads гэх нэртэй зам олсон

дараа нь ямар нэгэн файл inpput хийх гэж оролдтол болохгүй байсан ба судалгаа хийсний дараагаар php reverse shell хийж болохыг олж мэдэн ямар ч хамаагүй php file upload хийтэл denied хийгээд байсан учир дахин судалж php4 php5 буюу extension ийг өөрчлөн upload хийж үзтэл амжиллттай болсон

![Screenshot (55)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f01c37df-b876-413e-901f-92768444f0d9)
php reverse shell бэлэн source code татаж аван өөрийн tun0 үүсгэсэн local ip хаяг болон порт ийн дугаарыг оруулж өгснөөр амжиллтай reverse shell авах юм 
 



![Screenshot (56)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f5dec809-57da-406c-a6e7-caa89b9e53cd)
*
![Screenshot (58)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/321493f6-e23d-4931-ada1-c6fc2c92cd9d)
#### nc -lvnp 1234 --> netcat ашиглан user ээр нэвтэрч чадав


![Screenshot (59)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/252a2042-254d-4f91-8609-5b00b9550754)

![Screenshot (61)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/b119c093-07ba-463d-92f5-fc64fe9af849)
$find / -user root -perm / 4000 командаар шалгатал root рүү permission denied зааж байсан тул 


![Screenshot (63)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/d6e7df8f-fb87-45b5-88db-bcbb35c36b42)
SUID privileges хийх арга олсон

![Screenshot (65)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/d517dedf-b8cc-480a-8541-23f65a1f3434)
##### /usr/bin/./python -c 'import os; os.execl("/bin/sh", "sh", "-p")
```#whoami```
root 
cd /root
ls
root.txt
cat root.txt
THM{pr1v1l3g3_3sc4l4t10n}
