# Inertia checklist

- Shared props малы и не содержат скрытые model attributes.
- Каждый mutating route имеет server validation и policy.
- Form различает processing, success, validation и network error.
- Partial reload не оставляет критичные данные устаревшими.
- Links и buttons имеют корректную семантику.
- Vue/React keys стабильны; effects/listeners очищаются.
- SSR не использует глобальное mutable request state.
- TypeScript types соответствуют реальному response contract.

Источники: <https://inertiajs.com/> и <https://laravel.com/docs/12.x/vite>.
