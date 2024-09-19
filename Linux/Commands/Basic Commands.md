#linux #basic #commands

---
### Present Working Directory
#pwd #commandline #directory 

`pwd`

Reads out the present working directory.

#### Options

##### Logical
`-l, --logical
Use PWD from environment, even if it contains [symlinks](Files%20and%20Folders.md#Symbolic%20Links).

##### Physical
`-p, --physical
(Default) Avoid all [symlinks](Files%20and%20Folders.md#Symbolic%20Links).

---
### Change Directory
#cd #directory #directory-manipulation 

`cd [dir]`

Changes the shell working directory.

#### Returns
Returns 0 if the directory was successfully changed, non-zero otherwise.

#### Options

##### Symbolic Links
`-L
Force symbolic links to be followed.

##### Physical
`-p
Use the physical directory structure without following symbolic links, resolve symbolic links in DIR before processing instances of `[..]`.

##### Exit
`-e`
If the -P option is supplied, and the current working directory cannot be determined successfully, exit with a non-zero status.


---
### List
#ls #directory  #directory-contents 

`ls [optional dir]`

List directory contents.

#### Returns
0 if OK,
1 if minor problem (cannot access subdirectory),
2 if serious trouble (cannot access command-line argument).
#### Options

##### All
`-a, --all
Do not ignore entries starting with `[.]`.

##### Almost All
`-A, --almost-all
All command but ignore implied `[.]` and `[..]`.

##### Author
`--author
With `-l` option, read the author of each file.

##### Escapes
`-b, --escape
Print C-style escapes for non-graphic characters.
##### Long
`-l, --list
Long listing.

##### Hide
`--hide=PATTERN
Do not list entries matching shell PATTERN.

##### Human Readable
`-h, --human-readable
Lists sizes units of bytes.

##### Recursive Subdirectories
`-R, --recursive
List subdirectories recursively.

##### I Node
`-i, --inode
Print the index number of each file.



---

Make Directory

Remove

Copy

Move

Touch

Concatenate

Head

Tail

Link

Find

Change file Permission

Change file Owner

Change file group Owner

Umask

Get Regular Expression

Who Am I

Uname

