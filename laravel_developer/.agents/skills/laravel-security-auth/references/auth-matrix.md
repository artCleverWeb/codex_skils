# Выбор auth

| Сценарий | Базовый выбор |
|---|---|
| Blade/Livewire first-party web | Session guard + CSRF |
| First-party SPA/mobile/simple API tokens | Sanctum после проверки требований |
| Полноценный OAuth2 server для сторонних клиентов | Passport после подтверждения сложности |
| Внутренний service-to-service | Короткоживущая подписанная схема или инфраструктурная identity по стандарту проекта |

Проверить session fixation, logout/revocation, token expiry, rotation, abilities, tenant isolation и audit trail.

Документация: <https://laravel.com/docs/12.x/authentication>, <https://laravel.com/docs/12.x/authorization>, <https://laravel.com/docs/12.x/sanctum>, <https://laravel.com/docs/12.x/passport>.
