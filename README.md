# Systemd unit restart checker

To run, you need to describe the configuration file and execute app with him

Example with use cron:

```cron
*/1   *   *   *   *   su -c 'cd /opt/projects/toolctl && ./main ./config' -s /bin/bash user 2>&1 >> /opt/projects/toolctl/app.log
```
