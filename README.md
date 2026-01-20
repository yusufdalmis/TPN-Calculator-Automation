# 👶 Yenidoğan TPN Hesaplayıcı ve Kayıt Sistemi
### (Neonatal TPN Calculator Automation)

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)

Bu proje, yenidoğan yoğun bakım ünitelerinde (YYBÜ) kullanılan **Total Parenteral Nutrisyon (TPN)** hesaplamalarını otomatize etmek, insan hatasını en aza indirmek ve hasta verilerini düzenli bir şekilde kayıt altına almak için geliştirilmiş açık kaynaklı bir araçtır.

## 🚀 Özellikler

* **Otomatik Hesaplama:** Bebek ağırlığı ve istenen katsayılar girildiğinde tüm sıvı, elektrolit ve besin ihtiyaçlarını anında hesaplar.
* **Akıllı Glukoz Solver (Çözücü):** Hedef glukoz yüküne (mg/kg/dk) ulaşmak için eldeki Dextroz sıvılarını (D5, D10, D20, D50) matematiksel olarak en uygun oranda karıştırır.
* **Excel Raporlama:** Hesaplanan verileri otomatik olarak Excel dosyasına kaydeder.
    * **Yatay Mod:** Hastaları yan yana sütunlar halinde karşılaştırmalı kaydeder.
* **Yuvarlama Algoritması:** Klinik pratiğe uygun olarak Cernevit'i üste (tamsayıya), diğer değerleri ise enjektör hassasiyetine (0.1) göre yuvarlar.
* **Cross-Platform:** Hem **Windows** hem de **Linux** (Pardus, Ubuntu, Kali vb.) işletim sistemlerinde çalışır.

---

## 📥 İndirme ve Kurulum (Son Kullanıcılar İçin)

Python veya kodlama bilmenize gerek yoktur. Hazır programı indirip hemen kullanabilirsiniz.

1.  Bu sayfanın sağ tarafındaki **[Releases (Sürümler)](../../releases)** kısmına tıklayın.
2.  En güncel sürümün (Örn: `v1.0.0`) altındaki **Assets** bölümünü açın.
3.  İşletim sisteminize uygun dosyayı indirin:
    * 🪟 **Windows için:** `TPN_Hesaplayici.exe`
    * 🐧 **Linux için:** `TPN_Hesaplayici_Linux`

### 🐧 Linux Kullanıcıları İçin Önemli Not
Linux güvenlik önlemleri gereği, indirilen dosyaya çalışma izni vermeniz gerekebilir:
1.  İndirdiğiniz dosyaya sağ tıklayın -> **Özellikler**.
2.  **İzinler (Permissions)** sekmesine gidin.
3.  **"Dosyayı program olarak çalıştırmaya izin ver" (Allow executing file as program)** kutucuğunu işaretleyin.
4.  Artık çift tıklayarak çalıştırabilirsiniz.

---

## 💻 Geliştiriciler İçin Kurulum (Source Code)

Projeyi geliştirmek veya kaynak kodundan çalıştırmak isterseniz:

1.  Depoyu klonlayın:
    ```bash
    git clone [https://github.com/yusufdalmis/TPN-Calculator-Automation.git](https://github.com/yusufdalmis/TPN-Calculator-Automation.git)
    cd TPN-Calculator-Automation
    ```

2.  Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install -r requirements.txt
    ```

3.  Uygulamayı başlatın:
    ```bash
    # Yatay Excel kaydı yapan versiyon için:
    python main_yatay.py
    
    # Dikey Excel kaydı yapan versiyon için:
    python main_dikey.py
    ```

## 🛠️ Kullanılan Teknolojiler

* **Dil:** Python 3.11
* **Arayüz (GUI):** CustomTkinter
* **Veri Yönetimi:** OpenPyXL (Excel entegrasyonu)
* **Derleme:** PyInstaller (EXE/Binary dönüşümü)

## 🤝 Katkıda Bulunma

Hataları bildirmek veya yeni özellikler önermek için "Issues" sekmesini kullanabilir veya bir "Pull Request" gönderebilirsiniz.

---
**Geliştirici:** Yusuf Dalmış
