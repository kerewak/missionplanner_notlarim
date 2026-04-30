RTL_ALTITUDE, "Return To Launch" (Başlangıç Noktasına Dönüş) modundayken aracın hangi yükseklikte seyredeceğini belirleyen kritik bir parametredir.


RTL_AUTOLAND parametresi, bir hava aracının "Eve Dönüş" (RTL) manevrasını tamamladıktan sonra otomatik olarak iniş yapıp yapmayacağını belirleyen bir kontrol mekanizmasıdır.


RTL_CLIMB_MIN, ArduPilot ve benzeri uçuş kontrol yazılımlarında "Eve Dönüş" (RTL) manevrasının başlangıcında yapılan minimum tırmanma miktarını belirleyen bir güvenlik parametresidir.
Bu parametre, aracın eve dönüş yoluna geçmeden önce mevcut irtifasından ne kadar daha yukarı çıkması gerektiğini kontrol eder.


RTL_RADIUS, genellikle ArduPilot (özellikle ArduPlane) sistemlerinde kullanılan, aracın "Eve Dönüş" (RTL) manevrası sırasında ana nokta (Home) üzerinde hangi genişlikte bir daire çizeceğini belirleyen parametredir.
Sabit kanatlı bir uçak, döner kanatlı bir drone gibi olduğu yerde asılı kalamaz. Bu nedenle eve ulaştığında, havada güvenli bir şekilde kalabilmek için belirli bir yarıçapta dönmeye başlar.
