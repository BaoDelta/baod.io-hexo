title: Less to view and nano to edit in Linux
tags:
  - linux
  - editor
  - viewer
categories:
  - Tips and Hacks
date: 2015-12-23 21:46:00
---
**Use `less -S` to view file with scroll:**

```
$ less -S <path>
```

- `Left`, `Right`, `Up`, `Down`, `PgUp` and `PgDn` to navigate the file
- `/` to search forward: `n` for next match in forward and `N` for previous match in backward
- `?` to search backward: `n` for next match in backward and `N` for previous match in forward
- `&` to search and display only matching lines
- `g` for the start of file and `G` for the end of file
- `q` to exit

**Use `nano` to edit file:**

```
$ nano <path>
```

- `^W` (`Ctrl+W`) to search forward
- `^WY` for the start of file and `^WV` for the end of file
- `^K` to cut text and `^U` to paste text
- `^X` to exit and `^O` to save without exiting