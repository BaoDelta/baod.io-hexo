title: Monitor memory usage in Linux
tags:
  - linux
  - process
  - memory
categories:
  - Tips and Hacks
date: 2015-12-20 18:35:00
---
**Show amount of free and used memory:**

```
$ free -m
```

- Change the format by replacing `-m` (megabytes) with `-b` (bytes), `-k` (kilobytes) or `-g` (gigabytes)
- Watch the numbers continuously by adding `-s <seconds>` and/or `-c <times>`

**Show memory usage of all processes (in decreasing order):**

```
$ ps aux --sort -rss | less -S
```
- Sort by CPU usage by replacing `-rss` (resident set size) with `-pcpu` (cpu utilization)
- Filter the processes by piping `ps` to `grep <pattern>` and/or `head -<number of lines>`