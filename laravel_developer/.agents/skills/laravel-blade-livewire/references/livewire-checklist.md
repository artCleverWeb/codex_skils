# Blade/Livewire checklist

- Версия Livewire подтверждена через Composer.
- Action повторно проверяет policy и validation.
- Public state не содержит token, secret и лишние attributes.
- Lists имеют стабильный key.
- Modal/dropdown управляют focus и Escape.
- Alpine/JS listeners не дублируются после navigation/render.
- Upload очищается при ошибке и хранится с безопасным именем.
- Тест проверяет unauthorized и invalid state.

Источники: <https://laravel.com/docs/12.x/blade> и <https://livewire.laravel.com/docs>.
