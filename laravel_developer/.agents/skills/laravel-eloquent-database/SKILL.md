---
name: laravel-eloquent-database
description: "Проектирование, изменение и оптимизация Eloquent-моделей, relations, query builder, SQL, транзакций, schema и migrations в Laravel 12–13. Использовать для БД, индексов, casts, scopes, observers, seeders и устранения N+1."
---

# Eloquent и база данных

1. Определить СУБД и версию, существующую schema, объём данных, модели и механизм миграций.
2. Выбирать только нужные поля; применять eager loading, `withCount`/`withExists`, chunk/cursor с пониманием консистентности.
3. Не скрывать N+1 за глобальным eager loading. Проверять количество и стоимость запросов.
4. Задавать casts, fillable/guarded и relation types явно; не помещать сетевые и тяжёлые побочные эффекты в accessors.
5. Использовать транзакции для одной атомарной бизнес-операции; не держать транзакцию во время HTTP/queue вызовов.
6. Проектировать migrations для production-объёма: блокировки, backfill, nullable/default, индексы и совместимость rolling deploy.
7. Делать data migration возобновляемой и отдельной от опасного DDL, если объём значителен.
8. Запуск migrations, seeders и реальные записи/чтение БД выполнять только после согласования.

Для изменений schema прочитать [references/database-checklist.md](references/database-checklist.md).
