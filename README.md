# Systemd unit restart checker

Один из вариантов проверки перезапуска systemd unit

Необходимо определить $TIME_TICK эквивалентный таймеру крона

Создать файл конфигураций по подобию config_example и заменить нужные директивы

Example with use cron:

```cron
*/1   *   *   *   *   su -c 'cd /opt/projects/toolctl && ./main ./config' -s /bin/bash user 2>&1 >> /opt/projects/toolctl/app.log
```
