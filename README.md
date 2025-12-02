# 👶 Yenidoğan TPN Hesaplayıcı ve Kayıt Sistemi

Bu proje, yenidoğan yoğun bakım ünitelerinde (YYBÜ) kullanılan Total Parenteral Nutrisyon (TPN) hesaplamalarını otomatize etmek ve kayıt altına almak için geliştirilmiş bir Python masaüstü uygulamasıdır.

## 🚀 Özellikler

* **Otomatik Hesaplama:** Bebek ağırlığı ve katsayılar girildiğinde tüm bileşenleri (Lipit, Aminoasit, Elektrolitler vb.) otomatik hesaplar.
* **Akıllı Glukoz Solver:** İstenen glukoz konsantrasyonuna ulaşmak için Dextroz sıvılarını (D5, D10, D20, D30, D50) matematiksel olarak en uygun oranda karıştırır.
* **Hata Önleme:** Kullanıcı hatalarını minimize eden veri doğrulama sistemleri içerir.
* **Excel Raporlama:**
    * `main_dikey.py`: Hastaları alt alta satır olarak kaydeder.
    * `main_yatay.py`: Hastaları yan yana sütun olarak karşılaştırmalı kaydeder.
* **Modern Arayüz:** CustomTkinter ile geliştirilmiş kullanıcı dostu arayüz.

## 📦 Kurulum

1. Projeyi bilgisayarınıza indirin.
2. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install -r requirements.txt
İhtiyacınıza uygun versiyonu çalıştırın:

Bash

python main_yatay.py
🛠️ Kullanılan Teknolojiler
Python 3.11+

CustomTkinter (Arayüz)

OpenPyXL (Excel İşlemleri)

📸 Ekran Görüntüleri
<img width="1097" height="915" alt="app" src="https://github.com/user-attachments/assets/06370b2d-7a71-447a-8c26-09381a7cc30f" />
<img width="775" height="992" alt="horizontal excel" src="https://github.com/user-attachments/assets/ec7c23e8-49af-47db-8fa4-48fb6dfac230" />
<img width="1676" height="984" alt="vertical excel" src="https://github.com/user-attachments/assets/d03b159c-808d-49fa-a0d7-8de84248e632" />




## 🐧 Linux Kurulumu

Bu uygulama Linux (Ubuntu, Debian, Kali vb.) üzerinde sorunsuz çalışır.

1. Terminali açın ve gerekli paketleri yükleyin:
   ```bash
   sudo apt install python3-tk
   pip3 install -r requirements.txt
Uygulamayı başlatmak için:

Bash

python3 main_linux.py
Veya Linux binary dosyası oluşturmak için:

Bash

pyinstaller --noconsole --onefile --collect-all customtkinter main_linux.py



Geliştirici: yusufdalmis
