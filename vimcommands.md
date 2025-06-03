# Vim Commands
- VIM is a command mode editor for files in Linux.
- it has 3 modes:
    * Command mode
    * Insert mode (edit mode)
    * Extended command mode
Default mode is command mode.

## Basic Navigation
- `h` : Move left
- `j` : Move down
- `k` : Move up
- `l` : Move right
- `w` : Move the cursor forward, word by word
- `gg` : Go to first line
- `G` : Go to last line
- `:n` : Go to line number `n`

## Editing
- `i` : Insert before cursor
- `a` : Append after cursor
- `o` : Open new line below
- `O` : Open new line above
- `x` : Delete character under cursor
- `dd` : Delete current line
- `yy` : Yank (copy) current line
- `p` : Paste after cursor

## Search
- `/pattern` : Search forward for `pattern`
- `?pattern` : Search backward for `pattern`
- `n` : Next search result
- `N` : Previous search result

## Undo/Redo
- `u` : Undo
- `Ctrl + r` : Redo

## Saving and Exiting
- Done in extented command mode. Also called colon mode.
- `:w` : Save file
- `:q` : Quit
- `:wq` : Save and quit
- `:q!` : Quit without saving