# Fun vim tricks

## Useful scenarios / Magic :smile:
- See all the things you can pass into a table model with django ORM... BIG ONE!!!!
- Multiline select all lines that contain `variable = ` and comment them out
- Nesting html blocks
- Indent and exdent with:   `  > and < ` in visual mode
- I want to search to see what files reference a given variable.
  - Use cmd-shift-F to open a search in a new window. 
  - Navigate files using VIM
  - Use `gd` when over a reference I want to go directly to
- Find and replace all in a file
- Search for registration-redux in notes
  - Use `gd` to open document
  - Use `cmd F, cmd L` to open the link in browser directly from notes
  - search a selection (visual mode), find and replace with something new 
  - bounce between two markers in code
- wrap a selection in quotes

## Movement
- top/bottom of page
- go to line
- scroll up/down with cursor
- page up/down with escape + u/d
- move up/down by paragraph `{` or `}`
- move up/down by class block `[` or `]`
- e/E, b/B

## Most Common Compound
- ciw
- ea / Ea
- bi / Bi

## HOly Fuck!?
[**Vim multi-line**](https://www.barbarianmeetscoding.com/boost-your-coding-fu-with-vscode-and-vim/multiple-cursors/)
[**Vim easymotion**](https://www.barbarianmeetscoding.com/boost-your-coding-fu-with-vscode-and-vim/moving-even-faster-with-vim-sneak-and-easymotion/)
[**Vim Surround**](https://github.com/tpope/vim-surround)
[**Vim Sneak**](https://github.com/justinmk/vim-sneak)

## Folding

## Misc Basics
- Yank and put a line somewhere else
- Insert, change or delete whole line
- Insert, change or delete whole line from cursor to the end
- i/I, a/A, c/C
- ciw/ciW, delete, select, line select, ca)/ci), cit (for html)
- insert mode above/below line
- cmd-shift-enter / cmd-enter to add space

## Personal bindings
`<leader>`, `d` to add a snippet with the current year-month-day for journal entries
`<leader>`, `s` to add snippet for shell script
`<leader>`, `p` to add snippet for python script


## Not useful but still cool
- Switch between braces with `%` in normal mode.
- Capitalize text string quickly with `viW`

