## Тестовое задание для PHP developer Vprok.ru

**Задание выполнено на фреймворке Laravel**

**Версия php 7.3**\
**СУБД MySql 5.7**

Сервис реализует JSON API работающее по HTTP. Клиент может передать в сервис URL адрес и получить для него короткую ссылку. Также клиент может передать в сервис сгенерированную короткую ссылку и получить URL, для которого она была сгенерирована.

Для использования сервиса необходимо:
- выполнить в терминале команду ```composer install``` для загрузки всех необходимых зависимостей приложения
- в конфигурации окружения (.env) задать подключение к БД
и выполнить в терминале команду ```php artisan migrate``` для создания стукрутры БД
- для запуска приложения выполнить в терминале команду ```php artisan serve```

Методы API:
- просмотр всех имеющихся коротких ссылок - GET http://127.0.0.1:8000/api/short-link
- получения короткой ссылки - POST http://127.0.0.1:8000/api/short-link?link=https://www.google.com
- получения полной ссылки по коду короткой ссылки - GET http://127.0.0.1:8000/api/short-link/123
