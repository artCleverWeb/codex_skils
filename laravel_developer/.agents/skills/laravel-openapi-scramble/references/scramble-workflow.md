# Scramble workflow

## Базовый порядок

1. Проверить совместимость в Composer metadata: <https://github.com/dedoc/scramble/blob/main/composer.json>.
2. Установить пакет только после согласования: `composer require dedoc/scramble`.
3. Проверить UI `/docs/api` и JSON `/docs/api.json` в локальной среде.
4. Настроить доступ к документации через `viewApiDocs` gate для иных окружений.
5. Исправлять источник контракта в Form Request/Resource/type прежде custom override.
6. Экспортировать/генерировать спецификацию командой версии пакета, подтверждённой через `artisan list` и официальную документацию.

## Проверка схемы

- `openapi` и версия 3.1 присутствуют.
- Operation ids уникальны и стабильны.
- Request body, query/path params и required совпадают с validation.
- Responses включают реальные success/error statuses.
- Resource shape, nullability, enums и pagination совпадают с JSON.
- Security scheme не содержит реальный token и назначен только защищённым операциям.
- UI/JSON недоступны неавторизованному пользователю в production.

Источники: <https://scramble.dedoc.co/>, <https://github.com/dedoc/scramble>. Scramble генерирует OpenAPI 3.1 без обязательной ручной разметки; конкретные APIs всегда сверять с установленной версией.
