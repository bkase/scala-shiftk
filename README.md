# Scala Shift-K
A better Shift-K for vim for `.scala` source code

# Installation

### Dependencies
curl - in order to download data from the internet
tidy - clean up the html that is downloaded
an internet browser - to display the documentation
 
### Vimrc
 Put this in your .vimrc:
```vim
"Better silent from slack3r here: 
"http://stackoverflow.com/questions/890802/vim-disable-press-enter-or-type-command-to-continue-prompt
command! -nargs=1 Silent
\ | execute ':silent !'.<q-args>
\ | execute ':redraw!'
" Remap Shift-K for scala files to open relavent documentation in a browser
autocmd FileType scala nnoremap K :Silent ~/.vim/scala_doc <cword> <CR>
```

### Script installation
Move `scala_doc` into your ~/.vim directory


----
_Now try using Shift-K to lookup documentation for something in the standard library!_

