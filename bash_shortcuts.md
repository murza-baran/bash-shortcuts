Bash
====

## Moving

| command      | description                                                                         |
|--------------|-------------------------------------------------------------------------------------|
| Ctrl-a       | Goto beginning of command line                                                      |
| Ctrl-e       | Goto end of command line                                                            |
| Ctrl-b       | Move back one character                                                             |
| Ctrl-f       | Move forward one character                                                          |
| Alt-f        | Move cursor forward one word                                                        |
| Alt-b        | Move cursor back one word                                                           |
| Ctrl-] x     | Where x is any character, moves the cursor forward to the next occurance of x.      |
| Alt-Ctrl-] x | Where x is any character, moves the cursor backwards to the previous occurance of x.|


## Edit
### Delete
| command           | description                    |
|-------------------|--------------------------------|
| Ctrl-d            | Delete the character under the cursor |
| Ctrl-l            | Clear the screen (same as clear command) |
| Ctrl-u            | Clear all before cursor |
| Ctrl-k            | Clear all after cursor |
| Ctrl-w            | Delete the word before the cursor |
| Alt-[Backspace]   | Delete previous word |
| Esc-Del           | Delete previous word (may not work, instead try Esc followed by Backspace) |

### Various editing
| command           | description                                   |
|-------------------|-----------------------------------------------|
| Ctrl-t            | Swap the last two characters before the cursor |
| Ctrl-y            | Paste (if you used a previous command to delete) |
| Ctrl-_            | Undo |
| Ctrl-x Ctrl-u     | Undo. Same as previous |
| Alt-r             | Undo all changes to the line. |
| Esc-t             | Swap last two words before the cursor |
| Alt-Ctrl-e	    | Expand command line. |

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
| command           | description                                   |
|-------------------|-----------------------------------------------|
| esc-.           | |
| esc-_           | |
| Alt-?           | |
| Alt-\*           | |
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
