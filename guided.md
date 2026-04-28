GUIDED_TIMEOUT, ArduPilot’un Guided (Rehberli) modundayken yer istasyonundan (Mission Planner, QGroundControl vb.)
veya bir yardımcı bilgisayardan (Companion Computer) yeni bir komut gelmediği sürece ne kadar bekleyeceğini belirleyen güvenlik parametresidir.

GUIDED_SMAX, ArduPilot'un Guided (Rehberli) modunda hareket ederken ulaşabileceği maksimum yatay hızı sınırlayan parametredir.

GUIDED_PDMX, ArduPilot'un Guided (Rehberli) modunda bir yere giderken araç ile hedef noktası arasındaki maksimum kabul edilebilir mesafeyi (Position Displacement Maximum) belirleyen parametredir.

GUIDED_P, ArduPilot'un Guided (Rehberli) modunda konum kontrolünü sağlayan P (Proportional - Oransal) kazanç değeridir.

GUIDED_NTF (Guided Notifier), ArduPilot'un Guided (Rehberli) modundayken dışarıdan gelen komutların ulaşıp ulaşmadığını
veya kabul edilip edilmediğini kullanıcıya bildirmek için kullanılan bir parametredir.

GUIDED_NEF (Guided NAV Error Filtering), ArduPilot'un Guided (Rehberli) modunda dışarıdan gelen konum komutlarındaki
"gürültüyü" veya ani sıçramaları temizlemek (filtrelemek) için kullanılan bir parametredir.

GUIDED_IMAX, ArduPilot'un Guided (Rehberli) modundaki konum kontrol döngüsünde kullanılan I (Integral - Bütünleyici) kazancının maksimum sınırıdır.
arametrenin Kritik Görevi
Neden bu güce bir sınır (IMAX) koyuyoruz?
Eğer bu sınır olmasaydı ve dron rüzgara karşı çok fazla güç biriktirseydi, rüzgar aniden kesildiğinde dron o biriken devasa güçle hedefini fersah fersah geçerdi.
Bu duruma "Integral Wind-up" denir. GUIDED_IMAX bu patlamayı önleyen emniyet vanasıdır.

GUIDED_I, ArduPilot'un Guided (Rehberli) modundaki konum kontrol döngüsünün I (Integral - Bütünleyici) kazanç değeridir.
GUIDED_IMAX bu gücün sınırıyken, GUIDED_I bu gücün kendisini ifade eder.

GUIDED_FLTT (Guided Target Filter), ArduPilot'un Guided (Rehberli) modunda dışarıdan gelen konum/hedef verilerini işlerken kullandığı alçak geçiren filtre (Low Pass Filter) frekans değeridir.
Filtrenin kesim frekansıdır (Hz). ArduPilot'un veriyi hangi hızda süzgeçten geçireceğini söyler.

GUIDED_FLTE (Guided Velocity Error Filter), ArduPilot'un Guided (Rehberli) modunda dronun hız (velocity) hedeflerini takip ederken kullandığı alçak geçiren filtre (Low Pass Filter) değeridir.

GUIDED_FLTD (Guided Velocity Derivative Filter), ArduPilot'un Guided (Rehberli) modundaki hız kontrol döngüsünde kullanılan D (Derivative - Türevsel) kazancını süzgeçten geçiren alçak geçiren filtre değeridir.

GUIDED_FF (Guided FeedForward), ArduPilot'un Guided (Rehberli) modundaki hız kontrol döngüsünde kullanılan İleri Besleme (FeedForward) kazancıdır.
Bu parametre, otopilotun "bekle-gör" mantığıyla çalışan PID sistemini bir kenara bırakıp, verilen komutu anında ve doğrudan eyleme dökmesini sağlar.

GUIDED_D_FF (Guided Derivative FeedForward), ArduPilot'un Guided (Rehberli) modunda hız kontrolü yaparken, hedef hızdaki değişim oranına (ivmelenmeye) göre önceden tepki verilmesini sağlayan bir kazançtır.
GUIDED_FF hızın kendisiyle ilgilenirken, GUIDED_D_FF hızın ne kadar hızlı değiştiğiyle ilgilenir.

GUIDED_D, ArduPilot'un Guided (Rehberli) modundaki konum kontrol döngüsünün D (Derivative - Türevsel) kazanç değeridir.
Eğer GUIDED_P dronu hedefe çeken bir lastik bant ise, GUIDED_D bu hareketin hızını kontrol eden bir amortisördür.
