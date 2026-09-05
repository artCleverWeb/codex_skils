---
name: laravel-performance
description: "Диагностика и оптимизация производительности Laravel 12–13: Eloquent/SQL, cache, Redis, queues, Octane, HTTP latency, memory и profiling. Использовать для медленных запросов, высокой нагрузки, N+1, кеширования и capacity review."
---

# Производительность Laravel

1. Зафиксировать измеримую метрику и baseline; не оптимизировать по догадке.
2. Запросить разрешение до чтения production logs, profiler и БД.
3. Локализовать время между application, SQL, cache, external HTTP, queue и serialization.
4. Устранить N+1, лишние поля, joins, hydration и повторные вычисления до добавления кеша.
5. Проектировать cache key с tenant/user/locale/version и точной invalidation; не кешировать чувствительные данные публично.
6. Использовать locks для stampede и короткие TTL с jitter при высокой конкуренции.
7. Для Octane исключать request state из singleton/static, очищать ресурсы и проверять memory growth.
8. После изменения сравнить одинаковый workload, latency percentiles, queries, CPU/memory и корректность.

Чек-лист — [references/performance-checklist.md](references/performance-checklist.md).
