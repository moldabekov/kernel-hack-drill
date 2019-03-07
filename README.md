# Linux kernel exploitation experiments

This is a playground for the Linux kernel exploitation experiments.
Only basic methods. Just for fun.

__Contents:__

  - __drill_mod.c__ - a small Linux kernel module with nice vulnerabilities.
  You can interact with it via a simple debugfs interface.
  - __drill_exploit_uaf.c__ - a basic use-after-free exploit.
  - __drill_exploit_nullderef.c__ - a basic null-ptr-deref exploit, which uses 
  wonderful [mmap_min_addr bypass][1] by Jann Horn.

N.B. Only basic exploit techniques here. So compile your kernel with `x86_64_defconfig`
and run it with `pti=off nokaslr`.

Have fun!

[1]: https://bugs.chromium.org/p/project-zero/issues/detail?id=1792&desc=2
