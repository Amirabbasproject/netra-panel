# 🚀 Netra Panel

<p align="center">
  <img src="https://img.shields.io/badge/Cloudflare-Worker-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" />
  <img src="https://img.shields.io/badge/VLESS-Protocol-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Trojan-Protocol-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Warp-WireGuard-orange?style=for-the-badge" />
</p>

پنل **Netra** یک پنل VLESS / Trojan / Warp مبتنی بر Cloudflare Worker است که بدون نیاز به سرور اختصاصی و کاملاً رایگان کار می‌کند.

📢 **کانال تلگرام:** [t.me/Frog_V2ray](https://t.me/Frog_V2ray)

---

## ✨ ویژگی‌ها

- **VLESS + WebSocket** با پشتیبانی از TLS
- **Trojan + WebSocket** با پشتیبانی از TLS
- **Warp / Warp+** کانفیگ WireGuard
- **سابسکریپشن خودکار** برای v2rayNG, Nekoray, Streisand, Sing-box, Clash
- **DoH Server** داخلی (DNS over HTTPS)
- **پنل Web** زیبا و فارسی
- **بدون نیاز به Wrangler** - نصب مستقیم از داشبورد Cloudflare
- **بدون نیاز به دامنه** - با دامنه workers.dev کار می‌کند

---

## 🚀 نصب دستی (بدون Wrangler)

### مرحله ۱: ساخت Worker
1. به [dash.cloudflare.com](https://dash.cloudflare.com) بروید و لاگین کنید
2. از منوی سمت چب، **Workers & Pages** را انتخاب کنید
3. روی **Create** کلیک کنید
4. گزینه **"Hello World"** را انتخاب کنید
5. یک نام برای Worker خود انتخاب کنید (مثلاً `netra-panel`)
6. روی **Deploy** کلیک کنید

### مرحله ۲: آپلود کد
1. وارد داشبورد Worker خود شوید
2. به تب **Edit Code** بروید
3. **تمام کد پیش‌فرض** را پاک کنید
4. محتوای فایل `worker.js` این پروژه را **کپی و پیست** کنید
5. روی **Deploy** کلیک کنید

### مرحله ۳: تنظیم متغیرها (اختیاری)
1. در داشبورد Worker، به تب **Settings** بروید
2. روی **Variables** کلیک کنید
3. می‌توانید متغیرهای زیر را اضافه کنید:

| نام متغیر | توضیحات | مثال |
|-----------|---------|------|
| `UUID` | شناسه VLESS | `550e8400-e29b-41d4-a716-446655440000` |
| `TROJAN_PASS` | رمز Trojan | `mypassword123` |
| `PANEL_PATH` | مسیر پنل | `netra` |
| `SUB_PATH` | مسیر سابسکریپشن | `sub` |

### مرحله ۴: دسترسی به پنل
https://your-worker.your-subdomain.workers.dev/netra/panel
---

## 📱 آموزش استفاده

### v2rayNG (اندروید)
1. برنامه را از [GitHub](https://github.com/2dust/v2rayNG/releases) نصب کنید
2. روی **+** بزنید و **Import from Clipboard** را انتخاب کنید
3. وارد پنل Netra شوید و لینک VLESS یا Trojan را کپی کنید
4. در v2rayNG پیست کنید

### Streisand (iOS)
1. از App Store نصب کنید
2. **Add Configuration** > **Subscribe**
3. لینک سابسکریپشن پنل را وارد کنید:
4. https://your-worker.workers.dev/netra/sub

### Nekoray / NekoBox
1. **Server** > **Import from Clipboard** یا **Add from Subscription**
2. لینک سابسکریپشن را وارد کنید

---

## 🔗 مسیرهای مهم

| مسیر | توضیحات |
|------|---------|
| `/netra/panel` | پنل مدیریت و نمایش کانفیگ‌ها |
| `/netra/sub` | لینک سابسکریپشن (خودکار بر اساس User-Agent) |
| `/netra/warp` | کانفیگ Warp/Warp+ |
| `/dns-query` | سرور DoH (DNS over HTTPS) |
| `/netra/ip` | نمایش IP و موقعیت شما |

---

## ⚠️ نکات مهم

- این پنل برای استفاده **شخصی** طراحی شده است
- هر Worker روزانه محدودیت **۱۰۰,۰۰۰ درخواست** دارد
- برای استفاده بهتر، از **آی‌پی تمیز** (Clean IP) استفاده کنید
- کانال تلگرام ما را دنبال کنید: [@Frog_V2ray](https://t.me/Frog_V2ray)

---

## 📝 لایسنس

این پروژه تحت لایسنس MIT منتشر شده است.

---

<p align="center">
ساخته شده با ❤️ توسط Netra Team
</p>


   
