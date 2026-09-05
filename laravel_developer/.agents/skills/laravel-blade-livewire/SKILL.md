---
name: laravel-blade-livewire
description: "Разработка и ревью серверного интерфейса Laravel 12–13 на Blade и Livewire: components, forms, validation, actions, uploads, events, Alpine.js, accessibility и тесты. Использовать для Blade-шаблонов и Livewire-компонентов."
---

# Blade и Livewire

1. Определить установленную версию Livewire и conventions проекта; не смешивать синтаксис разных major versions.
2. Держать Blade представлением: вычисления и бизнес-правила переносить в component/view model/service.
3. Экранировать вывод по умолчанию; использовать raw output только для доверенного и санитизированного HTML.
4. Проверять server-side validation и authorization в каждой Livewire action; public property является недоверенным вводом.
5. Ограничивать данные public state, использовать стабильные `wire:key` и не сериализовать секреты/лишние модели.
6. Обрабатывать loading, empty, error, disabled и double-submit states.
7. Для uploads проверять размер, MIME, имя и storage visibility.
8. Сохранять keyboard navigation, labels, focus и live-region для динамических сообщений.
9. Добавить component/feature tests; browser test запускать только по прямому запросу или при критичном JS-взаимодействии.

Чек-лист — [references/livewire-checklist.md](references/livewire-checklist.md).
