---
name: laravel-inertia-frontend
description: "Разработка и ревью приложений Laravel 12–13 с Inertia.js и Vue или React: pages, shared props, forms, validation, partial reloads, SSR, routing, authorization и frontend tests. Использовать для Inertia frontend и full-stack SPA-подобных интерфейсов."
---

# Inertia с Vue или React

1. Определить adapter, версии Inertia/Vue/React, TypeScript, Vite и SSR по package files.
2. Считать Laravel источником routes, validation и authorization; не дублировать бизнес-правила только на клиенте.
3. Передавать минимальные props через Resources/DTO; не шарить модель, секреты и персональные поля целиком.
4. Использовать lazy/deferred/optional props и partial reload для дорогих данных только после измерения.
5. Обрабатывать validation errors, progress, double-submit, optimistic state и server conflict.
6. Сохранять state и scroll только когда это соответствует UX; учитывать history encryption и sensitive props.
7. Для SSR исключать browser-only side effects и утечки request state между рендерами.
8. Поддерживать accessibility, responsive states и conventions выбранного component library.
9. Проверять Laravel feature contract и релевантные frontend tests/lint/typecheck.

Чек-лист — [references/inertia-checklist.md](references/inertia-checklist.md).
