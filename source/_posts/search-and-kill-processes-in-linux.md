title: Search and kill processes in Linux
tags:
  - linux
  - process
categories:
  - Tips and Hacks
date: 2015-12-24 19:38:00
---
**Search processes by a pattern:**

```
$ ps aux | grep <[p]attern> | less -S
```

*For example, you can use `grep [j]ava` to search all Java processes.*

**Search processes then kill them:**

```
$ sudo kill -9 $(ps aux | grep <[p]attern> | awk '{print $2}')
```