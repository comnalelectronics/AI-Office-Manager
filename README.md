# **📌 Raspberry Pi 5 ile Yüz Tanıma, Kişiye Özel Sesli Uyarı ve Ofise Giriş-Çıkış Takip Sistemi**

## **🎯 Proje Amacı**

Bu proje, **IP kamera kullanarak yüz tanıma yapmayı, tanınan kişilere özel sesli uyarılar vermeyi ve giriş-çıkış saatlerini kaydetmeyi** amaçlamaktadır. Sistem, Raspberry Pi üzerinde çalışarak veritabanına giriş ve çıkış bilgilerini kaydeder.

## **📡 Sistem Bileşenleri**

✅ **IP Kamera (RTSP Destekli)** – Görüntüyü Raspberry Pi’ye aktarır.

✅ **Raspberry Pi 5** – Görüntü işleme, yüz tanıma ve veri kaydı için kullanılır.

✅ **Hoparlör** – Tanınan kişi için sesli mesaj verir.

✅ **Python + OpenCV** – Görüntü işleme ve yüz tanıma için kullanılır.

✅ **Pyttsx3 (TTS – Text-to-Speech)** – Sesli uyarı vermek için kullanılır.

## **🛠 Çalışma Prensibi**

1️⃣ **Kamera, RTSP üzerinden Raspberry Pi’ye gerçek zamanlı görüntü aktarır.**

2️⃣ **OpenCV, yüzleri tespit eder ve veritabanındaki kişilerle karşılaştırır.**

3️⃣ **Tanımlanan kişinin adı belirlenir (Örn: Keremalp, Yusuf vb.).**

4️⃣ **Hoparlör aracılığıyla kişiye özel sesli mesaj verilir ("Hoş geldin, Keremalp!").**

## **🚀 Kullanım Senaryoları**

✅ **Ofis giriş-çıkış takip sistemi** → Çalışanların giriş-çıkış saatleri otomatik olarak kaydedilir.

✅ **Ev otomasyonu** → Tanınan kişiye özel karşılama mesajları oynatılabilir.

## **📊 Veritabanı Yapısı (SQLite / MySQL)**

| ID | Adı | Giriş Zamanı | Çıkış Zamanı |
| --- | --- | --- | --- |
| 1 | Keremalp | 2025-03-11 09:00:00 | 2025-03-11 18:00:00 |
| 2 | Yusuf | 2025-03-11 09:15:00 | 2025-03-11 17:45:00 |

💡 **Sistem, bir kişinin ofise girişini tespit ettiğinde giriş zamanını kaydeder. Çıkış yaptığında son görülme zamanını "çıkış zamanı" olarak işler.**

## **🔧 Geliştirme Aşamaları**

1️⃣ **Kameradan RTSP yayını al ve OpenCV ile yüz algılama yap.**

2️⃣ **Tespit edilen yüzleri veri tabanına kaydet ve eğit.**

3️⃣ **Tanınan kişiyi veritabanında kaydedip giriş-çıkış saatlerini tut.**

4️⃣ **Hoparlörden kişiye özel sesli mesaj ver.**

5️⃣ **Verileri raporlayabilmek için bir arayüz geliştir.**

💡 **Sonuç:** **Bu sistem, bir ofiste çalışanların giriş-çıkış saatlerini otomatik kaydeden, kişiye özel sesli uyarılar veren akıllı bir yüz tanıma sistemi olacak.** 🚀
