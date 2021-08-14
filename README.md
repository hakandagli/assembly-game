# Assembly game

## Malzemeler
- Arduino
- 2 tane "7 segment display"
- 8 tane led
- 1 tane tuş
- kablolar ve dirençler

### Oyunun Hazırlanması
Gerekli pimlere gerekli bağlantıları yaptıktan sonra, arduino'ya kodumuzu yükledikten sonra ve güç verdikten sonra oyun başlar.

### Oyunun başlangıcı
Oyun başladığında 8 tane led sırayla yanıyor(1. led yanıyor,sönüyor ardından 2. led yanıyor), en son lede geldikten sonra, bu sefer ters yönden yanıp sönmeye başlıyor. Sondan başa geldiğinde tekrar döngü başlıyor.

### Oynanış
Herhangi bir led belirleyip, gezen ışığımızı aynı anda 3 defa üst üste seçtiğimiz lede yanarken denk getirmeye çalışmak.
Eğer 3 defa üst üste seçtiğimiz led yanarken tuşa basmayı başarabilmiş isek, display'imizde seçtiğimiz ledin numarası belirir ve oyun yeniden başlar.
Eğer 2. veya 3. tuşa bastığımızda önceki seçtiğimiz lede denk getirememiş isek seçtiğimiz led için durumumuz 0'lanır döngümüz kaldığı yerden devam eder.

### Kontrol
Seçtiğimiz ledde üst üste kaçıncı defa tuttuğumuzu ise 1. displayi mizde oluşturduğumuz çizgileriden takip ederiz. Örneğin eğer seçtiğimiz ledi 2 defa üst üste yanarken denk getirmeyi başarmış isek Display de altlı üstlü 2 tane çizgi görürüz
