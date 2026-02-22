# Yatube

🇷🇺 [Русский](#русский) | 🇬🇧 [English](#english)

---

## Русский

Социальная сеть для публикации личных дневников. Финальный проект спринта — Яндекс Практикум.

### Возможности

- Регистрация и аутентификация пользователей
- Создание, редактирование и удаление постов
- Прикрепление изображений к постам
- Комментирование записей
- Подписка на авторов
- Лента подписок
- Группировка постов по сообществам
- Пагинация
- Кеширование главной страницы
- Кастомные страницы ошибок (404, 403, 500)

### Стек

Python 3.7, Django 2.2, SQLite3, HTML, CSS, Bootstrap, Pillow, Sorl-Thumbnail, Pytest

### Запуск

```bash
git clone https://github.com/artemleonich/hw05_final.git
cd hw05_final

python -m venv venv
source venv/bin/activate  # Linux/macOS
# venv\Scripts\activate  # Windows

pip install -r requirements.txt

cd yatube
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Приложение будет доступно по адресу http://127.0.0.1:8000/

### Тесты

```bash
pytest
```

### Структура проекта

```
hw05_final/
├── yatube/
│   ├── about/          # приложение «О проекте»
│   ├── core/           # общие шаблоны и контекст-процессоры
│   ├── posts/          # основное приложение (посты, комментарии, подписки)
│   ├── templates/      # HTML-шаблоны
│   ├── users/          # регистрация и авторизация
│   ├── yatube/         # настройки проекта
│   └── manage.py
├── tests/              # тесты
├── requirements.txt
└── README.md
```

### Автор

Артём Леонов

---

## English

A social network for publishing personal blogs. Final project of the sprint — Yandex Practicum.

### Features

- User registration and authentication
- Create, edit, and delete posts
- Attach images to posts
- Comment on posts
- Follow/unfollow authors
- Subscription feed
- Group posts by communities
- Pagination
- Main page caching
- Custom error pages (404, 403, 500)

### Tech Stack

Python 3.7, Django 2.2, SQLite3, HTML, CSS, Bootstrap, Pillow, Sorl-Thumbnail, Pytest

### Getting Started

```bash
git clone https://github.com/artemleonich/hw05_final.git
cd hw05_final

python -m venv venv
source venv/bin/activate  # Linux/macOS
# venv\Scripts\activate  # Windows

pip install -r requirements.txt

cd yatube
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

The app will be available at http://127.0.0.1:8000/

### Tests

```bash
pytest
```

### Project Structure

```
hw05_final/
├── yatube/
│   ├── about/          # "About" app
│   ├── core/           # shared templates and context processors
│   ├── posts/          # main app (posts, comments, follows)
│   ├── templates/      # HTML templates
│   ├── users/          # registration and auth
│   ├── yatube/         # project settings
│   └── manage.py
├── tests/              # tests
├── requirements.txt
└── README.md
```

### Author

Artem Leonov
