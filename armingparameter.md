ARMING_SKIPCHK, ArduPilot’un kalkış öncesi yaptığı güvenlik kontrollerini (Pre-Arm Checks) baypas etmenizi sağlayan bir parametredir.
Normal şartlarda ArduPilot; GPS kilidi, pusula kalibrasyonu, pil seviyesi ve sensör sağlığı gibi onlarca veriyi kontrol eder.
Eğer bunlardan biri hatalıysa "Pre-Arm: [Hata Mesajı]" uyarısı verir ve motorların çalışmasına (Arm olmasına) izin vermez.
ARMING_SKIPCHK ise bu engelleri aşmak için kullanılır.

0 (Varsayılan): Hiçbir kontrolü atlama.
1: Tüm kontrolleri atla.


ARMING_RUDDER, aracın motorlarını (Arm/Disarm) kumanda üzerindeki Rudder (Yaw/Yön) çubuğunu kullanarak aktif edip edemeyeceğinizi belirleyen parametredir.
0 (Disabled): Çubukla Arm/Disarm yapma özelliği tamamen kapalıdır. Motorları sadece Mission Planner veya bir GCS (Yer Kontrol İstasyonu) üzerinden "Arm" yapabilirsiniz.
1 (Arming Only): Çubukla sadece motorları çalıştırabilirsiniz (genellikle Rudder sağa tam yaslıyken). Ancak çubukla motorları durduramazsınız (Disarm yapamazsınız).
2 (Arm or Disarm): Hem çalıştırma (Arm) hem de durdurma (Disarm) çubuk hareketiyle yapılabilir. (En yaygın kullanılan ayar budur).

Arm (Çalıştırma): Sol çubuğu (Gaz ve Yaw) en alta ve en sağa çekip birkaç saniye beklersiniz.

Disarm (Durdurma): Sol çubuğu en alta ve en sola çekip birkaç saniye beklersiniz.


ARMING_REQUIRE, ArduPilot sisteminde motorların çalışmaya başlamadan önce bir "Arm" (kurulma/hazır hale gelme) sürecinden geçip geçmeyeceğini belirleyen temel güvenlik parametresidir.
Bu parametre, sistemin bir "Arming" (Kurulma) moduna sahip olup olmayacağını belirler.
Pili taktığında motorların doğrudan çalışmaya hazır olup olmadığını seçer.
Ayar 1 (Normal): "Kapı kilitli." Motorların dönmesi için önce senin kumandadan "Arm" (aç) komutu vermen şarttır.
Ayar 0 (Tehlikeli): "Kapı yok." Pili taktığın an gaz kolunu kaldırırsan pervaneler döner.
Amacı: Yanlışlıkla gaza dokunup kendine zarar vermeni önlemek ve kalkış anında "Home" noktasını kaydetmektir.

ARMING_OPTIONS, motorların kurulması (Arm) ve durdurulması (Disarm) süreçlerindeki özel davranışları belirleyen bir "özellikler listesi" parametresidir.
1 (Bit 0)	Permit Arming in Mission	Araç bir "Mission" (Otonom Görev) modundayken Arm olmasına izin verir. Normalde sadece manuel modlarda Arm yapılması önerilir.
2 (Bit 1)	Disarm on Landing	Araç yere indiğini algıladığında motorları otomatik olarak durdurur. (En popüler seçeneklerden biridir).
4 (Bit 2)	Arm/Disarm via Transmitter Switch	Bir kumanda anahtarı (Switch) kullanarak Arm/Disarm yapmanızı sağlar. Çubukla (Stick) Arm yapmaktan çok daha hızlı ve güvenlidir.
8 (Bit 3)	Don't Mission Reset	Arm yapıldığında mevcut görevi (mission) sıfırlamaz, kaldığı yerden devam eder.

ARMING_MIS_ITEMS, otopilotun motorları kurmadan (Arm etmeden) önce yüklenen görev listesinde (Waypoint listesinde) herhangi bir hata veya eksiklik olup olmadığını kontrol etmesini sağlar.
Eğer görev listesinde bir mantık hatası varsa, sistem "Pre-Arm: Mission Error" uyarısı verir ve kalkışa izin vermez.
0 (Disabled): Görev listesi kontrol edilmez.
1 (Enabled): Görev listesi sıkı bir denetimden geçer. Hata varsa motorlar asla çalışmaz.
Özellikle büyük ve pahalı araçlarda, otonom bir uçuşun ortasında yazılımın kilitlenmesini veya aracın saçma bir yöne gitmesini engeller.
Hatalı bir görevi havada fark etmek yerine, yerdeyken fark edip düzeltmenizi sağlar.

ARMING_MAGTHRESH, ArduPilot'un kalkıştan hemen önce pusula (manyetometre) verilerinin ne kadar "gürültülü" veya değişken olduğunu kontrol ettiği bir güvenlik eşiğidir.
Pusuladan gelen ham verideki dalgalanmanın (gürültünün) kabul edilebilir sınırını belirler.

ARMING_ACCTHRESH, ArduPilot’un kalkış öncesinde ivmeölçer (accelerometer) verilerinin ne kadar stabil olduğunu kontrol ettiği bir güvenlik eşiğidir.
Bir "hareketsizlik kontrolü"dür.

