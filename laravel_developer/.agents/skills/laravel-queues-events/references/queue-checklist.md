# Queue checklist

- Driver, visibility/reserved timeout и worker timeout согласованы.
- Job безопасна при повторе и параллельном выполнении.
- Unique lock имеет разумный TTL и освобождение при сбое.
- Worker restart/rolling deploy не теряет совместимость payload.
- Horizon balancing и queue priorities соответствуют SLO.
- Failed jobs не содержат секреты; есть retention и процедура восстановления.
- Scheduler использует `onOneServer` только с подходящим shared cache.
- Reverb origin, channel auth и connection limits настроены.

Документация: <https://laravel.com/docs/12.x/queues>, <https://laravel.com/docs/12.x/scheduling>, <https://laravel.com/docs/12.x/events>, <https://laravel.com/docs/12.x/reverb>.
