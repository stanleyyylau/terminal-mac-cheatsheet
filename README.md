# Terminal Cheatsheet for Mac (Basics)

- [Version en Español](https://github.com/0nn0/terminal-mac-cheatsheet/tree/master/espanol)
- [Versão em Portuguêse](https://github.com/0nn0/terminal-mac-cheatsheet/tree/master/portugues)
- [中文请参考](https://github.com/0nn0/terminal-mac-cheatsheet/tree/master/%E4%B8%AD%E6%96%87%E8%AF%B7%E5%8F%82%E8%80%83)

------------


## SHORTCUTS

| Key/Command | Description |
| ----------- | ----------- |
| Ctrl + A  | Go to the beginning of the line you are currently typing on |
| Ctrl + E  | Go to the end of the line you are currently typing on |
| Ctrl + L  | Clears the Screen |
| Command + K|Clears the Screen |
| Ctrl + U  | Clears the line before the cursor position. If you are at the end of the line, clears the entire line. |
| Ctrl + H  | Same as backspace |
| Ctrl + C  | Kill whatever you are running |
| Ctrl + D  | Exit the current shell when no process is running, or send EOF to a the running process |
| Ctrl + Z  | Puts whatever you are running into a suspended background process. fg restores it. |
| Ctrl + W  | Delete the word before the cursor |
| Ctrl + K  | Clear the line after the cursor |
| Ctrl + T  | Swap the last two characters before the cursor |
| Ctrl + F  | Move cursor one character forward |
| Ctrl + B  | Move cursor one character backward |
| Esc + F | Move cursor one word forward |
| Esc + B | Move cursor one word backward |
| Esc + T | Swap the last two words before the cursor |
| Tab | Auto-complete files and folder names |

## CORE COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| cd |  Home directory |
| cd [folder] | Change directory e.g. `cd documents` |
| cd /  | Root of drive |
| cd -  | Previous directory |
| ls | Short listing |
| ls -l | Long listing |
| ls -a | Listing incl. hidden files |
| ls -lh| Long listing with Human readable file sizes |
| ls -R | Entire content of folder recursively |
| sudo [command] | Run command with the security privileges of the superuser (Super User DO) |
| open [file] | Opens a file ( as if you double clicked it ) |
| top | Displays active processes. Press q to quit |
| nano [file] | Opens the file using the nano editor |
| vim [file] | Opens the file using the vim editor |
| clear |  Clear screen |
| reset |  Resets the terminal display |

## CHAINING COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| [command-a]; [command-b] | Run command A and then B, regardless of success of A |
| [command-a] && [command-b] | Run command B if A succeeded |
| [command-a] || [command-b] | Run command B if A failed |
| [command-a] & | Run command A in background |

## COMMAND HISTORY

| Key/Command | Description |
| ----------- | ----------- |
| history n |  Shows the stuff typed – add a number to limit the last n items |
| Ctrl + r  | Interactively search through previously typed commands |
| ![value] |  Execute the last command typed that starts with ‘value’ |
| !! |  Execute the last command typed |

## FILE MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| touch [file] |   Create new file |
| pwd | Full path to working directory |
| . |  Current folder, e.g. `ls .` |
| .. | Parent/enclosing directory, e.g. `ls ..` |
| `ls -l ..` | Long listing of parent directory |
| `cd ../../` | Move 2 levels up |
| cat | Concatenate to screen |
| rm [file] |  Remove a file, e.g. `rm data.tmp` |
| rm -i [file] | Remove with confirmation |
| rm -r [dir] | Remove a directory and contents |
| rm -f [file] | Force removal without confirmation |
| rm -i [file] |  Will display prompt before |
| cp [file] [newfile] | Copy file to file |
| cp [file] [dir] | Copy file to directory |
| mv [file] [new filename] |  Move/Rename, e.g. `mv file1.ad /tmp` |
| pbcopy < [file] | Copies file contents to clipboard |
| pbpaste | Paste clipboard contents |
| pbpaste > [file] | Past clipboard contents into file, `pbpaste > paste-test.txt` |

## DIRECTORY MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| mkdir [dir] | Create new directory |
| mkdir -p [dir]/[dir] |  Create nested directories |
| rmdir [dir] | Remove directory ( only operates on empty directories ) |
| rm -R [dir] | Remove directory and contents |
| [command] \| [command] | Allows to combine multiple commands that generate output, e.g. `cat data.txt | pbcopy` |
| less |  Output content delivered in screensize chunks |
| [command] > [file] |  Push output to file, keep in mind it will get overwritten |
| [command] >> [file] | Append output to existing file |
| [command] < [file] |  Tell command to read content from a file |

## SEARCH

| Key/Command | Description |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Search for files, e.g. `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Search for all lines that contain the pattern, e.g. `grep "Tom" file.txt` |
| grep -r [search_pattern] [file] | Recursively search for all lines that do not contain the pattern |
| grep -v [search_pattern] [file] | Search for all lines that do NOT contain the pattern |

## HELP

| Key/Command | Description |
| ----------- | ----------- |
| [command] -h |  Offers help |
| [command] —help | Offers help |
| info [command] | Offers help |
| man [command] |  Show the help manual for [command] |
| whatis [command] | Gives a one-line description of [command] |
| apropos [search-pattern] | Searches for command with keywords in description |
