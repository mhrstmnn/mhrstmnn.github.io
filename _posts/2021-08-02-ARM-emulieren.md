---
title: "ARM emulieren"
description: "<a href='https://m.hrstmnn.de' style='color: white; text-decoration: none;'>← zurück zur Startseite</a>"
---

## GCC für ARM-Architektur

- mit `sudo apt install gcc-arm-linux-gnueabihf` installieren
- mit `arm-linux-gnueabihf-gcc FILE` kompilieren
- Optional: `sudo apt install build-essential` installieren

## QEMU user mode

- mit `sudo apt install qemu-user` installieren
- mit `qemu-arm -L /usr/arm-linux-gnueabihf/ EXEC` ausführen
- Quelle: <a href="https://yurovsky.github.io/2016/12/14/qemu-user-mode.html" target="blank">"Using qemu user mode to run cross-compiled binaries"</a>
