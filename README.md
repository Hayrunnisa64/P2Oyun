# 🚗 P2Oyun - Gelişmiş Adam Asmaca Oyunu

<!-- Teknoloji Rozetleri -->
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Swing](https://img.shields.io/badge/Java_Swing-007396?style=for-the-badge&logo=java&logoColor=white)
![File_IO](https://img.shields.io/badge/File_I%2FO-430098?style=for-the-badge&logo=databricks&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

Bu proje, **Java Swing** mimarisi ve nesne yönelimli programlama prensipleri kullanılarak geliştirilmiş; dinamik kelime havuzu, detaylı oyun logları, skor takibi ve şifre korumalı yönetim mekanizmalarına sahip gelişmiş bir masaüstü **Adam Asmaca** uygulamasıdır.

---

## 📌 İçindekiler
* [✨ Özellikler](#-özellikler)
* [🛠️ Kullanılan Teknolojiler](#️-kullanılan-teknolojiler)
* [📂 Proje Dosya Yapısı](#-proje-dosya-yapısı)
* [⚙️ Kurulum ve Çalıştırma](#️-kurulum-ve-çalıştırma)
* [📸 Ekran Görüntüleri](#-ekran-görüntüleri)

---

## ✨ Özellikler

| Özellik | Açıklama |
| :--- | :--- |
| 🎲 **Dinamik Kelime Seçimi** | Oyun başladığında `kelimeler.txt` dosyasından rastgele kelime seçilir ve harf sayısına göre dinamik arayüz (`*`) oluşturulur. |
| 🔠 **Esnek Tahmin Sistemi** | Kullanıcı ister tek tek harf tahmini yapar, isterse doğrudan kelime tahminiyle risk alabilir. |
| ⏳ **Zamanlayıcı (Timer)** | Swing `Timer` sınıfı kullanılarak oyun süresi anlık olarak saniye cinsinden hesaplanır ve ekranda gösterilir. |
| 📊 **Skor ve Veri Yönetimi** | Tamamlanan oyunların tarih, süre ve kazanma durumları `oyunlar.txt` dosyasına kalıcı olarak kaydedilir ve tabloda listelenir. |
| 🔓 **Güvenli Yönetici Paneli** | Skor geçmişi ve sistem logları, `sifre.txt` içerisindeki şifre doğrulanarak yetkili kişilerce temizlenebilir. |

---

## 🛠️ Kullanılan Teknolojiler

*   **Dil ve Çalışma Zamanı:** Java (JDK 17)
*   **Grafik Arayüz (GUI):** Java Swing (JFrame, JTabbedPane, JTable, JPanel, FlowLayout)
*   **Asenkron İşlemler:** `javax.swing.Timer` (Süre takibi için)
*   **Veri Yönetimi:** `java.nio.file.Files`, `java.io.FileWriter` (Dinamik Dosya I/O İşlemleri)

---

## 📂 Proje Dosya Yapısı

Uygulamanın yerel makinede stabil çalışabilmesi ve dosya okuma/yazma işlemlerini hatasız yürütebilmesi için aşağıdaki dizin şemasının kurulması gerekmektedir:

```text
C:\P2Oyun\
├── Resimler\
│   ├── 1.jpg          # İlk aşama görseli
│   ├── ...
│   └── 11.jpg         # Son aşama (Oyun Bitti) görseli
└── TXTDosyalar\
    ├── kelimeler.txt  # Oyunda çıkacak kelime havuzu
    ├── oyunlar.txt    # Geçmiş oyun skorlarının tutulduğu dosya
    ├── sifre.txt      # Admin paneli temizleme şifresi
    └── log.txt        # Sistem işlem geçmişi logları
