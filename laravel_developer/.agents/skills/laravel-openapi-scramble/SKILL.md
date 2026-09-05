---
name: laravel-openapi-scramble
description: "Установка, настройка, генерация, расширение и проверка OpenAPI 3.1 документации Laravel 12–13 через Dedoc Scramble. Использовать для автогенерации Swagger/OpenAPI из routes, Form Requests, controllers, API Resources и типов, настройки документа, security schemes, transformers и защиты UI документации."
---

# OpenAPI через Dedoc Scramble

1. Проверить Laravel/PHP и текущую версию `dedoc/scramble`; Laravel 12 работает на PHP 8.2+, Laravel 13 требует PHP 8.3+.
2. До установки пакета запросить согласование. Предпочитать актуальную совместимую stable-версию, а не фиксировать номер по памяти.
3. Сначала улучшить выводимые типы приложения: Form Requests, return types, API Resources, enums и PHPDoc там, где статический анализ не может вывести контракт.
4. Не размечать всё вручную. Добавлять Scramble attributes/extensions только для действительно невыводимого или внешнего контракта.
5. Настроить отбор API routes, metadata, servers, tags и security schemes без публикации секретов.
6. Защитить docs UI и JSON в non-local окружении через явный gate/policy; не полагаться на скрытый URL.
7. Генерировать schema детерминированно в CI и проверять, что команда завершается без ошибок.
8. Сопоставить OpenAPI с feature-тестами: status codes, validation 422, auth 401/403, pagination, errors и polymorphic responses.
9. Рассматривать schema diff как изменение публичного API; несовместимые изменения согласовывать и версионировать.

Перед настройкой прочитать [references/scramble-workflow.md](references/scramble-workflow.md).
