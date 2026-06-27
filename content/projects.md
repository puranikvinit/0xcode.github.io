+++
title = "My Projects"
author = "Vinit Puranik"
description = ""
tags = ["index"]
toc = false
+++

## [rpi5os](https://github.com/puranikvinit/rpi5os)

(C, ARMv8 assembly, Raspberry Pi, OpenOCD, LLDB)

- A minimalistic kernel for the Raspberry Pi 5, which uses the bcm2712 SoC based on ARM Cortex-A76 architecture.
- Uses ARM PrimeCell PL011 UART (revision r1p5) for serial communication, with a baud rate of 9600 bps.
- Uses the ARM Corelink Generic Interrupt Controller (GIC) v2-400 for handling interrupts.
- Uses the BCM2835 ARM System Timer for scheduling and timer ticks in general.
- Implements a basic set of system calls for process management, memory management, and I/O operations.
- Comes with Virtual Memory enabled, for a physical addressable memory of 4GiB, along with the peripheral space.

## [system monitor](https://github.com/puranikvinit/system-monitor)

(C, Linux, POSIX, Sockets, Valgrind)

- Engineered a C-based Linux daemon parsing the `/proc` VFS for real-time CPU telemetry.
- Designed a POSIX-compliant multi-threaded architecture featuring a dedicated watchdog thread.
- Built a custom TCP socket server to expose scraped metrics following the OpenMetrics standard.
- Profiled application memory using Valgrind to resolve leaks and guarantee execution stability.
