Python wrapper for libc reboot call, based on rust extension **rebo**.
Usage:
```python
from pylioff import reboot, LINUX_REBOOT_CMD_RESTART

with suppress(PermissionError):
   reboot(LINUX_REBOOT_CMD_RESTART)
```