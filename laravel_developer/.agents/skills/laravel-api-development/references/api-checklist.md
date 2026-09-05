# API checklist

- Контракт не зависит от скрытых Eloquent attributes и порядка SQL.
- Поля запроса и ответа названы последовательно; даты имеют timezone и формат.
- Policies/abilities применяются к сущности и операции.
- Mass assignment не принимает административные поля.
- Pagination links/meta и пустая коллекция проверены.
- Вебхук проверяет подпись, timestamp и replay; тяжёлая работа уходит в очередь.
- Логи не содержат Authorization, cookies, секреты и чувствительные payload.
- Feature-тесты утверждают структуру и семантику ответа.

Документация: <https://laravel.com/docs/12.x/requests>, <https://laravel.com/docs/12.x/eloquent-resources>, <https://laravel.com/docs/12.x/rate-limiting>.
