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

## 🌐 ساختار دو پلتفرم مستقل (Two Separate Platforms)

این پروژه اکنون شامل دو پلتفرم مجزا و هماهنگ است:

1. **پلتفرم ۱: سایت مرجع دوره‌ها (Kursrum AI-Verktyg)**
   - پورت لوکال: 👉 **[http://localhost:3001](http://localhost:3001)**
   - شامل تمام ۲۱ صفحه آموزشی، راهنمای نصب، ویدیوها و تمام تمرین‌ها به ۳ زبان (سوئدی، انگلیسی و فارسی با RTL).

2. **پلتفرم ۲: پرتال آموزشی Omniway LMS**
   - پوشه: `omniway-platform/`
   - پورت لوکال: 👉 **[http://localhost:3002](http://localhost:3002)**
   - ظاهر دقیق (Exact UI/UX) سامانه Omniway با تم سبز جنگلی (`#1b382b`)، تب‌های درسی، هفته‌های آموزشی، جعبه‌های تحویل تکالیف و لینک‌های متصل به پلتفرم ۱.

---

## 🚀 نحوه اجرای لوکال (Running Locally)

### پلتفرم اصلی (Kursrum):
```bash
npm start
# یا node server.js -> پورت 3001
```

### پلتفرم Omniway:
```bash
cd omniway-platform
npm start
# یا node server.js -> پورت 3002
```


---

## 🌐 نحوه انتشار آنلاین (Deployment)

این پروژه یک سایت استاتیک (Static Site) استاندارد است و در هر پلتفرمی با یک کلیک قابل انتشار است:

1. **Cloudflare Pages**: پوشه را به گیت‌هاب وصل کنید یا مستقیماً فولدر را در Cloudflare Pages آپلود کنید.
2. **Vercel**: دستور `npx vercel` را در این پوشه اجرا کنید.
3. **Netlify**: پوشه را در پنل Netlify بکشید و رها کنید (Drag & Drop).
4. **GitHub Pages**: پروژه را در یک ریپازیتوری گیت‌هاب پوش کنید و GitHub Pages را از شاخه `main` فعال کنید.
