title: Free up disk space in Linux
tags:
  - linux
  - disk space
categories:
  - Tips and Hacks
date: 2015-12-21 20:09:00
---
**Show amount of free and used disk space:**

```
$ df -h
```

**Locate top `100` largest files or directories in current directory `.`:**

```
$ sudo du -a . | sort -nr | head -100
```

- The command will be slow, if there are a lot of files or directories
- Limit how deep to visit subdirectories by adding `-d <max depth>`
- Using `-t <size threshold>` to set minimum (negative) or maximum (positive) size