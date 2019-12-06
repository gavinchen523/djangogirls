# djangogirls 
### git command 
`git remote add drangogirls git@github.com:gavinchen/drangogirls.git ` 
`git push -u origin master ` 
#### delete commit
`git reset commite-tag ` 

### install package for django 
`sudo apt-get -y install python3-mvenv python3-pip ` 

### make working directory 
`mkdir djangogirls ` 

### create venv 
`python3 -m venv venv ` 

### activee myvenv 
`. venv/bin/activate ` 

### install django(1.8) 
`pip install django==1.8 ` 

### add drango project  
`django-admin startproject mysite . ` 

### change setting 
`vi mysite/settings.py ` 

### setup database 
`vi mysite/settings.py ` 
`python manage.py migrate ` 

### run mysite 
`python manage.py runserver 0:8000 ` 

#### open browser
`http://localhost:8000 ` 

### Django 模型(Model) 
放在資料庫中的資料 

#### 創建應用程序  
`python manage.py startapp blog `  

├── blog
│   ├── admin.py
│   ├── __init__.py
│   ├── migrations
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── db.sqlite3
├── manage.py
├── mysite
│   ├── __init__.py
│   ├── __pycache__
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── README.md
└── venv
    ├── bin
    ├── include
    ├── lib
    ├── lib64 -> lib
    ├── pip-selfcheck.json
    ├── pyvenv.cfg
    └── share

##### add apps to setting 
`vi mysite/settings.py ` 


INSTALLED_APPS = (
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'blog',
)

#### 創建一個博客的資料庫
`vi blog/models.py ` 
