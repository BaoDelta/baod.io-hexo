title: Work with clipboard in Linux
tags:
  - linux
  - clipboard
categories:
  - Tips and Hacks
date: 2015-12-22 22:20:00
---
**Install `xclip`:**

```
$ sudo apt-get install xclip
```

**Add the following line to your `.bash_aliases` file for shortcuts:**

```
alias clip="xclip -selection c"
```

*`-selection c` is used so that you can paste to anywhere (instead of just X applications by default).*

**Copy command output to clipboard:**

```
$ <command> | clip
```

**Copy the last command to clipboard:**

```
$ fc -nl -1 | awk '{$1=$1};1' | clip
```

**Paste the text from clipboard:**

```
$ clip -o
```