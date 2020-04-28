Bash
====

## Moving

| command      | description                                                                         |
|--------------|-------------------------------------------------------------------------------------|
| Ctrl-a       | Goto BEGINNING of command line                                                      |
| Ctrl-e       | Goto END of command line                                                            |
| Ctrl-b       | move back one character                                                             |
| Ctrl-f       | move forward one character                                                          |
| Alt-f        | move cursor FORWARD one word                                                        |
| Alt-b        | move cursor BACK one word                                                           |
| Ctrl-] x     | Where x is any character, moves the cursor forward to the next occurance of x.      |
| Alt-Ctrl-] x | Where x is any character, moves the cursor backwards to the previous occurance of x.|


## Edit
### Delete
| command           | description                    |
|-------------------|--------------------------------|
| Ctrl-d            | Delete the character under the cursor |
| Ctrl-l            | Clear the screen (same as clear command) |
| Ctrl-u            | Clear all BEFORE cursor |
| Ctrl-k            | Clear all AFTER cursor |
| Ctrl-w            | delete the word BEFORE the cursor |
| Alt-[Backspace]   | delete PREVIOUS word |
| Esc-Del           | Delete previous word (may not work, instead try Esc followed by Backspace) |

### Various editing
| command           | description                                   |
|-------------------|-----------------------------------------------|
| Ctrl-t            | swap the last two characters before the cursor |
| Ctrl-y            | paste (if you used a previous command to delete) |
| Ctrl-_            | undo |
| Ctrl-x Ctrl-u     | Undo the last changes.
| Alt-r             | Undo all changes to the line.
| Esc-t             | Swap last two words before the cursor |
| Alt-Ctrl-e	    | Expand command line.

### History
| command           | description                                   |
|-------------------|-----------------------------------------------|
| Ctrl-p            | Fetch the previous command from the history list, moving back in the list (same as up arrow) |
| Ctrl-n            | Fetch the next command from the history list, moving forward in the list (same as down arrow) |
| Ctrl-r            | Search backward starting at the current line and moving 'up' through the history as necessary |
| Crtl-s            | Search forward starting at the current line and moving 'down' through the history as necessary |
| Alt-<             | Move to the first line in the history |
| Alt->             | Move to the end of the input history, i.e., the line currently being entered |
| Alt-p		        | Non-incremental reverse search of history.
| !!		        | Execute last command in history
| !abc		        | Execute last command in history beginning with abc
| !abc:p	        | Print last command in history beginning with abc
| !n		        | Execute nth command in history
| !$		        | Last argument of last command
| !^		        | First argument of last command
| ^abc^xyz          | Replace first occurance of abc with xyz in last command and execute it
 
### Processes
| command           | description                                   |
|-------------------|-----------------------------------------------|
| Ctrl-c            | kill whatever is running |
| Ctrl-d            | Exit shell (same as exit command) |
| Ctrl-z            | Place current process in background |

### Unknown
| esc-.           | |
| esc-_           | |
| Alt-?           | |
| Alt-*           | |
| Alt-.           | print the LAST ARGUMENT (ie "vim file1.txt file2.txt" will yield "file2.txt") |
| Alt-c           | |
| Alt-d           | |
| Alt-l           | |
| Alt-n           | |
| Alt-p           | |
| Alt-r           | |
| Alt-t           | |
| Alt-u           | |
| ~[TAB][TAB]       | List all users |
| $[TAB][TAB]       | List all system variables |
| @[TAB][TAB]       | List all entries in your /etc/hosts file |
| [TAB]             | Auto complete |
| !!                | Run PREVIOUS command (ie `sudo !!`) |
| !vi               | Run PREVIOUS command that BEGINS with vi |
| cd -              | change to PREVIOUS working directory |


   
# Kill a job

n = job number, to list jobs, run `jobs`

```bash
kill %n
```

Example:

```bash
kill %1
```

## References

1. http://cnswww.cns.cwru.edu/php/chet/readline/readline.html
