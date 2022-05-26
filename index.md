# How to use VIM: A Tutorial and Cheat Sheet

VIM is a powerful tool that allows us to work on machines that do not have a graphical user interface, such as accessing remote servers or editing on the cloud. For these situations, we do not have the option of using VSCode or other editors. Instead, we can use a terminal-based text editor to make changes to our code. 

## Vim Grammar:

Verb + Modifier + Noun

*Verbs*: Signifies actions, ie. yank, delete, etc <br>
*Modifiers*: Signifies precisely where an action should be executed, ie. inside, around, etc <br>
*Nouns*: Signifies the item on which the action is performed, ie. word, sentence, paragraph, etc <br>

### Examples:
* diw: deletes the current word, Delete Inside Word
* d3w: deletes 3 words
* cis: changes the current sentence, Change Inside Sentence
* ci": changes the content inside " "

## Command Mode and Insert Mode
Command mode is the default/ normal mode, typically used for viewing. Command mode allows for efficient navigation and editing of existing text. <br>
Insert mode is the editing mode to directly insert or change content. <br>
Use `i` to switch from Command Mode &rarr; Insert Mode <br>
Use the escape key `esc` to switch from Insert Mode &rarr; Command Mode <br>

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

## Modifiers:
`i`: inside <br> 
`a`: around <br>
`t`: til find a character, exclusive of the character <br>
`f`: find a character, inclusive of the character <br>

## Objects:
`w`: to the start of the next word <br> 
`e`: to the end of the current word <br>
`s`: sentence <br>
`b`: block/ parentheses <br>
`p`: paragraph <br>

## Edits:
`r`: replace 1 character <br> 
`R`: replace more than 1 character, until `esc` is pressed <br>
`ciw`: replace entire word <br>
`ce`: replace until the end of the word <br>
`cc`: replace until the end of the entire line <br>
`c$`: replace to the end of the line <br>
`ce [replacement]` or `:s/[to replace]/[replacement]/g`: replaces the current word with the given replacement <br>
`s`: delete 1 character and substitute text <br>
`S`: delete line and substitute text <br>
`u`: undo (can be done multiple times) <br>
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
`x`: delete/cut char <br>
`r`: splits a line between words <br>
`J`: combines two lines together <br>

## Searching
`/<search-phrase>`: searches for the given search phrase <br>
`?`: search backwards for the given search phrase <br>
`n`: repeat search in same direction <br>
`N`: repeat search in opposite direction  <br>
`:set hlsearch`: enables highlighted search <br>

## File Interactive Commands
`vim <file-name>`: edits an existing file, or creates a new one if the file name does not exist <br>
`Ctlr` + `G`: shows your location in the file <br>
`:set nu`: enables line numbers on the editor <br>
`:w`: save the file (no exit) <br>
`:wq`: save the file and quit <br>
`:q`: quit, exists without changes assuming no changes have been made <br>
`:q!`: quit forcefully and throw away all unsaved changes <br>
`:!`: execute a single unix command from without completly exiting the current editor <br>
`:sh`: temporarily return to the shell use <br>
`:f`: display the name of the current file in use <br>

## References + More Articles:
* [Mastering Vim Grammar](https://irian.to/blogs/mastering-vim-grammar/)
* [Learn to speak vim - verbs, nouns, and modifiers!](https://yanpritzker.com/learn-to-speak-vim-verbs-nouns-and-modifiers-d7bfed1f6b2d)
* [Vim Cheat Sheet](https://vim.rtorr.com/)
