# Machine - Crocodile
![1](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/4de3b2c3-99c9-458c-9a27-7c881e20e42c)
хамгийн түрүүнд nmap ашиглан 21, 80р портууд асаалттай байгааг харсан бөгөөд ихэнхи серверүүд FTP ээ hiden байдалтай байлгадаг бөгөөд энэ машин FTP тэй ямар нэгэн холбоотой байж болзошгүй гэж үзсэн.

![Screenshot (16)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f304cd95-9043-41b4-a5e1-c3009b5378da)
* дараагаар gobuster dir -u 10.129.247.38 -w /usr/share/wordlists/dirb/common.txt

* ![Screenshot (18)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2dcb3d59-8267-48c2-9f01-95a47120d514)
* ftp 10.129.247.38 
#Anonymous оор нэвтэрхэд шууд орсон бөгөөд 
ls command аар ямар лист байгааг шалгатал
 -rw-r--r-- allowed.userlist
            allowed.userlist.passwd
олж харсан.
![Screenshot (22)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/94273a55-2c83-48cd-b908-220c73051fce)
* ftp ээр get параметр ашиглан файлыг local дээрээ татаж аваад задалж үзтэл
* ![Screenshot (23)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/7dbf65e9-275f-4860-89cd-3e5d6f41afb4)
#### хэрэглэгчийн username password хадгалсан байсан 

дараагаар 
![Screenshot (21)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/adb8cfa5-ca34-494b-8cd7-4c45af089a1e)
* анх 80р порт байсан учраас веб сервер ажиллаж байсан /login.php/ ээр хандаж авсан name password ууд аль алинтайн тулгаж үзтэл хэрэглэгчийн эрхээр нэвтэрч орж чадан
* ![Screenshot (24)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/b7096e97-d9a4-4440-a08a-e0ca985b04d4)
* admin эрхээр нэвтрэн server manager dashboard хандаж орж болж байсан.


*  




