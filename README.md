# esp32 firmware for Homemate
..or mabye someday. At least stuff is compiling / flashing without any manual installs on WSL :O.

## Linux user
Devcontainer assumes default Linux user with UID/GID 1000 on the host machine; otherwise files won't be writeable within the devcontainer.

## Attach USB
These commands bind the specified USB-device to `/dev/ttyUSB0`. The devcontainer auto-forwards this with a bind mount.

```
usbipd wsl list
usbipd wsl attach --busid <busid>
```
