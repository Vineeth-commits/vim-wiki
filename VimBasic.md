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
## Miscellaneous
* Use the -R option to view the file in read only mode
```bash
   vim -R filename.txt
```
* To get the actual name of the swap file execute the following command
```bash
   :swapname
```
