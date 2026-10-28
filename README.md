# ☀️ Ob-Havo Pro — Mukammal Ob-Havo Platformasi

O'zbekiston viloyatlari va butun dunyo shaharlarining real vaqtdagi ob-havosi, 24 soatlik interaktiv grafikli prognozi, 7 kunlik haftalik kutilma, havo sifati indeksi (AQI) hamda quyosh/oy holatini ko'rsatib beruvchi zamonaviy veb-platforma.

![Ob-Havo Pro](https://img.shields.io/badge/Status-Production%20Ready-emerald?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![API](https://img.shields.io/badge/API-Open--Meteo-cyan?style=for-the-badge)
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FJahon214%2Fweather)

---

## 🌟 Asosiy Imkoniyatlar (Features)

1. **⚡ Real Vaqt Rejimida Aniq Ma'lumotlar**:
   - Harorat, his qilinishi (Feels Like), min/maks ko'rsatkichlar.
   - Havoning namligi, shamol tezligi va yo'nalishi.
   - Atmosfera bosimi (mm simob ustuni formatida).
   - UV (ultrabinafsha nurlanish) indeksi.
   - Aniq ko'rinuvchanlik darajasi (Visibility - km).

2. **🏙 O'zbekiston Viloyatlari va Dunyo Shaharlari**:
   - O'zbekistonning barcha 14 ta ma'muriy hududi (Toshkent sh., Samarqand, Buxoro, Andijon, Farg'ona, Namangan, Qarshi, Termiz, Urganch, Nukus, Jizzax, Guliston, Navoiy, Nurafshon).
   - Dunyoning yirik megapolislari (Istanbul, London, Moskva, Dubay, Nyu-York, Tokio).

3. **📍 Haqiqiy Geolokatsiya va Shaharni Avtomatik Aniqlash**:
   - "Mening Joylashuvim" tugmasi bosilganda GPS koordinatalar orqali siz turgan haqiqiy shahar nomini avtomatik aniqlaydi.

4. **🔍 Tezkor va Aqlli Qidiruv (Open-Meteo Geocoding)**:
   - Dunyoning istalgan shahrini lotin yoki kirill alifbosida yozib bir zumda qidirib topish.
   - Klaviaturada `/` tugmasi orqali qidiruv maydonini ochish.

5. **📊 24 Soatlik Prognoz va Dinamik Chart.js Grafiki**:
   - Har soatdagi harorat o'zgarishini qulay vizual chiziqli grafikda ko'rsatadi.

6. **📅 7 Kunlik Haftalik Ob-havo**:
   - Haftaning har bir kuni uchun kutilayotgan ob-havo holati va harorat diapazoni.

7. **🍃 Havo Sifati Indeksi (AQI - European Standard)**:
   - PM2.5 va PM10 zarrachalari miqdori hamda salomatlik uchun tavsiyalar.

8. **🌗 Kun va Tun Rejimi (Day/Night Theme)**:
   - Kunduzi quyoshli va iliq animatsiyalar, kechasi esa oydin tun va miltillovchi yulduzlar effektlari.
   - Yomg'ir, qor va momaqaldiroq vaqtida jonli Canvas animatsiyasi.

9. **⭐ Sevimlilar (Favorites) & Harorat Birligi (°C / °F)**:
   - Istalgan shaharni sevimlilarga qo'shish va olib tashlash.
   - Selsiy va Farengeyt o'rtasida bir klik bilan o'tish.
   - Oxirgi ko'rilgan shahar brauzer xotirasida (`localStorage`) saqlanib qoladi.

---

## 🛠 Ishlatilgan Texnologiyalar

- **HTML5 & CSS3** (Zamonaviy Glassmorphism dizayn)
- **Tailwind CSS** (Utility-first styling)
- **Vanilla JavaScript (ES6+)** (Yuqori tezlik, hech qanday ortiqcha framework yuklamasisiz)
- **Chart.js** (Interaktiv harorat grafigi)
- **Font Awesome 6 & Google Fonts (Plus Jakarta Sans)**
- **Open-Meteo API** (Bepul, cheklovsiz va API-kalit talab qilmaydigan professional ob-havo API)
- **BigDataCloud API** (Geolokatsiya teskari geokodlash)

---

## 🚀 Mahalliy Kompyuterda Ishga Tushirish (Local Setup)

Hech qanday murakkab sozlash shart emas. Loyihani yuklab oling va `index.html` faylini istalgan brauzerda oching!

Yoki lokal serverda ishga tushirish uchun:
```bash
# Repozitoriyani klonlash
git clone https://github.com/Jahon214/weather.git

# Loyiha papkasiga o'tish
cd weather

# Lokal serverda ochish (Node.js orqali)
npx serve .
```

---

## 📦 GitHub va Vercel'ga Joylash Bo'yicha Qo'llanma

### 1-qadam: GitHub'ga joylash

1. [GitHub.com](https://github.com/new) saytiga kiring va yangi repozitoriya yarating (masalan: `weather` yoki `ob-havo-pro`).
2. Terminalda (PowerShell yoki Git Bash) quyidagi buyruqlarni ketma-ket bajaring:

```bash
# Asosiy tarmoqqa o'tish
git branch -M main

# O'z GitHub repozitoriyangiz manzilini ulang (o'zingiz yaratgan repo linki bilan almashtiring):
git remote add origin https://github.com/Jahon214/weather.git

# O'zgarishlarni GitHub'ga yuklash:
git push -u origin main
```

---

### 2-qadam: Vercel'ga joylash (Deploy to Vercel)

Vercel — bu statik saytlar uchun dunyodagi eng tezkor va bepul hosting platformasi.

#### Variant A: Vercel sayti orqali (Tavsiya etiladi - 1 daqiqa)
1. [vercel.com](https://vercel.com) saytiga kiring va **"Continue with GitHub"** tugmasi orqali kiring.
2. Dashboard'da **"Add New..."** -> **"Project"** tugmasini bosing.
3. GitHub ro'yxatidan o'zingiz yuklagan `weather` repozitoriyasini topib, **"Import"** tugmasini bosing.
4. Hech qanday sozlamani o'zgartirish shart emas — to'g'ridan-to'g'ri **"Deploy"** tugmasini bosing.
5. 10-20 soniyada loyihangiz butun dunyoga ochiq bo'lgan bepul `https://weather-....vercel.app` domeni orqali ishga tushadi!

#### Variant B: Terminal orqali (Vercel CLI)
```bash
# Vercel orqali deploy qilish
npx vercel
```
Terminaldagi savollarga `Enter` bosib davom etsangiz, loyihangiz darhol deploy bo'ladi.

---

## 📄 Litsenziya

Ushbu loyiha [MIT](LICENSE) litsenziyasi asosida ochiq manbalidir.
