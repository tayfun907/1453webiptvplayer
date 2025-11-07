# 📺 1453 Web IPTV Player

**1453 Web IPTV Player**, HLS ve DASH dahil olmak üzere modern medya akışlarını destekleyen, tek bir HTML dosyasından çalışan **tamamen istemci tabanlı** bir medya oynatıcısıdır. Kullanıcı gizliliğini ön planda tutarak, çalma listelerinizi güvenle yönetmenizi sağlar.

---

## 🔒 Güvenlik ve Gizlilik Beyanı

Bu projenin temel prensibi **maksimum kullanıcı gizliliği**dir.

* **İstemci Tarafı Çalışma:** Tüm ayrıştırma, yönetim ve oynatma işlemleri **doğrudan tarayıcınızda** gerçekleşir.
* **Veri Gizliliği:** Çalma listesi (M3U) içeriğiniz ve favori kanallarınız, geliştirici de dahil olmak üzere **hiçbir uzak sunucuya gönderilmez**. Verileriniz tarayıcınızın güvenli **IndexedDB/LocalStorage** alanında saklanır.
* **XSS Koruması:** Tüm kanal bilgileri (başlık, kategori) DOM'a eklenmeden önce temizlenir (sanitized), bu da **Cross-Site Scripting (XSS)** saldırılarına karşı tam koruma sağlar.

---

## 🚀 Başlarken

Bu aracı kullanmanın iki temel yolu vardır:

* **Canlı Kullanım (Önerilen):** Geliştiricinin sunduğu [**https://tinyurl.com/1453webiptvplayer**](https://tinyurl.com/1453webiptvplayer) adresi üzerinden aracı doğrudan tarayıcınızda kullanın.
* **Yerel Kullanım:** Kod dosyasını (`index.html`) bilgisayarınıza indirin ve herhangi bir modern tarayıcıda çift tıklayarak internet bağlantısına ihtiyaç duymadan çalıştırın.

Kullanıma başlamak için:

1.  Uygulamayı açın.
2.  Ekranın üst sağ tarafında bulunan **"+ Çalma Listesi Ekle/Yönet"** butonuna tıklayın.
3.  **URL** ile listenizi çekin veya `.m3u` / `.m3u8` dosyanızı yükleyin.

---

## ✨ Temel Özellikler

* **Gelişmiş Oynatma:** Video.js, HLS.js ve Shaka Player entegrasyonu sayesinde M3U8 (HLS), MPD (DASH) ve diğer video akışlarını sorunsuz oynatır.
* **Kalıcı Çalma Listesi:** Yüklediğiniz liste ve yaptığınız favori seçimleri tarayıcıda kalıcı olarak saklanır.
* **Favori Yönetimi:** Kanalları tek tıklamayla favorilere ekleme ve favori kanalları özel bir kategoride listeleme.
* **Liste Dışa Aktarma:** Düzenlenmiş ve favorilerle zenginleştirilmiş listenizi M3U formatında yedek olarak indirebilme.
* **Hızlı Arama:** Kanal listesi içinde anlık arama ve filtreleme.
* **Gelişmiş Kontroller:** Tam ekran (F), sesi kapatma/açma (M) gibi klavye kısayolları ve anlık çözünürlük bilgisi.
