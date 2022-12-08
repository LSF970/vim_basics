# Basic VIM guide

## What is VIM?

VIM is a UNIX text editor that is used in Linux, BSD and MacOS. It is know for being fast and effcient, this mainly due to it's keyboard only control system. VIM is also known as Vi. 

To check VIM/Vi is installed, run the command `which vim`

## Why use VIM?

VIM is the default editor on all POSIX systems. So for example in Docker containers, where very little is installed other than the base system (for example no nano), you can still use VIM. No matter what system you use, VIM will be available.

## How to use VIM 

**Open a file with vim:**

```
sudo vim filename.txt
# or
sudo vi filename.txt
```

**To enter insert mode (to make changes):**

```
i key
```

**To go back to normal mode:**

```
Esc key
```

**Move cursor while in normal mode:**

```
h (left)
j (down)
k (up)
l (right)
```

**Save changes:**

```
:x!
```

**Save and exit:**

```
:wq
```

**Exit without saving:**

```
:q!
```

## More advanced use

**Move to a specific line in normal mode:**

```
:Line_Number

# So for example to go to line 2 

:2
```

**Move to the end of a file:**

```
:$
```

**Remove line completely (moves other lines up one):**

```
dd
```

**Undo command:**

```
u
```

**Highlight text:**

```
v # then use arrow keys or h + l to highlight text
```

**To copy (yank mode):**

```
y # (with text highlighted)
```

**To make a new line:**

```
o
```

**Paste:**

```
p
```

## Searching

**In normal mode, to search for a string:**

```
:/stringhere
```

**Go to next keyword (if multiple in document):**

```
n 
```

## VIM split

You can have two files open in one window with VIM.

**While in a file with VIM, be in normal mode and enter:**

```
:split filename.txt
```

This will open the second file below the current file.

**Switch between both windows:**

```
Ctrl + ww
```