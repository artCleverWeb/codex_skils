---
name: laravel-api-development
description: "Создание, изменение, диагностика и ревью HTTP JSON API в Laravel 12–13: маршруты, controllers, Form Requests, API Resources, pagination, versioning, idempotency, rate limiting, webhooks и обработка ошибок. Использовать для REST-подобных API и интеграционных endpoints."
---

# HTTP API Laravel

1. Зафиксировать потребителей, контракт, версию, auth, права, лимиты и обратную совместимость.
2. Определять маршруты явно, использовать route model binding осознанно и не раскрывать внутренние ID без решения проекта.
3. Валидировать вход через Form Request или согласованный validator; авторизовать запрос отдельно от валидации.
4. Формировать публичный ответ через API Resources. Не возвращать модель или исключение напрямую.
5. Задать стабильные error codes, HTTP status и correlation id; не раскрывать stack trace и SQL.
6. Для списков использовать фильтр по allowlist, стабильную сортировку, pagination и ограничение размера страницы.
7. Защищать изменяющие retryable-запросы idempotency key либо проверкой достигнутого состояния.
8. Настроить rate limiting по реальному субъекту и сценарию; учитывать proxy configuration.
9. Проверить happy path, 401, 403, 404, 422, 429, конфликт, повтор запроса и границы пагинации.

Перед реализацией свериться с [references/api-checklist.md](references/api-checklist.md). Для OpenAPI использовать `$laravel-openapi-scramble`.
