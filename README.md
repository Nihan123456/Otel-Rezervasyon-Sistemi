🏨 Otel Rezervasyon Sistemi
C++ kullanılarak geliştirilmiş, konsol tabanlı bir Otel Rezervasyon Sistemi. Proje; oda listeleme, rezervasyon oluşturma, rezervasyon sorgulama ve verileri dosyaya kaydetme işlemlerini gerçekleştirmektedir.
📌 Proje Hakkında
Bu proje, temel C++ programlama ve veri yönetimi konularını uygulamak amacıyla geliştirilmiştir.
Sistem üzerinde toplam 5 oda bulunmaktadır. Kullanıcı, mevcut odaları görüntüleyebilir, boş bir odaya rezervasyon yapabilir ve rezervasyon numarası üzerinden rezervasyon bilgilerini görüntüleyebilir.
Program sonlandırıldığında oda ve rezervasyon bilgileri .txt dosyalarına kaydedilir.
✨ Özellikler
* 🛏️ Odaları listeleme
* 📋 Oda türlerini ve doluluk durumlarını görüntüleme
* 📝 Yeni rezervasyon oluşturma
* 🔎 Rezervasyon numarası ile rezervasyon sorgulama
* 🔢 Otomatik rezervasyon numarası oluşturma
* 💾 Oda bilgilerini odalar.txt dosyasına kaydetme
* 💾 Rezervasyon bilgilerini rezervasyonlar.txt dosyasına kaydetme
* ⚠️ Hatalı kullanıcı girişlerini kontrol etme
* 🚫 Dolu odalara tekrar rezervasyon yapılmasını engelleme
🛠️ Kullanılan Teknolojiler
* C++
* iostream
* fstream
* cstring
📚 Kullanılan C++ Konuları
Projede aşağıdaki temel programlama konuları uygulanmıştır:
* struct yapıları
* Diziler (Arrays)
* Fonksiyonlar
* Pointer kullanımı
* C-style string işlemleri
* Dosya okuma/yazma
* if / else
* switch-case
* while döngüsü
* Kullanıcı girdi kontrolü
* Global değişkenler
🗂️ Veri Yapıları
Oda
struct Oda {
    int numara;
    char tur[20];
    int dolu;
};
Her oda için oda numarası, oda türü ve doluluk durumu tutulmaktadır.
Rezervasyon
struct Rezervasyon {
    int rezervasyonNo;
    char musteriAdi[50];
    int odaNumarasi;
};
Her rezervasyon için rezervasyon numarası, müşteri adı ve oda numarası tutulmaktadır.
🖥️ Menü
Program çalıştırıldığında aşağıdaki menü kullanıcıya sunulur:
=== Otel Rezervasyon Sistemi ===
1. Odaları Göster
2. Oda Rezerve Et
3. Rezervasyonumu Göster
4. Çıkış
Seçiminizi girin:
1. Odaları Göster
Sistemde bulunan odaların:
* Oda numarasını
* Oda türünü
* Doluluk durumunu
ekrana yazdırır.
2. Oda Rezerve Et
Kullanıcı boş olan bir odayı seçerek rezervasyon oluşturabilir.
Rezervasyon sırasında:
1. Oda seçilir.
2. Müşteri adı alınır.
3. Rezervasyon numarası oluşturulur.
4. Oda dolu olarak işaretlenir.
5. Rezervasyon bilgileri bellekte saklanır.
3. Rezervasyonumu Göster
Kullanıcı rezervasyon numarasını girerek kayıtlı rezervasyon bilgilerini görüntüleyebilir.
4. Çıkış
Program sonlandırılır ve mevcut veriler dosyalara kaydedilir.
💾 Dosya Yapısı
Program çalıştırıldığında/sonlandırıldığında aşağıdaki dosyalar oluşturulur:
odalar.txt
rezervasyonlar.txt
Örnek odalar.txt:
101 TekKisilik 0
102 CiftKisilik 1
103 Suit 0
104 TekKisilik 0
105 CiftKisilik 0
Buradaki 0 odanın boş, 1 ise dolu olduğunu belirtir.
🚀 Çalıştırma
Projeyi çalıştırmak için bir C++ derleyicisine ihtiyaç vardır.
Linux / macOS
g++ main.cpp -o otel
./otel
Windows
g++ main.cpp -o otel.exe
otel.exe
Proje C++98 uyumlu olacak şekilde hazırlanmıştır.
📁 Proje Yapısı
otel-rezervasyon-sistemi/
│
├── main.cpp
├── README.md
├── odalar.txt
└── rezervasyonlar.txt
odalar.txt ve rezervasyonlar.txt program çalıştıktan sonra otomatik olarak oluşturulabilir.
🎯 Projenin Amacı
Bu proje ile C++ programlama dilinde temel veri yapıları, fonksiyonlar, dosya işlemleri ve kullanıcı etkileşimi konularında pratik yapılması amaçlanmıştır.
