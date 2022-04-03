# MyPan-build-by-Django-with-Python
基于Django开发的个人网盘

## 创建项目
#### 创建实体模型
python manage.py startapp panUser
python manage.py startapp panFile

#### 在settings.py中注册app
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'panUser',
    'panFile',
]

#### 将模型写入MYSQL
python manage.py makemigrations
python manage.py migrate
