# my-course-repo

Ứng dụng **Django** `onlinecourse` cho khoá học trực tuyến (bài cuối khoá IBM
Skills Network), bổ sung chức năng bài kiểm tra.

## Nội dung

- `onlinecourse/models.py` — `Course`, `Lesson`, `Instructor`, `Learner`,
  `Question`, `Choice`, `Submission`.
- `onlinecourse/admin.py` — đăng ký model với trang quản trị.
- `onlinecourse/migrations/` — migration cho các model.
- `myproject/` — cấu hình Django (settings, urls, wsgi/asgi).
- `Procfile`, `manifest.yml` — cấu hình triển khai.

## Chạy

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Trang quản trị: `/admin`; API bài học: `/course/<id>/`.
