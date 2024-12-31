# ditana-print-system-infos

This package provides a script to print system information in Ditana GNU/Linux shells.

## Description

`ditana-print-system-infos` is a utility that displays comprehensive system information. It is not Ditana specific. It provides users with a quick overview of their system's configuration and status.

## Features

The script prints various system details, including:

- computer model, Graphics card and CPU information
- Linux distribution and family
- kernel version and GNU C Library version
- GNU C Library and GTK version
- window manager, desktop environment and Display server protocol
- various kernel settings
- the kernel parameters based on `/proc/cmdline`, with known parameters labeled descriptively; parameters that are less relevant for this output, like `BOOT_IMAGE`, are filtered out. Known parameters that do not appear in `/proc/cmdline` are displayed with the value "default".

## Usage

This package is a dependency of [ditana-config-shell](https://github.com/acrion/ditana-config-shell). The script is automatically executed when opening a bash or zsh shell in Ditana GNU/Linux.

To run the script manually:

```bash
/usr/bin/print-system-infos
```

## Example

```yaml
❯ print-system-infos
Computer model: Micro-Star International Co., Ltd. MS-7D42      Alt+SysRq+<b/e/f/s/u>:                        activated
Graphics card:  NVIDIA Corporation TU116 GeForce GTX 1660 SUPER Background Reclaiming of fs cache (0..100..): 50
CPU:            12th Gen Intel(R) Core(TM) i9-12900T            Background Memory Compaction (0..100):        1
                                                                Swappiness (0..200):                          180
Linux distribution:      Ditana GNU/Linux                       Swap Readahead (0..):                         0
Codename:                n/a                                    Extra Memory Reclaim (0..):                   0
Distro family:           arch                                   Maintain free memory (0..3000):               125
Hostname:                akino                                  Out Of Memory Kill Allocating Task:           activated
Physical CPU cores:      16                                     Unprivileged Container Access:                activated
Hyperthreading (SMT):    enabled                                Allow Performance Profiling:                  activated
Total RAM:               125 GiB                                Allow flexible device initialization:         permissive
Linux kernel version:    6.11.6-zen1-1-zen                      Audit Queue Size Limit:                       8192
GNU C Library version:   2.40                                   Audit System:                                 enabled
GTK version:             4.16.5                                 Automatically fill allocated memory with 0:   enabled
Shell:                   zsh 5.9 (x86_64-pc-linux-gnu)          Automatically fill deallocated memory with 0: enabled
Display Server Protocol: x11                                    RFDS Mitigation:                              enabled
Window Manager:          Xfwm4                                  Spectre Variant 2 Mitigation:                 enabled
Desktop Environment:     XFCE                                   Zswap Cache Layer:                            disabled
```

## Dependencies

- pciutils
- util-linux

## Installation

In Ditana GNU/Linux, this package is always installed.

For more information about Ditana GNU/Linux, visit [https://ditana.org](https://ditana.org)
