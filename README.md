Python wrapper for libc reboot call, based on rust extension **rebo**.
Usage:
```python
from pylioff import reboot, LINUX_REBOOT_CMD_RESTART

with suppress(PermissionError):
   reboot(LINUX_REBOOT_CMD_RESTART)
```
Available flags: LINUX_REBOOT_CMD_CAD_ON, LINUX_REBOOT_CMD_HALT,
LINUX_REBOOT_CMD_RESTART, LINUX_REBOOT_CMD_KEXEC, LINUX_REBOOT_CMD_CAD_OFF,
LINUX_REBOOT_CMD_SW_SUSPEND, LINUX_REBOOT_CMD_POWER_OFF