# Dolphin Schaduler kullanımı.

- *cmd ekranına ** docker run --name dolphinscheduler-standalone-server -p 12345:12345 -p 25333:25333 -d apache/dolphinscheduler-standalone-server:3.0.0 ** yazıyoruz

- http://localhost:12345/dolphinscheduler adresine gidiyoruz 

- Username and password: admin/dolphinscheduler123

- Security kısmından gerekli işlemleri yapacağız![image](https://user-images.githubusercontent.com/110333072/183598567-9f8be81f-ccd0-43e4-a24e-ea61255b2d29.png)

- Create Queue 

![image](https://user-images.githubusercontent.com/110333072/183604454-7c186fe9-cb20-4285-b9a4-77138eb95670.png)

- Tenant Manage (iş oluşturma)

![image](https://user-images.githubusercontent.com/110333072/183604800-52768afe-f5c6-4c66-9103-af216d949c97.png)

ilk olarak isim veriyoruz ardından oluşturduğumuz Queue yi seçiyoruz ardından ayrıntıları giriyoruz

- Users Manage (Kulanıcı oluştur - Düzenle)

![image](https://user-images.githubusercontent.com/110333072/183605270-4e5bb9ab-a402-40e1-aee6-6103f81a1020.png)

Burada kullanıcı oluşturuyoruz önceden oluşturduğumuz tenant ve queue yi seçiyoruz.

- Alarm İnstanca Manage

![image](https://user-images.githubusercontent.com/110333072/183606759-7a765ec7-3ce1-4842-8ddf-1e596c966fdd.png)

İsim gir - türü seç ve gerekli kısımları ekle


- Alarm Group Manage 

![image](https://user-images.githubusercontent.com/110333072/183609212-5298eea4-f8a8-4b97-895c-1d770d3e3446.png)

İsim giriyoruz ardından oluşturduğumuz Alarm İnstance yi seçiyoruz en sonunda ayrıntıları giriyoruz

                                                                                                                                              
