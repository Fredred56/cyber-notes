# Kernel (Linux)

## What is the kernel?
- Core of the OS (runs in memory after boot)
- Manages hardware resources and provides services to programs
- Acts as bridge between software and hardware

## What the kernel does
- Process scheduling (CPU time)
- Memory management (RAM allocation)
- Device management (drivers)
- Filesystem access (read/write)
- Networking stack (TCP/IP)

## Important idea
- Users don't interact with kernel directly
- Programs use kernel via **system calls**

## Quick notes
- Kernel ≠ full OS (OS = kernel + system tools + programs)
- Kernel is always running

## Useful commands (later practice)
- `uname -r`  # kernel version
- `lsmod`     # loaded modules
- `dmesg`     # kernel messages
