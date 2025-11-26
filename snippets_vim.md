#### VIM Substitute from current line to last line
## CMD
.,$s/foo/bar/g


#### VIM Substitute from current to next lines to the 2 next lines
## CMD
.,+2s/foo/bar/g


#### VIM Substitute line starting with "baz"
## CMD
g/^baz/s/foo/bar/g


#### VIM Substitute with register a
## CMD
%s/foo/<c-r>a/g


#### VIM Substitute with register a, a with many lines
## CMD
%s/foo/\=@a/g


#### VIM Substitute on each line
## delete the whole word "foo" and all following tex
## CMD
%s/\<foo\>.*//


#### VIM Grep, search for pattern in multiple files
## CMD
vim[grep] /foo/ **/*


#### VIM Sort in reverse
## CMD
%sort!


#### VIM Sort removing duplicate lines
## CMD
%sort u


#### VIM Sort numerical
## CMD
sort n


#### VIM Delete line from 3 to 5
## CMD
3,5d


#### VIM Delete all lines containing pattern
## CMD
g/{pattern}/d


#### VIM Delete all lines NOT containing pattern
## CMD
g!/{pattern}/d


#### VIM Rot13
g?


#### VIM Execute macro again
@@


#### VIM Open in default App
## in Safari for example
## CMD
open %


#### VIM Actions in Insert Mode
## Ex: Ctrl-o o, goes to the next line in insert mode
Ctrl-o then action


#### VIM Context in Insert Mode
## Ex: Ctrl-x Ctrl+p pull from context
Ctrl-x  Ctrl-p


#### VIM REDO
Ctrl-r


#### VIM Print Full Path
## Count Ctrl-g, 1 current buffer
Ctrl-g
{count}Ctrl-g 


#### VIM Insert Terminal Commands
:r! ls -l


#### VIM Lazy Config Disable Plugins
return {
  -- disable trouble
  { "folke/trouble.nvim", enabled = false },
}


#### VIM Delete Trailing characters
g_lD


#### VIM Uppercase entire line
gUU


#### VIM Move to none empty char of next line
+


#### VIM Delete line and goes into INSERT
S


#### VIM Jump to the last change
g;


#### VIM Junp back forward through the change list
g,


#### VIM Repeat last Substitute on current line
&


#### VIM Repeat last Substitute on all lines
g&


#### VIM Save and close the current file
ZZ


#### VIM Go to prarent directoy
:cd ..


#### VIM Insert Math in current line
CTRL-R=5*5


#### VIM Insert date
:r!date


#### VIM contents of the current file is sorted and only unique lines are kept
:%!sort -u

