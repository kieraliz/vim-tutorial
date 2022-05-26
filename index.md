# VIM Cheat Sheet + Tutorial

## Moving the cursor:
`h`: move cursor left <br>
`j`: move cursor down <br>
`k`: move cursor up <br>
`l`: move cursor right <br>
`0`: jump to the start of the line <br>
`$`: jump to the end of the line <br>
`gg`: go to the first line of the document <br>
`G`: go to the last line of the document <br>

## Insert mode:
`i`: insert before the cursor <br> 
`I`: insert at the beginning of the line <br>
`a`: insert/ appened after the cursor <br>
`A`: insert/ appened at the end of the line <br>
`o`: open a new line below the current line <br> 
`O`: open a new line above the current line <br>

## Edits:
`r`: replace 1 character <br> 
`R`: replace more than 1 character, until `esc` is pressed <br>
`ciw`: replace entire word <br>
`ce`: replace to the end of the word <br>
`cc`: replace an entire line <br>
`c$`: replace to the end of the line <br>
`s`: delete 1 character and substitute text <br>
`S`: delete line and substitute text <br>
`u`: undo <br>
`U`: restore the last changed line <br> 
`Ctrl` + `r`: redo <br>
`.`: repeat last command <br>

## Copy + Paste
`y`: yank/copy marked text <br>
`yy`: yank/copy a line <br>
`yw`: yank/copy the characters of the word from the cursor position up until the start of the next word <br>
`yiw`: yank/copy the word under the cursor <br>
`y$`: yank/copy to the end of the line <br>
`p`: paste the content after cursor <br>
`P`: paste the content before cursor <br>
`dd`: delete/cut a line <br>
`dw`: delete/cut the characters of the word from the cursor position up until the start of the next word <br>
`diw`: delete/cut the word under the cursor <br>
`d$`: delete/cut to the end of the line <br>
`x`: delete/cut 1 character <br>

## Exiting
`:w`: save the file (no exit) <br>
`:wq`: save the file and quit <br>
`:q`: quit (fails if there are unsaved changes <br>
`:q!`: quit and throw away all unsaved changes <br>
`:!`: run the command line without completly exiting the current editor <br>

## Searching + Replacing
`/`: search <br>
`?`: search backwards <br>
`n`: repeat search in same direction <br>
`N`: repeat search in opposite direction  <br>
`ce [replacement]` or `:s/[to replace]/[replacement]/g`: replaces the current word with the given replacement <br>
