# Dolphin Schaduler kullanımı.

- Docker ' i açıyoruz.

- *cmd ekranına ** docker run --name dolphinscheduler-standalone-server -p 12345:12345 -p 25333:25333 -d apache/dolphinscheduler-standalone-server ** yazıyoruz

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

- Worker Group Manage 

![image](https://user-images.githubusercontent.com/110333072/183610472-0fd92a95-9231-421d-9211-3b2a030cc22b.png)

isim giriyoruz, Worker Adress giriyoruz.

- Environment Manage 

![image](https://user-images.githubusercontent.com/110333072/183612137-eda57009-66df-4f70-bfc8-7d12f941c69e.png)

isim gir , çevre elemanları gir , detayları yaz  , worker group seç.

- Token Manage 

![image](https://user-images.githubusercontent.com/110333072/183613914-f5a60e38-342a-4bbf-8911-461d55f36b25.png)

Kullanıcıya oluşturduğumuz token in son kullanım tarihini giriyoruz hangi kullanıcı olduğunu seçiyoruz 

- Kendi Oluşturduğumuz Kullanıcıya girmek için admin hesaptan çıkış yapıyoruz

![image](https://user-images.githubusercontent.com/110333072/183627206-9f24b23b-ca8a-42a1-a7e5-90701b312717.png)

- Kendi oluşturduğumuz kullanıcı adı ve şifresini giriyoruz


- Ardından üst kısımdan project i seçiyoruz

![image](https://user-images.githubusercontent.com/110333072/183626547-b02e3c97-f57e-4273-a783-f7cf0f8577c4.png)

- Create Project e tıklayıp proje oluşturuyoruz hangi kullanıcının sahip olacağı orada yazıyor. 

![image](https://user-images.githubusercontent.com/110333072/183629480-c02704b9-98f9-44ba-811b-d231521a8dfb.png)
 
 - Proje isminin üstüne tıklıyoruz

- Workflow Defination a giriyoruz sonra Crate Workflow Definition a basıyoruz

![image](https://user-images.githubusercontent.com/110333072/183630210-870fc81d-28f5-41a8-b566-927f24d55c35.png)

- Proje için Workflow çizebiliriz.

![image](https://user-images.githubusercontent.com/110333072/183630348-97538496-b47e-4af5-8264-d54540a807e8.png)

- Node Name 	Görevin adını ayarlayın. Bir iş akışı tanımındaki düğüm adları benzersizdir.
- Run flag	Düğümün normal şekilde programlanıp programlanamayacağını gösterir. Yürütmek gerekli değilse, yürütmeyi yasaklayan anahtarı açabilirsiniz.
- Description	Bu düğümün işlevini açıklar.
- Task priority	  Çalışan iş parçacığı sayısı yetersiz olduğunda, önceliğe göre yüksekten düşüğe doğru, öncelik aynı olduğunda ilk giren ilk çıkar ilkesine göre yürütülürler.
- Worker group	 Görev, yürütme için çalışan grubundaki makinelere atanır. Varsayılan seçilirse, yürütme için rastgele bir çalışan makine seçilir.
- Task group name	    Kaynaklar'daki grup, yapılandırılmamışsa kullanılmayacaktır.
- Environment Name	Komut dosyasının çalıştırılacağı ortamı yapılandırın.
- Number of failed retries    Başarısızlıktan sonra görevin yeniden gönderilme sayısı. Açılır ve manuel doldurmayı destekler.	
- Failure Retry Interval     Görev başarısız olursa görevi yeniden göndermek için zaman aralığı. Açılır ve manuel doldurmayı destekler.
- Timeout alarm        Zaman Aşımı Alarmını ve Zaman Aşımı Hatasını kontrol edin. Görev "zaman aşımı süresini" aştığında, bir alarm e-postası gönderilir ve görev yürütme başarısız olur.
- Script	  Kullanıcı tarafından geliştirilen bir SHELL programı.
- Resource	Komut dosyasında çağrılması gereken kaynak dosyalarının listesini ve Kaynak Merkezi - Dosya Yönetimi'nde yüklenen veya oluşturulan dosyaları ifade eder
- User-defined parameter   ${variable}Komut dosyasındaki içeriği değiştirecek olan, Shell'in kullanıcı tanımlı bir parametresidir.
- Predecessor task   	Mevcut görevin öncül görevinin seçilmesi, seçili öncül görevi mevcut görevin yukarı akışı olarak ayarlar


- Opreation bölümündeki HTTP istek göndermemizi sağlar. isimi girdikten sonra Http url kısmını dolduruyoruz.

- İşlem Bitince Saveliyoruz

- Workflow Instance den hata var mı yok mu kontrol ediyoru

- Ardından Workflowumuzun sağ tarafında yer alan operation bölümünden işlemler yapacağız.

- offline mod tam anlamıyla duraklatır edit vs yapmamızı sağlar

- Timing kısmından zaman ayarlamalarını yapabiliriz 

- Zaman ayarında değişiklik istersek cron manage ye girip edit kısmından start ve stop kısımlarından zaman ayarı yapabiliriz

- Start Başlatır.


* Timing başlatma ve durdurma zamanını ayarlar. uygulama başlatıldıktan sonra değişiklik yapmak için cron manage yi kullanın.
-Start stop time başlatma ve durdurma zamanı Timin kısmı ise zaman aralıklarını belirler 

![image](https://user-images.githubusercontent.com/110333072/184120602-b62c159f-1838-4c4e-b3c2-ce610a94966f.png)

- Dakika saat gün ay veya yıl olarak seçebiliyoruz ayrıca spesific kısmından düzenli olmayan aralıkları da ekleyebiliyoruz







                                                                                                                                              
