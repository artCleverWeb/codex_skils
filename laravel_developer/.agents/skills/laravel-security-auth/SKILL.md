---
name: laravel-security-auth
description: "Реализация и аудит безопасности Laravel 12–13: authentication, guards, sessions, Sanctum, Passport, gates, policies, CSRF, validation, uploads, encryption, secrets и защита API. Использовать для входа, токенов, ролей, прав и security review."
---

# Безопасность и авторизация Laravel

1. Определить субъектов, guards, доверительные границы, активы и операции; не выбирать Sanctum/Passport до понимания клиента.
2. Проверять authentication и authorization на сервере для каждой операции. Скрытие кнопки не является контролем доступа.
3. Использовать Policies/Gates последовательно; учитывать tenant и ownership в запросе и политике.
4. Для cookie-сессий сохранять CSRF-защиту и безопасные cookie settings. Для API выдавать минимальные abilities/scopes.
5. Валидировать по allowlist и экранировать по контексту; не использовать `{!! !!}` для непроверенных данных.
6. Защищать uploads по размеру, MIME/extension, имени и месту хранения; не доверять оригинальному имени.
7. Использовать `Hash`, `Crypt`, signed URLs и Laravel secrets APIs по назначению; не изобретать криптографию.
8. Ограничивать login/reset/OTP и чувствительные endpoints; не допускать enumeration.
9. Ранжировать findings по риску, описывать путь эксплуатации и минимальное исправление без выполнения атаки.

Перед изменением auth прочитать [references/auth-matrix.md](references/auth-matrix.md).
