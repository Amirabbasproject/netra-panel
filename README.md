🚀 Netra Panel

<p align="center">
  <img src="https://img.shields.io/badge/Cloudflare-Worker-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" />
  <img src="https://img.shields.io/badge/VLESS-Protocol-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Trojan-Protocol-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Warp-WireGuard-orange?style=for-the-badge" />
</p>📌 معرفی

Netra Panel یک پنل مبتنی بر Cloudflare Worker برای مدیریت کانفیگ‌های:

- VLESS
- Trojan
- Warp / Warp+

است که بدون نیاز به سرور اختصاصی و با استفاده از زیرساخت Cloudflare اجرا می‌شود.

📢 کانال تلگرام:
https://t.me/Frog_V2ray

---

✨ امکانات

- ✅ VLESS + WebSocket با پشتیبانی TLS
- ✅ Trojan + WebSocket با پشتیبانی TLS
- ✅ کانفیگ Warp / Warp+ مبتنی بر WireGuard
- ✅ سابسکریپشن خودکار برای:
  - v2rayNG
  - Nekoray
  - Streisand
  - Sing-box
  - Clash
- ✅ DoH Server داخلی (DNS over HTTPS)
- ✅ پنل وب فارسی و زیبا
- ✅ نصب مستقیم از داشبورد Cloudflare
- ✅ بدون نیاز به Wrangler
- ✅ بدون نیاز به دامنه اختصاصی (قابل استفاده با workers.dev)

---

🚀 نصب دستی (بدون Wrangler)

مرحله ۱: ساخت Worker

1. وارد داشبورد Cloudflare شوید:

https://dash.cloudflare.com

2. از منوی سمت چپ وارد بخش:

"Workers & Pages"

شوید.

3. روی Create کلیک کنید.

4. گزینه Hello World را انتخاب کنید.

5. یک نام برای Worker انتخاب کنید:

netra-panel

6. روی Deploy کلیک کنید.

---

مرحله ۲: قرار دادن کد Worker

1. وارد Worker ساخته‌شده شوید.
2. به بخش Edit Code بروید.
3. تمام کد پیش‌فرض را حذف کنید.
4. محتوای فایل:

worker.js

را جایگزین کنید.
5. روی Deploy کلیک کنید.

---

مرحله ۳: تنظیم متغیرهای محیطی (اختیاری)

از مسیر:

Settings → Variables

می‌توانید متغیرهای زیر را اضافه کنید:

نام متغیر| توضیحات| نمونه
"UUID"| شناسه VLESS| "550e8400-e29b-41d4-a716-446655440000"
"TROJAN_PASS"| رمز عبور Trojan| "mypassword123"
"PANEL_PATH"| مسیر پنل| "netra"
"SUB_PATH"| مسیر سابسکریپشن| "sub"

---

مرحله ۴: ورود به پنل

پس از Deploy شدن Worker، آدرس ایجادشده توسط Cloudflare را باز کنید:

https://YOUR-WORKER-NAME.YOUR-SUBDOMAIN.workers.dev

پنل Netra آماده استفاده است.
📢 کانال تلگرام:
https://t.me/Frog_V2ray

---

✨ امکانات

- ✅ VLESS + WebSocket با پشتیبانی TLS
- ✅ Trojan + WebSocket با پشتیبانی TLS
- ✅ کانفیگ Warp / Warp+ مبتنی بر WireGuard
- ✅ سابسکریپشن خودکار برای:
  - v2rayNG
  - Nekoray
  - Streisand
  - Sing-box
  - Clash
- ✅ DoH Server داخلی (DNS over HTTPS)
- ✅ پنل وب فارسی و زیبا
- ✅ نصب مستقیم از داشبورد Cloudflare
- ✅ بدون نیاز به Wrangler
- ✅ بدون نیاز به دامنه اختصاصی (قابل استفاده با workers.dev)

---

🚀 نصب دستی (بدون Wrangler)

مرحله ۱: ساخت Worker

1. وارد داشبورد Cloudflare شوید:

https://dash.cloudflare.com

2. از منوی سمت چپ وارد بخش:

"Workers & Pages"

شوید.

3. روی Create کلیک کنید.

4. گزینه Hello World را انتخاب کنید.

5. یک نام برای Worker انتخاب کنید:

netra-panel

6. روی Deploy کلیک کنید.

---

مرحله ۲: قرار دادن کد Worker

1. وارد Worker ساخته‌شده شوید.
2. به بخش Edit Code بروید.
3. تمام کد پیش‌فرض را حذف کنید.
4. محتوای فایل:

worker.js

را جایگزین کنید.
5. روی Deploy کلیک کنید.

---

مرحله ۳: تنظیم متغیرهای محیطی (اختیاری)

از مسیر:

Settings → Variables

می‌توانید متغیرهای زیر را اضافه کنید:

نام متغیر| توضیحات| نمونه
"UUID"| شناسه VLESS| "550e8400-e29b-41d4-a716-446655440000"
"TROJAN_PASS"| رمز عبور Trojan| "mypassword123"
"PANEL_PATH"| مسیر پنل| "netra"
"SUB_PATH"| مسیر سابسکریپشن| "sub"

---

مرحله ۴: ورود به پنل

پس از Deploy شدن Worker، آدرس ایجادشده توسط Cloudflare را باز کنید:

https://YOUR-WORKER-NAME.YOUR-SUBDOMAIN.workers.dev

پنل Netra آماده استفاده است.
