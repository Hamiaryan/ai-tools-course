# Kursrum AI-Verktyg (Kopia / Clone)

نسخه کامل و دقیق (Exact clone & 100% pixel-perfect) از وب‌سایت آموزشی:
[https://kursrum-ai-verktyg.pages.dev/](https://kursrum-ai-verktyg.pages.dev/)

تمامی صفحات، استایل‌ها، فونت‌های اختصاصی (Atkinson Hyperlegible, Newsreader)، آیکون‌ها، اسکریپت کپی کدها و چیدمان به صورت کامل و دقیق دانلود و سازمان‌دهی شده‌اند.

---

## 📁 ساختار پروژه (Project Structure)

```text
├── index.html                # صفحه اصلی (Start)
├── 404.html                  # صفحه خطای ۴۰۴
├── robots.txt                # تنظیمات موتورهای جستجو
├── favicon.svg               # آیکون سایت
├── _headers                  # تنظیمات هدر برای Cloudflare Pages
├── package.json              # اسکریپت‌های اجرا
├── server.js                 # سرور محلی بدون نیاز به پکیج جانبی
├── installation/             # راهنمای نصب ابزارها
│   └── index.html
├── videos/                   # لیست تمام ویدیوها و لینک‌های یوتیوب
│   └── index.html
├── ovningar/                 # بخش تمرین‌ها (Övningar)
│   ├── index.html            # فهرست اصلی تمرین‌ها
│   ├── 02/index.html         # ماژول 02
│   ├── 03/index.html         # ماژول 03
│   ├── 04/index.html         # ماژول 04
│   ├── 05/index.html         # ماژول 05
│   ├── 06/index.html         # ماژول 06
│   ├── 07/index.html         # ماژول 07
│   ├── 11/index.html         # ماژول 11
│   ├── 14/index.html         # ماژول 14
│   ├── 15/index.html         # ماژول 15
│   ├── 16/index.html         # ماژول 16
│   ├── 17/index.html         # ماژول 17
│   ├── 18/index.html         # ماژول 18
│   ├── 19/index.html         # ماژول 19
│   └── 20/index.html         # ماژول 20
├── lasanvisningar/           # راهنمای مطالعه
│   └── index.html
├── ordlista/                 # واژه‌نامه تخصصی هوش مصنوعی
│   └── index.html
├── vanliga-fragor/           # سوالات متداول (FAQ)
│   └── index.html
└── _astro/                   # فایل‌های استایل CSS و تمامی فونت‌های WOFF2/WOFF
    ├── Layout.BIaf-YTx.css
    └── *.woff2 / *.woff
```

---

## 🚀 نحوه اجرای محلی (How to Run Locally)

### روش اول: با استفاده از Node.js (پیشنهادی)
فقط کافیست در ترمینال دستور زیر را اجرا کنید (بدون نیاز به `npm install` چون سرور داخلی و بدون dependency است):

```bash
npm start
```
یا:
```bash
node server.js
```
سپس در مرورگر آدرس زیر را باز کنید:
👉 [http://localhost:3000](http://localhost:3000)

### روش دوم: با Python
```bash
python3 -m http.server 3000
```
سپس به [http://localhost:3000](http://localhost:3000) بروید.

---

## 🌐 نحوه انتشار آنلاین (Deployment)

این پروژه یک سایت استاتیک (Static Site) استاندارد است و در هر پلتفرمی با یک کلیک قابل انتشار است:

1. **Cloudflare Pages**: پوشه را به گیت‌هاب وصل کنید یا مستقیماً فولدر را در Cloudflare Pages آپلود کنید.
2. **Vercel**: دستور `npx vercel` را در این پوشه اجرا کنید.
3. **Netlify**: پوشه را در پنل Netlify بکشید و رها کنید (Drag & Drop).
4. **GitHub Pages**: پروژه را در یک ریپازیتوری گیت‌هاب پوش کنید و GitHub Pages را از شاخه `main` فعال کنید.
