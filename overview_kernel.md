| Ordner     | Beschreibung                                                             | Beispielinhalte                                              |
| ---------- | ------------------------------------------------------------------------ | ------------------------------------------------------------ |
| `boot/`    | Bootloader-Code, der den Kernel lädt                                     | `bootsect.S`, `setup.S`                                      |
| `tools/`   | Hilfsprogramme für die Erstellung des Boot-Images                        | `build.c` (zum Schreiben des Kernels auf Disk)               |
| `kernel/`  | Zentrales Kernel-Subsystem: Prozessverwaltung, Systemaufrufe, Timer usw. | `fork.c`, `sched.c`, `sys_call.s`, `panic.c`                 |
| `mm/`      | Speicherverwaltung: Paging, Speicherzuweisung                            | `memory.c`                                                   |
| `fs/`      | Dateisystem, Zugriff auf Dateien, Inodes, Superblöcke                    | `open.c`, `read_write.c`, `inode.c`, `super.c`, `file_dev.c` |
| `lib/`     | Standardfunktionen für Kernelgebrauch                                    | `ctype.c`, `string.c`, `vsprintf.c`, `malloc.c`              |
| `include/` | Header-Dateien mit wichtigen Strukturen und Definitionen                 | `linux/`, `asm/`, z. B. `sched.h`, `fs.h`, `system.h`        |
| `init/`    | Kernel-Startpunkt (main) nach dem Laden durch den Bootloader             | `main.c`                                                     |
| `drivers/` | Geräte-Treiber: Festplatte, Konsole, TTY                                 | `tty.c`, `hd.c`, `console.c`                                 |
