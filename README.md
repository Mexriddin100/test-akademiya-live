# TEST AKADEMIYA LIVE — haqiqiy onlayn serverli versiya

## Ishga tushirish
Node.js 20+ o‘rnating, terminalda loyiha papkasiga o‘ting:

```bash
npm install
npm start
```

Brauzerda `http://localhost:3000` oching. Telefonlar bilan internet orqali ishlash uchun loyihani Node.js va WebSocket qo‘llaydigan HTTPS hostingga (masalan, Render Web Service yoki Railway) joylashtiring.

## Render orqali joylashtirish
1. Papkani GitHub repositoryga yuklang.
2. Render.com da New > Web Service > GitHub repositoryni tanlang.
3. Build Command: `npm install`; Start Command: `npm start`.
4. Hosil bo‘lgan `https://...onrender.com` havolasini o‘qituvchi ochadi.
5. Testni kiriting, sessiya yarating, havolani Zoom chatiga yoki Telegram guruhiga yuboring.
6. Talabalar telefon orqali kirib ism-sharif va avatar tanlaydi.
7. O‘qituvchi testni boshlaydi. Har bir javobdan keyin reyting barcha ekranlarda yangilanadi.

## Muhim cheklovlar
- Bu Node.js serveri ishlayotgan vaqtda onlayn sinxronlashni ta’minlaydi; oddiy HTML faylni yuborish yetarli emas.
- Ma’lumotlar server RAM xotirasida: qayta ishga tushganda sessiyalar yo‘qoladi. Doimiy saqlash uchun PostgreSQL/Redis qo‘shish kerak.
- O‘qituvchi boshqaruvi maxfiy token bilan cheklangan, ammo production darajadagi login, audit, rate limiting va antifraud hali qo‘shilmagan.
- Savol javoblari serverda tekshiriladi; ishtirokchiga javob kaliti yuborilmaydi.
- Telegram orqali havola ishlaydi; Telegram bot yoki Mini App integratsiyasi emas.
- Hostingni foydalanuvchi hisobida joylashtirish kerak; ChatGPT hisobga kira olmaydi.
