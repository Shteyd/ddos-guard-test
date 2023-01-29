# ddos-guard-test

## Как использовать:
Tgbot commands:
- /start - стандартное приветствие
- /calculate %formula% - решение выраждения

HTTP server routes:
- /ping - Пинг сервера
- /v1/metrics - получение метрики (user_count)

## Немного про архитектуру:
За референс брал https://github.com/evrone/go-clean-template/

### cmd/bot && cmd/http
Точки входа в аппы

### config/
Инициализация конфига

### docker/
Докерфайлы для проекта

### internal/app
Модули запуска каждого приложения

### internal/controller/
Получение/обработка запросов в http и tg

### internal/entity/
Модели данных

### internal/infrastructure/
Слой с логикой взаимодействия с бд, сторонними библиотеками и тд.

### internal/infrastructure/mathservice
Сервис получения, обработки и отдачи ответов

### internal/infrastructure/repository
Репозиторий. Работа с БД, в моем случае с PostgreSQL

### internal/usecase
Слой юзкейсов
