# Performance checklist

- Есть baseline p50/p95/p99 и объём нагрузки.
- Количество SQL и внешних HTTP измерено.
- Индекс подтверждён query plan, а не названием поля.
- Cache miss и invalidation протестированы.
- Pagination не загружает всю коллекцию в память.
- Queue throughput учитывает длительность job и retry.
- Octane не сохраняет user/request state между запросами.
- Оптимизация не ухудшила права, свежесть и консистентность.

Документация: <https://laravel.com/docs/12.x/cache>, <https://laravel.com/docs/12.x/octane>, <https://laravel.com/docs/12.x/eloquent-relationships#preventing-lazy-loading>.
