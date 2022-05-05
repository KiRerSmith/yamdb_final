# YaMDb API ![example workflow](https://github.com/KiRerSmith/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)
##### В этом проекте реализован API для небольшой социальной сети YaMDb. В YaMDb пользователи могут писать рецензии к различным произведениям (книги, музыка, фильмы и т.д.), а также оставлять к рецензиям комментарии. Сами произведения в YaMDb не хранятся.  

### Технологии:
``Python 3.7``; ``Django``; ``Django REST Framework``; ``PostgreSQL``; ``Simple-JWT``; ``GitHub Actions``; ``Docker``; ``DockerHub``; ``Яндекс.Облако``

### Запуск:

Проект автоматически разворачивается на удаленном сервере по принципу Continuous Integration (Непрерывная интеграция) при помощи GitHub Actions.

Алгоритм:
1. Тестирование всего проекта после внесения измений в код;
2. Формирование контейнеров docker-compose ``web``, ``db``, ``nginx`` в образ, заливка образа в репозиторий DockerHub;
3. Деплой образа на сервер Яндекс.Облака;
4. Отправка сообщения в Telegram Bot о завершении workflow.
