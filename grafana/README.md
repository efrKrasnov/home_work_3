1. Добавил в запись docker-compose для того, чтобы поднять grafana (alert-manager вывел из работы, потому что он не умеет в подтягивание переменных через энвы (как например тот же самый mimir))
2. Создал папки data и provisioning чтобы сохранять информацию о данных, генерируемых grafana
3. Задал необходимые энвы в переменных
4. Запустил docker-compose
5. Первое время grafana не могла установиться - пришлось явно укзать пользователя для соотвествующих permission
6. С помощью UI создал 2 папки - infra и app (screen-1)
7. Добавил datasource mimir (screen-2)
8. Для infra добавил из https://grafana.com/grafana/dashboards/ дашборд для node-exporter для отображения состояния железа (screen-3). Он создался в корневой папке - переместил в infra
9. Для app оттуда же добавил дашборд для blackbox-exporter (screen-4)
10. Для infra добавил оттуда же метрики для mysql (screen-5)
