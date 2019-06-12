# Environment

### language / framework

- Python3 / Django

### package

- api design : Django REST framework
- pdf to image processing : wand / ImageMagick

### command

- 安裝套件 : `pip install -r requirements.txt`
- 建 DB : `python manage.py migrate`
- 啟動 : `python manage.py runserver`
- 其餘請參考 [Django 文件](https://docs.djangoproject.com/en/1.10/) ( 1.10 )

### database

- 使用 `SQLite` 資料庫
- migrate 時有參考 settings.py 裡的 `DOMAIN` ( 要注意，不然資料會變髒 )

### imagemagick

> 需先另行安裝

- 請使用 Version 6
- [官網下載區](https://imagemagick.org/download/windows/) 可載到舊版本的