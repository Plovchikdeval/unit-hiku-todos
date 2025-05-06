
# Dev3Quest Unit-Hiku Project

Добро пожаловать в проект UnitHiku **Dev3Quest** — инструмент для мониторинга системной информации, управления API и отображения статуса зеркал и локаций.

## Проект состоит из двух основных компонентов:

- **API** — backend-часть, отвечающая за взаимодействие с данными.
- **Bot** — Telegram-бот, предоставляющий удобный интерфейс для пользователей и администраторов.

---

## Содержание

- [Функциональность](#функциональность)
- [Структура проекта](#структура-проекта)
  - [Bot структура](#bot-структура)
  - [API структура](#api-структура)
- [TODO-файлы](#todo-файлы)
- [Контакты](#контакты)

---

## Функциональность

- Получение и отображение статуса API, зеркал и локаций.
- Отображение аптайма и ресурсов системы.
- Панель управления сообщениями.
- Обновление сообщений в реальном времени.
- Система банов пользователей.

---

## Структура проекта

### Bot структура:

```
app
├── __init__.py
├── __main__.py
├── api.py
├── arguments.py
├── commands.py
├── config.py
├── configs
│   └── maintenance.py
├── dialogs
│   ├── __init__.py
│   ├── check_dialog.py
│   ├── delete_dialog.py
│   ├── info_dialog.py
│   ├── mailing_dialog.py
│   ├── moderation_dialog.py
│   └── sample_dialog.py
├── filters
│   ├── __init__.py
│   ├── is_moder.py
│   └── is_owner.py
├── handlers
│   ├── __init__.py
│   ├── owner
│   │   ├── __init__.py
│   │   ├── auto_upd.py
│   │   ├── dev.py
│   │   ├── devs.py
│   │   ├── help.py
│   │   ├── manage_users.py
│   │   ├── mod.py
│   │   ├── mod_help.py
│   │   ├── moderate.py
│   │   ├── mods.py
│   │   ├── si.py
│   │   ├── stuff.py
│   │   └── upd.py
│   └── user
│       ├── __init__.py
│       ├── callback.py
│       ├── devs.py
│       ├── profile.py
│       ├── search.py
│       ├── start.py
│       ├── stats.py
│       └── watcher.py
├── inline
│   ├── __init__.py
│   ├── articles
│   │   ├── __init__.py
│   │   └── search.py
│   └── handlers
│       ├── __init__.py
│       └── search.py
├── keyboards
│   ├── __init__.py
│   ├── inline.py
│   └── reply.py
├── middlewares
│   ├── __init__.py
│   ├── maintenance.py
│   └── throttling.py
└── search.py

21 directories, 68 files
```

### API структура:

```
api
├── __init__.py
├── __main__.py
├── aerich_config.py
├── arguments.py
├── config.py
├── db
│   ├── __init__.py
│   ├── functions.py
│   └── models.py
├── dispatcher.py
├── handlers
│   ├── __init__.py
│   ├── db_use
│   │   └── api.py
│   ├── developer
│   │   └── api.py
│   ├── manage_server
│   │   └── api.py
│   ├── mirrors
│   │   └── api.py
│   ├── module
│   │   └── api.py
│   ├── server
│   │   └── api.py
│   ├── updates
│   │   └── api.py
│   └── user
│       └── api.py
├── pages
│   ├── login.css
│   ├── login.html
│   └── login.js
├── protect
│   └── __init__.py
├── utils
│   ├── __init__.py
│   ├── diff.html
│   ├── diff.py
│   └── parser.py
└── version.py

26 directories, 66 files
```

---

## TODO-файлы

В разработке используются следующие TODO-документы:

- [API TODO](api/TODO.md)
- [Bot TODO](bot/TODO.md)

---

## Контакты

- Автор: **Dev3Quest**
- GitHub: [Plovchikdeval](https://github.com/Plovchikdeval)

---

**Проект находится в активной разработке. Спасибо за интерес!**
