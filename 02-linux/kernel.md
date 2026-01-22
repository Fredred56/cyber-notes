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

# Linux Kernel (Basics)

## What is the kernel?
- The kernel is the core of Linux.
- It manages hardware resources and provides services for programs.

## Main responsibilities
- Process management (multitasking)
- Memory management
- Device drivers
- Filesystem drivers
- Network management

## Kernel vs Operating System
- Kernel = core component
- OS = kernel + system programs + utilities

## User space vs Kernel space
- User space: normal programs (browser, terminal tools)
- Kernel space: kernel code (drivers, memory, processes)

## Quick notes
- Kernel communicates with programs via **system calls**
- Most Linux distros share the same kernel base, but different tools/packages
