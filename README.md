# Django Library Management System

سیستم مدیریت کتابخانه با Django

## اجرا روی Hugging Face Spaces

1. این ریپو را به عنوان Space از نوع **Docker** بسازید.
2. بعد از build، سایت روی لینک Space باز می‌شود.

### حساب پیش‌فرض
- Username: admin (یا از دیتابیس موجود)
- Password: admin123 (اگر در دیتابیس تنظیم شده)

## اجرا لوکال

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
