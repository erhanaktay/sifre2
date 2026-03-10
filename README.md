# 🔐 VaultX – Şifre Yöneticisi

Güvenli, offline çalışan, AES-256-GCM şifreli PWA şifre yöneticisi.

## Güvenlik Mimarisi
- **AES-256-GCM** — Web Crypto API ile tarayıcı içi şifreleme
- **PBKDF2** — 310.000 iterasyon ile master şifre türetme
- **Sıfır sunucu** — Tüm veriler yalnızca cihazınızda (localStorage)
- **Otomatik kilit** — 5 dakika hareketsizlikte kasa kilitlenir
- **Master şifre** — Yanlış giriş kasayı açamaz, kurtarma yok

## Özellikler
- 🔒 Master şifreli giriş ekranı
- ⚡ Güçlü şifre üreteci (uzunluk, karakter seti ayarlanabilir)
- 💪 Şifre güç analizi (Zayıf / Orta / Güçlü)
- 📁 6 kategori: Sosyal, İş, Finans, E-posta, Oyun, Diğer
- 🔍 Anlık arama
- 📋 Tek dokunuşla kopyalama
- 📤 Şifreli JSON yedekleme / geri yükleme
- 📴 Offline çalışır (Service Worker)
- 📱 iPhone ana ekran uygulaması (PWA)
- ⏱ Otomatik kilit (5 dk)

---

## GitHub Pages'e Yükleme

### 1. Repo oluştur ve yükle
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/KULLANICIADIN/vaultx.git
git push -u origin main
```

### 2. GitHub Pages aç
Repo → **Settings** → **Pages** → Source: `main` / `root` → **Save**

### 3. iPhone'a yükle
1. **Safari**'den `https://KULLANICIADIN.github.io/vaultx` aç
2. Paylaş 📤 → **Ana Ekrana Ekle** → **Ekle**
3. Ana ekrandan aç — tam uygulama gibi çalışır! 🎉

---

## ⚠️ Önemli Uyarılar
- Master şifreni unutursan veriler **kurtarılamaz** — güvenli yere not al
- Düzenli **JSON yedeği** al (Ayarlar → Dışa Aktar)
- Uygulama tarayıcı verisini temizlersen şifreler silinir
- Farklı cihazlarda kullanmak için yedek/geri yükle kullan
