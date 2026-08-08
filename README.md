# 🚀 Netra Panel

&lt;p align="center"&gt;
  &lt;img src="https://img.shields.io/badge/Cloudflare-Worker-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" /&gt;
  &lt;img src="https://img.shields.io/badge/VLESS-Protocol-blue?style=for-the-badge" /&gt;
  &lt;img src="https://img.shields.io/badge/Trojan-Protocol-red?style=for-the-badge" /&gt;
  &lt;img src="https://img.shields.io/badge/Warp-WireGuard-orange?style=for-the-badge" /&gt;
&lt;/p&gt;

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
