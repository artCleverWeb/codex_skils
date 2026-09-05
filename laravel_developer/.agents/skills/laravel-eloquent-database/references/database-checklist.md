# Database checklist

- Уникальность защищена constraint, а не только validation.
- Foreign keys и политика удаления осознанны.
- Индекс соответствует реальным filter/order/join и проверен планом запроса.
- Денежные значения не используют float; timezone определён.
- Mass update учитывает отсутствие model events.
- `chunkById` предпочтён изменяемой пагинации по offset.
- Migration имеет безопасный deploy-порядок и стратегию отката.
- Тесты не зависят от порядка без `orderBy`.

Документация: <https://laravel.com/docs/12.x/eloquent>, <https://laravel.com/docs/12.x/queries>, <https://laravel.com/docs/12.x/migrations>.
