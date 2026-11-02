# SANO BOOKS Telegram bot — hostingga tayyor paket

## Ishga tushirish
- Python: 3.11 yoki 3.12
- Install: `pip install -r requirements.txt`
- Start: `python bot.py`

## Environment Variables
- `BOT_TOKEN` — BotFather'dan olingan yangi token
- `ADMIN_ID` — Telegram foydalanuvchi ID
- `DATABASE_URL` — SQLite manzili

## Railway
1. ZIP'ni oching. Ichidagi `sano` papkasiga kiring va uning ichidagi fayl/papkalarni (sano papkasining o'zini emas) GitHub repository ildiziga yuklang. `sano_books.db` ataylab ZIP'dan olib tashlangan: unda foydalanuvchi va buyurtma yozuvlari bor edi. `*.db` fayllarni GitHub'ga yuklamang.
2. Railway'da repository'dan service yarating.
3. Variables bo'limida `BOT_TOKEN` va `ADMIN_ID` kiriting.
4. SQLite ma'lumotlari saqlanishi uchun Volume yarating va `/data` ga ulang.
5. `DATABASE_URL` ni `sqlite+aiosqlite:////data/sano_books.db` qilib belgilang.
6. Start Command: `python bot.py`.

Muhim: `.env` va eski token paketga kiritilmagan. Eski token ZIP ichida bo'lganligi sababli BotFather'da uni bekor qilib, yangisini ishlating.
