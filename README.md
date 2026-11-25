# RFID Tetiklemeli Akıllı Görüntü Yakalama ve Geçiş Kontrol Sistemi

## Proje Tanımı ve Çözdüğü Problem
Geleneksel RFID tabanlı geçiş kontrol sistemleri yalnızca kart kimliğini (UID) doğrulamakta, ancak kartı okutan kişinin gerçekten kart sahibi olup olmadığını veya geçiş anındaki fiziksel durumu kayıt altına almamaktadır. Bu proje; yetkili veya yetkisiz her RFID kart okutma anında yüksek çözünürlüklü görüntü yakalayarak kart taklitçiliği (cloning) ve izinsiz geçiş kaynaklı güvenlik açıklarını ortadan kaldırmayı amaçlamaktadır.

## Hedef Kitle
Sistem; laboratuvarlar, üniversite atölyeleri, sunucu odaları ve düşük maliyetli ancak görsel doğrulamalı fiziksel güvenlik ihtiyacı duyan küçük ve orta ölçekli kurumlar için geliştirilmiştir.

## Donanım ve Yazılım Mimarisi
- **Mikrodenetleyici:** Deneyap Kart v2 (ESP32-S3, 8 MB OPI PSRAM)
- **Görüntüleme Modülü:** OV2640 Kamera Sensörü (DVP / SCCB arayüzü)
- **Kimlik Doğrulama:** MFRC522 RFID Okuyucu (SPI arayüzü)
- **Geliştirme Ortamı:** PlatformIO & ESP-IDF (C / FreeRTOS)
