# RUNBOOK (Аварийная инструкция)
## Если сервис не отвечает:
1. Проверить логи: `docker compose logs app`
2. Перезапустить: `docker compose restart app`
## Как откатить версию:
1. Открыть `compose.yaml`.
2. Заменить тег `latest` на `v1.0.0` (предыдущую версию).
3. Выполнить `docker compose up -d`.