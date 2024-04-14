on Hackthebox Appointment Machine

![Screenshot (2)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/572a44d0-6d93-4333-91be-9fe7c7ca9461)
Hackthebox Appointment machine ийг туршиж үзсэн нь
-
![Screenshot (6)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/a90e3442-e04e-45c9-be7e-3d22315ea485)
`Nmap хайлтаас харахад бид порт 80 нээлттэй бөгөөд 2.4.38 хувилбартай Apache httpd сервер ажиллаж байгаа`

![Screenshot (4)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/9378d6bc-9a10-4c90-9056-7bf54dcf42c4)

`Login user interface байсан учир эхлээд brute force хийж үзсэнч хамгийн оновчтой арга нь датабэйс рүү SQL injection халдлага хийх юм`

![Screenshot (7)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/0873af22-492e-4248-a4ff-9dc2318fce55)

``` tool ашиглан ямар хандалтууд байгааг олж харах```

![Screenshot (9)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/f663b8e6-0ef9-4d9a-92e2-abd1e4ba3caa)

`Login байсан учир энгийн SQL inject хийх гэж үзсэн ч бүтэлгүйтсэн`

![Screenshot (8)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/6a89efa3-58cf-4388-bda2-58c6e0b02b8d)


`default username: admin password:password гэх зэрэг brute force хийж үзсэн`
![Screenshot (12)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/ff5c4e69-5796-4578-8052-206d2db81699)


`HTB start point toi machine хийсэн учир A03:2021 SQL injection
юу хийдэг талаар асуухад гүүглдэж үзэн username дээр  admin’#  гэж ажиллахад database дээр username password 2 ийг зэрэг шалгахгүйгээр эхний username dabataase дээр зөв ажиллахад шууд тэр нэртэй хэрэглэгчээр хандалт хийж орох юм`


![Screenshot (11)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/bfb4efd7-68f2-48cd-bcf0-41aff7edc127)
`username: admin’# гэх sql injection энэ веб сайтад байсан учир эцэс сүүлд нь root flag олж авав`



![Screenshot (13)](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/7ee8dadf-b86b-43f8-9ce4-8d489fcf97d7)






