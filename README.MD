# MICROMENU

Micromenu is a little shellscript developed to enabled limited devices (in terms of I/O and hardware) to have sort of a front-end selector for applications. It was created for Dingux back in 2009 when people started to hack and modify handheld game devices.
It works parsing text files to create the selector on screen. It may work on other devices like GP2x, Pandora and Caanoo.

# PERFORMANCE

Other front-end applications like Dmenu or Gmenu keep around 4~6MB stuck on memory representing 25% of the actual memory of the device. Micromenu has a small footprint and doesn't interfere like the others do.

# USAGE

Copy the `main` file to your `/usr/local/sbin/main`.
To customize entries edit the file `menu`. You can chain multiple sub-menus, see the `menu-inc` and `samples-inc` to get an idea.

**syntax:** `(display name)|(working dir)|(executable)|parms`

**parms:**
*--keep*: make the executable run again when closed.
