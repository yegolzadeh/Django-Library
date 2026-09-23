# Django Library Management System

سیستم مدیریت کتابخانه با Django

## 🚀 اجرای آنلاین روی Hugging Face Spaces (لینک عمومی)

با این روش یک لینک عمومی می‌گیری که هر کسی بتونه باز کنه و استفاده کنه.

### مراحل:

1. برو به [https://huggingface.co/spaces](https://huggingface.co/spaces) و وارد حسابت شو (اگر نداری رایگان بساز).
2. روی **Create new Space** کلیک کن.
3. تنظیمات:
   - **Space name**: مثلاً `django-library` یا هر اسمی که دوست داری
   - **SDK**: حتماً **Docker** را انتخاب کن
   - **Visibility**: Public (تا بقیه بتونن ببینن)
4. بعد از ساخت Space، فایل‌های این پروژه را آپلود کن:
   - یا همه فایل‌های داخل پوشه `django_lms` را بکش و رها کن داخل Space
   - یا از تب **Files** دکمه **Upload** را بزن و کل محتویات را آپلود کن
   - یا اگر گیت بلدی: این ریپو را push کن
5. Hugging Face خودش Docker را build می‌کند (چند دقیقه طول می‌کشد).
6. بعد از سبز شدن وضعیت، لینک Space تو این شکلی می‌شه:
   ```
   https://huggingface.co/spaces/USERNAME/SPACE-NAME
   ```
   یا مستقیم:
   ```
   https://USERNAME-SPACE-NAME.hf.space
   ```

### حساب پیش‌فرض برای ورود
- **Username**: `admin`
- **Password**: `admin123`  
  (اگر کار نکرد از دیتابیس موجود استفاده کن یا از پنل ادمین بساز)

---

## اجرا لوکال (برای تست)

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

بعد برو به: http://127.0.0.1:8000

---

## نکات مهم
- این پروژه برای دمو آماده شده (DEBUG=True و SQLite).
- فایل‌های media و دیتابیس داخل پروژه هستن.
- پورت پیش‌فرض Hugging Face: `7860` (توی Dockerfile تنظیم شده).
