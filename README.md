# gorzdrav_spb
Скрипт мониторит свободную запись к врачу, и присылает уведомление в телеграм при ее появлении (бот @gorzdrav_spb_35_bot)

Веб-адрес сервиса для записи к врачу - https://gorzdrav.spb.ru/service-free-schedule
Выбираем район и медучреждение, потом смотрим в инструменты разработчика, и находим, что данные подгружаются из JSON. Его и будем использовать текущем скрипте.

На сервере нужно настроить cron для регулярного запуска shell скриптов gorzdrav.sh и update_doctors_specialities.sh
На сервере должен быть всегда запущен bot.py
