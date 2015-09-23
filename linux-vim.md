- http://vim.wikia.com/wiki/Vim_Tips_Wiki
- http://learnvimscriptthehardway.stevelosh.com/
- http://www.vim.org/docs.php
- https://github.com/vim/vim

## Plugin Manager for Vim
- [Vundle](https://github.com/VundleVim/Vundle.vim)

## Variables
### Boolean
- `ruler` - show current line, column and percentage of total document size
- `number` - show line numbers
- `autoindent` - automatically indent on <kbd>enter</kbd> button press
- `hlsearch` - highlight all strings matching a search pattern
- `expandtab`- insert spaces on <kbd>tab</kbd> button press
- `backup` - create backup `.swp` files while editing
- `list` - display new line characters

### Integer
- `tabstop=4`
- `shiftwidth=4`

### List
- `backspace=eol,start,indent`

## Text editing
- http://vim.wikia.com/wiki/Switching_case_of_characters
- `gg=G` - reformat/reindent text
- Put `filetype plugin indent on` into `~/.vimrc` - enable java indentation

## Search
- `:%s/\n//gc` - replace newlines

## Compare
- See differences between the original file and the current buffer.
```
:w !diff % -
```

## Bulk edit
- `:args src/main/java/**/*.java | argdo execute "normal gg=G" | update` - reindent
- `:args src/main/java/**/*.java | argdo :%s/\s\+$//g | update` - remove all trailing whitespace
- `:args src/main/java/**/*.java | argdo set ff=unix | update` - convert all line terminators to unix (LF)

## File navigation
- `:o path/to/file` - open another file (requires save of changes before this)
- `:bd` - close the current file and return to previous
- `:q` - quit vim
- `:w` - save changes