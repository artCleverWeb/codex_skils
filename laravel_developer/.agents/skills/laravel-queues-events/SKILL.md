---
name: laravel-queues-events
description: "Проектирование, реализация и диагностика jobs, queues, Horizon, events/listeners, scheduler, notifications, broadcasting и Reverb в Laravel 12–13. Использовать для фоновой, отложенной, периодической и realtime-обработки."
---

# Очереди, события и realtime

1. Выбрать синхронную операцию, domain event, queued job или schedule по требованию к задержке и надёжности.
2. Передавать в job стабильные идентификаторы и компактные DTO, а не большой сериализованный object graph.
3. Делать job идемпотентной; задавать `tries`, timeout, backoff, retryUntil и unique/overlap lock осознанно.
4. Различать временные и постоянные ошибки; не превращать validation/business error в бесконечный retry.
5. Dispatch после commit выполнять через поддерживаемый after-commit механизм, когда job зависит от записанных данных.
6. Делать listeners короткими; документировать порядок только если он действительно гарантирован архитектурой.
7. Для scheduler предотвращать overlap и дубли на нескольких узлах; учитывать timezone и DST.
8. Для broadcasting/Reverb авторизовать private/presence channels и не передавать секретные payload.
9. Настроить наблюдаемость failed jobs и безопасный replay. Ручной retry/purge требует согласования.

Перед production-настройкой прочитать [references/queue-checklist.md](references/queue-checklist.md).
