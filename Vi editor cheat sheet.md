## Movement Commands
### Character
h, j, k, l Left, down, up, right
Text
w, W, b, B Forward, backward by word
e, E End of word
(, ) Beginning of next, previous sentence
{, } Beginning of next, previous paragraph
\[\[, ]] Beginning of next, previous section
### Lines
0, $ First, last position of current line
^ First non blank character of current line
+, - First character of next, previous line
H Top line of screen
M Middle line of screen
L Last line of screen
n H, n L Line n from top, bottom of screen
### Scrolling
\[Ctrl]F, \[Ctrl]B Scroll forward, backward one screen
\[Ctrl]D, \[Ctrl]U Scroll down, up one half screen
\[Ctrl]E, \[Ctrl]Y Show one more line at bottom, top of window
z\[Enter] Scroll until line with cursor is at top of screen
z. Scroll until line with cursor is at middle of screen
z- Scroll until line with cursor is at bottom of screen
### Searches
/pattern Search forward for pattern
?pattern Search backward for pattern
n, N Repeat last search in same, opposite direction
/, ? Repeat previous search forward, backward
fx search forward for character x in current line
Fx search backward for character x in current line
tx search forward for character before x in current line
Tx search backward for character after x in current line
; Repeat previous current line search
, Repeat previous current line search in opposite direction
### Line Number
\[Ctrl]G Display current line number
n G Move to line number n
G Move to last line in file
:n move to line number n
### Marking Position
mx Mark current position as x
\`x Move cursor to x
\`\` Return to previous mark or context
'x Move to beginning of line containing mark x
'' Return to beggining of line containing previous mark
## Editing Commands
### Insert
i, a Insert text before, after cursor
I, A Insert text at beginning, end of line
o, O Open new line for text below, above cursor
### Change
r Replace with next typed characer
~ Change between uppercase and lowercase
cm Change text block defined by movement command m (e.g., cw changes next word)
cc Change current line
C Change to end of line
R Type over characters
s Delete character and continue typing
S Delete current line and continue typing
### Delete, Move
x Delete character
X Delete character to the left of the cursor
dm Delete text block defined by movement command m (e.g., dw deletes next word)
dd Delete current line
D Delete to end of line
p, P Put deleted text before, after cursor
"n p Put text from delete buffer number n after cursor (for last nine deletions)
### Yank (copy)
ym Yank (copy) text block defined by movement command m (e.g., yw yanks next word)
yy, Y Yank current line
"ayy Yank current line into named buffer a
p, P Put yanked text before, after cursor
"aP Put text from buffer a before cursor
### Other Commands
. Repeat last edit command
u Undo last edit
U Undo changes to current line
J Join two lines
\[Ctrl]L, \[Ctrl]R Redraw screen
## Invoking vi
vi file Invoke vi editor on file
vi file1 file2 Invoke vi editor on files sequentially
view file Invoke vi editor on file in read only mode
vi -R file Invoke vi editor on file in read only mode
vi -r file Recover file and recent edits after system crash
vi + file Open file at last line
vi +n file Open file at line number n
vi +/pattern file Open file at pattern
## Exit and Save Commands
ZZ Save file and quit
:x Save file and quit
:wq Save ("write") file and quit
:w Save file
:w! Save file (overriding protection)
:30,60w newfile Save lines 30 through 60 as file newfile
:30,60w>> file Append lines 30 through 60 to file file
:w %.new Save current buffer named file as file.new
:q Quit
:q! Quit, discarding any changes
Q Quit vi and invoke ex
:e file2 Edit file2 without leaving vi
:e! file2 Discard changes to current file, then edit file2 without leaving vi
:n Edit next file
:e! Discard all changes since last save
:e# Edit alternate file