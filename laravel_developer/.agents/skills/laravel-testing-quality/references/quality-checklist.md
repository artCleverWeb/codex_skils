# Quality checklist

- Регрессия сначала воспроизводит ошибку и падает без исправления.
- Проверены успех, validation, authorization и ключевой edge case.
- DB assertions проверяют эффект, а response assertions — контракт.
- Не используются sleeps; асинхронность контролируется fake или polling с deadline.
- Parallel tests не делят mutable state.
- Pint запускается на изменённых файлах или по правилам проекта.
- Larastan/PHPStan baseline не расширяется без объяснения.
- CI-команды взяты из проекта, а не придуманы.

Документация: <https://laravel.com/docs/12.x/testing>, <https://laravel.com/docs/12.x/http-tests>, <https://laravel.com/docs/12.x/mocking>.
