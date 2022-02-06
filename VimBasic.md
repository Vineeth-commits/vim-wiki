## Editing options
* Use *I* to move the cursor to the beginning of the line and switch to insert mode
* Use *a* to move the cursor by one position and switch to insert mode
* Use *A* to move the cursor to the end of the line and switch to insert mode
* Use *o* to insert a black line below the current line and switch to insert mode
* Use *s* to delete a character under the cursor and switch to insert mode
* Use *S* to delete entire line and switch to insert mode
* Use *R* to switch to replace mode
* Use *J* to join two lines
## Cut, Copy and Paster options
* Use *x* to delete character from cursor position
* Use *X* to delete previous character from cursor position
* Use *y* to copy single character from cursor position
* Use *p* to paste character after the cursor position
* Use *P* to paste character before the cursor position
## Multi-position command
* dW - delete word from cursor position
* D - delete entire line from cursor position
* dd - delete entire line
## Navigating
### Basics navigations
* h - move left
* j - move down
* k - move up
* l - move right
* Multiple positions can be moved by prefixing a number like 5j, 20l
* To move the cursor to the beginning of the line, type *0*
* To move the cursor to the end of the line, type *$*
* To scroll down entire page, type *Ctrl + f*
* To scroll up entire page, type *Ctrl + b*
### Navigating lines
* To jump to the nth line, type *:[n]*
* To jump to the start of the file, type *:0*
* To jump to the end of the file, type *:$*
## Word Navigation
* To move the cursor to the beginning of the next word, type *w*
* To move the cursor to the end of the current word, type *e*
* To move the cursor to the beginning of the previous word, type *b*
### Jumps
* To jump back to the previous position, type *Ctrl + o*
* To jump to the next position, type *Ctrl + i*

## Vim folding
* The key combination *zo* opens the fold at the cursor
* The key combination *zO* opens all the folds at the cursor
* The key combination *zc* closes a fold at the cursor
* The key combination *zm* increases the fold level by one
* The key combination *zM* closes all open folds
* The key combination *zR* all folds will open
## Vim Searching
* To perform incremental search execute following command -
```bash
:set incsearch
```
* To highlight search execute following command
```bash
:set hlsearch
```
* To disable the above -
```bash
:set noincsearch
:set nohlsearch
```
* To search in forward direction
```bash
/<expression> # Search expression in forward direction
n # Find the next occurrence
N # Find the previous occurrence
// # Repeat previous forward search
```
* To search in backward direction
```bash
?<expression> #Search expression in backward direction
n # Find previous occurance
N # Find next occurrence
?? Repeat previous backward search
```
* Search word under cursor
```bash
* # Search next occurrence of current word
# #Search previous occurrence of current word
```
* Search in multiple files
```bash
:vimgrep [search term] *.txt
:cn # Go to next occurrence of expression
:cN # Go to previous occurrence of expression
```
## Working with multiple things
* Multiple files
```bash
:e # Load new file in buffer for editing
:edit # Same as :e
:edit<tab> # List the files for editing from current directory
:edit<tab> # Same as :e<tab>
```
* Multiple Buffers
```bash
:badd<file> # Add file into new buffer
:bN # Switch to Nth buffer. For instance to switch to 3rd buffer use :b3
:bnext # Move to the next buffer in buffer list
:bprevious # Move to the previous buffer in buffer list
:buffers # List all buffers
:bfirst # Move to the first buffer
:blast # Move to the last buffer
:ball # Load all buffers
```
* Multiple tabs
```bash
:tabnew # Open new tab
:tabnew<file> # Open new file in tab
:tabclose # Close current tab
:tabnext # Move to the next tab
:tabprevious # Move to the previous tab
:tabfirst # Move to the first tab
:tablast # Move to the last tab
```
* Multiple windows
```bash
:new<file> # Open file in new window
```

## Miscellaneous
* Use the -R option to view the file in read only mode
```bash
   vim -R filename.txt
```
* To get the actual name of the swap file execute the following command
```bash
   :swapname
```
* We can undo single or multiple actions -
```bash
u # undo single action
[n]u # undo multiple actions
U # to undo all
```
* Redo is the opposite action of undo.
```bash
ctr l + r
```
