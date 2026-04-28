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
