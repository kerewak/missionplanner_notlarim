Simulation sekmesinde hangi araç üzerine simülasyon yapmak istiyorsak onu seçiyoruz.
Plan sekmesinde waypointlerin grad seviyelerini minimumda tutmaya çalışmalıyız. Dik inişler istemeyiz.
Plan sekmesinde Distance pil bitinceye kadar ne kadar uzağa uçabileceğini gösterir.
Uçak seçtiysek uçağı nasıl hareket ettiririz
Simulation sekmesinde Sim Speed kısmından uçağın hızıyla oynayabiliriz (Uçağın gerçek hızını değil simülasyonun hızını etkiler).
sağ tıka bastığımızda çeşitli komutlar görürüz.
Fly To Here dediğimizde bize alt(irtifa) sorar.
Bunu yaptığımızda uçak gitmez çünkü uçağımız DISARMED modda yani
herhangi bir komuta hazır değil. Uçağı ARMED moda geçirirsek uçak hazır olacaktır.
Data sekmesinde Acions kısmında Arm/Disarm butonu var ona bir kere basarsak uçağımız ARMED hale gelecektir.
Bu haldeyken Fly To Here dediğimizde bizim komudumuzu yine dinlemeyecektir. Uçak çünkü Manual moddadır.
Bizden emir alacak moda getirmek için Actions kısmında modunu değiştireceğiz. Guided moda alalım. Sonra yanındaki
Set Mode butonuna basalım. Şimdi Fly To Here dersek yine gitmez çünkü uçağımız yerde.
Uçağı kaldırmak için uçağı TAKEOFF moda alırız. Uçak kalkışa başladı ve kendi kendine daire çizecektir. Uçağı emrimizi dinlemesi 
için Guided moda alalım. Uçuş planı sekmesi yazılım olmayan bir otomasyondur, program üzerinden uçağa belirli rotalar tanımlayabiliyoruz.
Sol tık yaparak hedef belirliyoruz. Daha sonra bu rotayı kaydetmemiz lazım, Write butonuna basalım. Uçak Guided modda olduğu için
çizdiğimiz rotayı takip etmiyor. Takip etmesini istiyorsak uçağı Actions kısmından uçağı Auto moduna alacağız. Uçak son hedefe vardığında RTL moduna
geçer ve H noktasına döner ve o noktada dönüş yapmaya başlar.

Config sekmesinde Full Parameter List kısmında parametrelerle oynayabiliriz ancak çok dikkatli olmamız gerekir.
Plan sekmesinde biz rota çizimiyle Mission kısmına baktık. Fence seçeneğinde ise bir alan seçiyoruz ve uçak programdan aldığı
otomasyonlar sayesinde istediğimiz şeyi yapabiliyor. FENCE_CIRCLE_EXCLUSION seçeneğiyle sol tıkladığımızda kırmızı bir alan yaratırız.
Bu alan yasaklı bölge olarak geçer. Full Parameter List kısmında uçağın Fence durumunda uçağın nasıl bir tepki vereceğini kontrol edebiiriz.

Plan sekmesinde Polygon butonuna basalım Draw a Polygon seçeneğiyle istediğimizi çizebiliriz. 
Fence Inclusion ve Fence Exclusion seçenekleri:
Fence Inclusion çizdiğimiz alanın dışına çıkmaz, Fence Exclusion ise bu alanın içine girme demektir.
Fence Inclusion'u seçersek ve uçak bu alanın dışına çıkarsa benim parametre ayarlardından aksiyonu RTL seçmem gibi, uçak
Fence etkisinde RTL moduna girecek ve H noktasına dönecektir.

Yarışma alanındaki diğer İHA'ların da ekranda temsili olarak bulunmasını isteyebiliriz.
Simulation sekmesinde  Plane Swarm - Multilink butonu var ona bastığımızda kaç tane uçak uçurmak istediğimizi sorar ve girdiye göre
o kadar pencere açar.

Yazılımımızı uçağa bağlanarak çalıştırabiliriz.
