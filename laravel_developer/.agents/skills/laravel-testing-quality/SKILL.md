---
name: laravel-testing-quality
description: "Создание, изменение и ревью тестов и quality tooling Laravel 12–13: PHPUnit, Pest, factories, fakes, HTTP/database tests, parallel testing, Pint, Larastan/PHPStan и CI. Использовать для регрессий, TDD и проверки качества."
---

# Тестирование и качество

1. Продолжить установленный framework и стиль тестов; не смешивать PHPUnit/Pest без причины.
2. Тестировать наблюдаемое поведение и контракт, а не внутренние private-вызовы.
3. Выбирать unit test для чистой логики, feature test для Laravel integration, browser test только при реальной UI-необходимости.
4. Использовать factories и states; создавать минимальный набор данных и явно задавать важные значения.
5. Применять Laravel fakes точечно; не подменять тестируемое поведение. Проверять dispatch/mail/notification содержательно.
6. Контролировать время, UUID и внешние HTTP через штатные средства; запрещать неожиданные внешние запросы.
7. Делать тесты независимыми от порядка, timezone, локальной БД и случайных данных.
8. Запускать сначала целевой тест, затем релевантный suite, Pint и установленный static analysis.

Матрица проверок — [references/quality-checklist.md](references/quality-checklist.md).
