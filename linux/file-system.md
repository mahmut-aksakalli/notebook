**binary directories**
- `/bin` directory contains binaries for use by all users.

- `/sbin` contains binaries to configure the operating system. Many of the system binaries require root privilege to perform certain tasks.

- `/lib` contains shared libraries.

- `/lib/modules` Linux kernel loads kernel modules from `/lib/modules/$kernel-version/`

- `/opt` is to store optional software. In many cases this is software from outside the distribution repository.

**configuration directories**

- `/etc` All of the machine-specific configuration files should be located here

- `/etc/passwd` Stores user information - Often used to see all the users on a system

- `/etc/shadow`  Has all the passwords of these users

- `/etc/sudoers` Used to control the sudo permissions of every user on the system

**data directories**

- `/home` The directory where all your downloads, documents etc are. The equivalent on Windows is `C:\Users\<user>`

- `/root` - The root user's home directory

- `/srv` is used for data that is served by your system. The FHS allows locating cvs,rsync, ftp and www data in this location.

- `/media` directory serves as a mount point for removable media devices such as CDROM's, USB.

- `/mnt` used for temporary mount points. it's used for various local and remote filesystems.

- `/tmp`  Every file inside it gets deleted upon shutdown, used for temporary files

- `/var` - Files that are unpredictable in size, such as log, cache should be located in here, most of the processes store data in `/var`
    - `/var/log`serves as a central point to contain all log files.

**in memory directories**

- `/dev` directory is populated with files as the kernel is recognising hardware.

- `/dev/tty` and `/dev/pts` For example, `/dev/tty1` represents a terminal or console attached to the system. When typing commands in a terminal that is part of a graphical interface, then your terminal will be represented as `/dev/pts/1`

- `/dev/null` black hole

- `/proc` is actually a view of the kernel 
- `/proc/interrupts` On the x86 architecture, it displays the interrupts.

**/usr**
it stands for *Unix System Resources*,contain shareable, read only data.
- `/usr/local` it can be used by an administrator to install software locally

- `/usr/include` contains general use include files for C.

- `/usr/src` is the recommended location for kernel source files.

- `$PATH` - Stores all the binaries you're able to run










