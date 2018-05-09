@title[Shell Environment and the CLI]
## Bash Shell Environment with the CLI

### Interacting with the Shell

Something clever! <!-- .element: class="fragment" -->



### more Bash verbiage, short shell examples 


---
@title[How computers organise information - file operations]

### Moving (and renaming) files 

These `header` files look like they belong in the `meta/` directory. 

Let's move them, with the `mv` **command**

```bash
[username @ hostname lfr](cdc-data)$ mv --help
Usage: mv [OPTION]... [-T] SOURCE DEST
  or:  mv [OPTION]... SOURCE... DIRECTORY
  or:  mv [OPTION]... -t DIRECTORY SOURCE...
Rename SOURCE to DEST, or move SOURCE(s) to DIRECTORY.
```

What does this mean?

---
@title[How computers represent information - file operations]

### Moving (and renaming) files

Functionally, `mv` can either:
  - **relocate** one or more files to a _directory_
  - **rename** only one file at a time 
  
Note:
Renaming is moving one file to another file 
`mv` accepts absolute and relative paths 
  
---
@title[How computers represent information -- mv]

To **move** (relocate) files with the `mv` command: 
  - the last argument (the target) must be a _directory_ (not a file) 

Let's try..









---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  move header files</span></p>

## Exercise:  move header files 

We can TAB-complete filesystem names OR use globbing 

```bash
[username @ hostname lfr](cdc-data)$ mv header*
[username @ hostname lfr](cdc-data)$ ls
data_groups/       ftables/              meta/
move.source        rename.source 
```

The header files no longer appear in the current directory listing.  

Note:
Running `ls` after filesystem operations is a good habit to develop 

How did the asterisk work? 


+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  confirm move operation</span></p>

Let's check the folder we moved them to: 

```bash
[username @ hostname lfr](cdc-data)$ ls meta/
...
header.list      header_col_names.tab
```

[comment]: # (exercise slide)

Note:
<-----------------EXERCISE---------------------------------------------------->




---
@title[How computers represent information - file operations]

## Renaming files (with move) 

What would happen if the last `mv` argument is **not** a directory?
> let's look at `mv --help` again

```bash
$ mv --help
Usage: mv [OPTION]... [-T] SOURCE DEST
  or:  mv [OPTION]... SOURCE... DIRECTORY
  or:  mv [OPTION]... -t DIRECTORY SOURCE...
Rename SOURCE to DEST, or move SOURCE(s) to DIRECTORY.
```
---
@title[How computers represent information - file operations]

`mv` will **rename** the _source_ file to the _destination_ name 

Note:
When `mv` has only 1 _source_ (and the last argument is **not** a directory), 
the last argument is the _destination_ (top usage) 









---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  rename with mv</span></p>

the `-v` option (verbose) confirms operations 

```bash
[username @ hostname lfr](cdc-data)$ mv -v rename.source to.dest 
'rename.source' -> 'to.dest'
[username @ hostname lfr](cdc-data)$ ls 
..
to.dest
```

Note:
<-----------------EXERCISE---------------------------------------------------->


---
@title[How computers represent information - file operations]

When `mv` has more than 1 _source_ (and the last argument is **not** a directory)

`mv` will **do nothing** to the _source_ arguments (and produce an error)

> Specifying more than one file, or one directory, as _source_ will produce different errors.

---








---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  mv errors</span></p>

```bash
[username @ hostname lfr](cdc-data)$ mv meta/ to.dest
mv: cannot overwrite non-directory 'to.dest' with directory 'meta/'

[username @ hostname lfr](cdc-data)$ mv meta/ move.me to.dest
mv: target 'to.dest' is not a directory
```

Note:
Similar to the globbing asterisk `*`, Bash expands _directories_ like `meta/` into their contents (multiple files).

`mv` cannot relocate multiple _sources_ to an individual file _destination_ 


+++---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  examine mv target</span></p>

```bash
[username @ hostname lfr](cdc-data)$ file to.dest
to.dest: ASCII text
[username @ hostname lfr](cdc-data)$ cat to.dest
A file to be renamed 
```

Note:
<-----------------EXERCISE---------------------------------------------------->




---
@title[How computers organise information]

### File Operation Permanence Reminder

**File operations** performed by Shells like Bash are ***permanent*** 

Robot Kitchen CLIs don't have "Recycle" or "Trash" bins.

When the Shell moves an item off a shelf,  
**THAT ITEM IS GONE FROM THAT SHELF** 

...and hopefully _on_ your target shelf







---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  mkdir</span></p>

```bash
[username @ hostname lfr](master)$ cd ~
[username @ hostname ~] $ mkdir menu; ls -1
..
menu
..

```

Note:
`;` **special character** End Of Line, to put two commands on one line 
`ls -1` to show results in one column 

We'll use this `menu` shelf in later Bash exercises.

<-----------------EXERCISE---------------------------------------------------->










+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Filesystem Operations</span></p>

- `mkdir` make one or more directories 
  - `mkdir -p dir1/dir2/dir3` make all ancestors, as needed 
- `rmdir` remove one or more directories (if empty) 
  - `rmdir -p dir1/dir2/dir3` remove all ancestors (if empty) 
- `mv` relocate file(s); rename 1 file
- `rm` remove file(s) only, not directories
  - `rm -r <directory>` recursively remove all files _and parent directory_ 
- `cp` copy file(s) without renaming; copy 1 file & rename the copy 

Note:
<-----------------DEFINITIONS------------------------------------------------->







---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git add & commit</span></p>

```bash
[username @ hostname lfr](cdc-data)$ git status
..
..
..
..
..


```


---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git add & commit</span></p>

```bash
[username @ hostname lfr](cdc-data)$ git add .
..
..
..
..
..


```



Note:
<-----------------EXERCISE---------------------------------------------------->





### git add, commit -m ""




What about creating files? 


@title[How programs can be used together]

### Creating text files with redirection 

Bash's `>` **operator** redirects _outputs_ to a file 

- We can use it to create an empty file, by redirecting an empty stream. 
- Using `echo`, we can redirect specific text. 
- And using `cat`, we can redirect (output from) a live stream.

Note:
`>` right angle bracket, "greater-than" sign 






---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  redirection file creation</span></p>

```bash
[username @ hostname ~]$ > myemptyfile.txt
[username @ hostname ~]$ echo "A short note" > mynote.txt
```
+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  redirection file creation</span></p>

```bash
[username @ hostname ~]$ cat > mylongnote.txt 
A long note [ENTER]
This input stream will be redirected into mylongnote.txt [ENTER]
when we terminate the process with CTRL-C [ENTER]
[CTRL-C]
[username @ hostname ~]$ ls my*
myemptyfile.txt     mylongnote.txt    mynote.txt 
```
Note:
`ls my*` using the asterisk wildcard 

<-----------------EXERCISE---------------------------------------------------->






+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">IO Redirection Operators</span></p>

- `>` redirect _output_ to a **file** (overwrite) 
  - `2>` redirect _error_ to a **file** (overwrite) 
  - `>>` redirect _output_ (append) 
  - `2>>` redirect _error_ (append) 
- `|` pass _output_ of a command as _input_ to another command 
- `<` redirect standard input _from a file_ 

Note:
Recall in IO, the default output is 1 **stdout**
If we want to redirect **stderr**, specify 2 before the `>` operator

  - `2>&1 |` redirect _error_ to _output_, then pass as _input_ to another command 

<-----------------DEFINITIONS------------------------------------------------->
 
 
 
 
 
 

### nano text editor lessons here?? 




 
 
 
---
@title[Bash's environment]

How does Bash find all these recipes? 

- When we make orders, Bash looks on specific pantry shelves for our recipes. 







---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  locate menu items</span></p>

## Exercise:  locate menu items 

```bash
[username @ hostname ~]$ which pwd
/usr/bin/pwd
```
- **which** shows the recipe location for a menu item
- (the _program file_ for a _command_) 
- **whereis** shows the program & manual file (Linux & Mac only)

Note:
<-----------------EXERCISE---------------------------------------------------->



---
@title[Bash's environment -- notebook]

### Bash's Notebook 

- How does Bash keep track of this menu? 
  - with a personal notebook!

@fa[arrow-down]
  
+++
@title[Bash's environment -- notes]

### Bash's Notebook -- the Variables 

- When we hail Waiters, they bring a notebook & some notes
- Notes keep track of our kitchen preferences.
- _Key notes_ can be marked, to copy into all shell notebooks

--- 
@title[Bash's environment]

### Environment Variables & Shell Variables

- Shells (like Bash) keep track of settings & preferences using variables
- System-defined variables are typically named in ALL CAPS
- **Environment Variables** are copied to programs and subshells
- _Shell Variables_ are valid only in the current shell (not copied to subshells)

_Shell Variables_ can be **exported** into Environment Variables  









---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  environment variables</span></p>

### Look at Bash's Key notes 

```bash
[username @ hostname ~]$ printenv 
HOSTNAME=localhost.localdomain
TERM=xterm-256color
SHELL=/bin/bash
HISTSIZE=1000
```

Note:
That's a lot!  Let's page through them with `less` 

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  environment variables</span></p>

```bash
$ printenv | less 

[ENTER or j, k] to scroll by line forward, backward

[f, b] to scroll by page forward, backward

[g, G] jump to start, end (of file) 

[h] summary of less commands 

[q] to quit pagers 
```

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  environment variables</span></p>

```bash
$ printenv SHELL 
/usr/bin/bash
$ printenv USER HOME HISTFILE
username
/home/username 

```

No results for HISTFILE.  It might not be an "environment" variable. 

Note:
<-----------------EXERCISE---------------------------------------------------->


---
@title[Bash's environment -- history]

Recall that we can cycle through our most recent orders using the arrow keys.

- Our order history must be somewhere in the pantry
- `printenv` only prints Bash's _Key notes_ 

Note:
How else can we print a note?

---
@title[Bash's environment]

### Shell Variables

We can use the `echo` command to print the value of _any_ variable, including Bash's personal notes: 

```bash
$ echo $SHELL
/bin/bash
$ echo $HISTFILE 
/home/username/.bash_history 
```

The `$` special character tells Bash to use the _contents_ of the variable. 

Note:
`echo` accepts a variety of inputs; use `$` to tell echo we want _contents_ 
`printenv` only accepts variable names, so it already knows we want _contents_ 

---
@title[Bash's environment -- environment variables]

### Environment Variables
#### Key notes, all shells (and subshells) get copies

- $SHELL -– the current shell (absolute path to Bash recipe)
- $USER -– your username
- $HOME –- absolute path to your home pantry shelf
- $HOSTNAME -– the Robot Kitchen you are in
- $PATH –- Bash's kitchen menu

`printenv SHELL` or `echo $SHELL` 

---
@title[Bash's environment -- shell variables]

### Shell Variables
#### personal notes, only this shell has a copy

- $HISTFILE -- the location of your Bash command history file
  - only interactive Bash shells add to your order history
  - ..therefore only interactive Bash shells have this note
- $BASH -- the location of this Bash's recipe
- $DIRSTACK -- the list of directories used by dirs, pushd, and popd
- $PPID -- the process ID of this Bash

`echo $HISTFILE` only 

---
@title[Bash's environment -- IFS]

### IFS Shell Variable 
#### Internal Field Separator

- character(s) used as delimeters (for word separation)
- default is the 3 "whitespace" chars: 
  - `<space><tab><newline>` 

Use `echo` & `cat`, or `printf`, to view 

@fa[arrow-down]

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  IFS shell variable</span></p>

```bash
$ echo -n "$IFS" | cat -vte
 ^I$
```
- `-n` remove `echo`'s newline (before piping to `cat`)
- `-vte` 
  - show non-printing chars (space) 
  - show `^I` for tabs
  - show `$` for end of line 

```bash
$ printf %q "$IFS"
$' \t\n'
```
- `%q` print in POSIX $'' syntax 


Note:

<-----------------EXERCISE---------------------------------------------------->



---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - Shell Environment</span></p>

- **Environment Variable** -- 
- **Shell Variable** -- 
- `export MYVAR` -- make shell var _MYVAR_ an **Environment Variable** (send a copy to all subshells)
  - `export -p` -- print list of global variables 
- `printenv` -- 
- `echo $VARIABLE` -- 

- `$` -- special character, "value/contents of" 

Note:
<-----------------DEFINITIONS------------------------------------------------->












---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  conga Bash</span></p>

We can hail another Waiter to stand in front of Bash.
- each Bash will queue up
- often, we will only "see" the newest one 

```bash
$ bash

$
```

**Environment Variables** to the rescue! 

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  conga Bash</span></p>

How can we tell where we are in the Bash line? 
with **SHLVL**

```bash
$ printenv SHLVL
2

$ exit [or CTRL-D]

$ printenv SHLVL
1
```

Note:
The topmost shell level may start at 2, depending on your system. 

[comment]: # (exercise slide)

<-----------------EXERCISE---------------------------------------------------->




---
@title[Bash's environment -- command execution]

### Command Execution 

When Bash processes orders, Robot Kitchen executes `fork` & `exec` system calls.

- `fork` starts a new process, by copying the current one
- `exec` replaces old process contents with new process contents 

During **command execution**, our Bash Copy is replaced by the _contents_ of the command's **program file**.

For subshells (_Conga Bash_), our Bash Copy is replaced by a new Waiter Bash (with a clean personal notebook).

Note:
Recall that all Bash shells receive copies of Bash **Key notes** (environment variables) for their notebooks 

---
@title[Bash's environment -- shell variables]

We can ask Bash to keep any note (as a _shell variable_):

```bash
$ MYNOTE="this is my note"
$ echo $MYNOTE
this is my note

$ printenv MYNOTE

```

No results from `printenv` indicate MYNOTE is not a Key note (environment variable).   

---
@title[Bash's environment -- exporting]

To make MYNOTE a Key note (**Environment Variable**), we can `export` it:

```bash
$ export MYNOTE
$ printenv MYNOTE
this is my note
```

Now `printenv` knows about this note, and subshells will get a copy. 

---
@title[Bash's environment -- copying]

**Reminder** 

Shell & Environment Variables are not shared.

If you change the value of MYNOTE, `export` it again to copy the new value to subshells. 


---
@title[Bash's environment -- menu]

### Bash's Menu 

We can check all menu recipes with `which -a`:

```bash
$ which -a ls
/usr/bin/ls
/bin/ls
/usr/bin/ls
```
In Bash's menu, the `/usr/bin/ls` shelf comes first. 

---
@title[Bash's environment -- menu]

### Bash's Menu -- PATH Key note 

A colon-separated (:) list of pantry shelves, searched in-order for commands 






---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  show menu/span></p>

```bash
$ printenv PATH
/usr/local/bin:/usr/local/sbin:/usr/bin:/usr/sbin:/bin:/sbin:/home/kalan/.local/bin:/home/kalan/bin

$ which ls
/usr/bin/ls
```

Note:
<-----------------EXERCISE---------------------------------------------------->


---
@title[Bash's environment  -- menu]

When we check which recipe an order will use, Bash:
- looks in the $PATH note for a list of pantry shelves
- checks each shelf in order for a matching recipe
- prints the absolute path of the first matching recipe


---
@title[Bash's environment  -- menu]

What if we have a recipe somewhere else in the pantry?
- We can modify Bash's PATH note, with our own menu 


---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  update menu</span></p>

```bash
$ export PATH=$PATH:$HOME/menu
```

Here, we set (and export) the PATH key note to:
- `$PATH` (the previous _contents_ of the PATH key note)
- `:` (the list separator)
- `$HOME/menu` (the shelf with our recipe)



Note:
If you don't have `menu`, make one with `mkdir`:

```bash
$ cd ~
$ mkdir menu
$ export PATH=$PATH:$HOME/menu
```

<-----------------EXERCISE---------------------------------------------------->



### shell param exercise examples 
```
$_
$!
$1, $2
$#
$?
```


### parameter expansion 
```
${!My*}
```


### BASH alias with Nano 

$ vi .bash_profile
..
alias lsl='ls -lh'


### dotfiles & profile order & interactive 



+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Process Control</span></p>

- `CTRL-Z` suspend current process 
- `jobs -l` list active jobs & PIDs 
- `bg` put suspended process in background 
  - `bg %1` put first process in bg
  - `bg %cat` put `cat` process in bg 
- `fg` bring suspended process to foreground 
  - `fg %1` bring first process to fg 
  - `fg %cat` bring `cat` process to fg 
- `kill PID` ask PID process to terminate itself 
  - `kill -9 PID` terminate PID process 

Note:
<-----------------DEFINITIONS------------------------------------------------->





+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Special Parameters</span></p>

- `echo $$` PID of current shell 
- `echo $-` options set for current shell (`i` for interactive) 
- `echo $0` shell script name
- `echo $!` PID of last bg process
- `echo $?` last fg exit status 
(0 is nice) 
(useful for arithmetic & expansion tests) 

+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Special Parameters</span></p>

- `echo $@` all parameters, individually 
- `echo $*` all parameters, together separated by IFS char 
- `echo $1` first argument from last command 
- `echo $_` last argument, or last command if no arguments
- `echo $#` argument/parameter count from last command


+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Metacharacters & Substitutions</span></p>

- `~` home
- `*` file substitution; zero or more characters
- `?` file substitution; one character
- `[ ]` file substitution; any character between brackets

- `$(cmd)` command substitution with expansion & parentheses 
- `` `cmd` `` command substitution with backticks

+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Metacharacters & Substitutions</span></p>

- `;`	Command sequence, Sequences of Commands
- `||`	OR conditional execution
- `&&`	AND conditional execution
- `( )`	Group commands, Sequences of Commands
- `&`	Run command in the background, Background Processes
- `#`	Comment


+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Metacharacters & Substitutions</span></p>

- `$`	Expand the value of a variable
- ` \ `	Prevent or escape interpretation of the next character

- `' '`   Single-quotes, for literal characters & escape expansion ` \ ` (backslash)
- `" "`   Double-quotes, to expand `\`, `$`, and `` ` `` (backtick)


Note:

Escape the metacharacter with a backslash ` \ ` . Escaping characters can be inconvenient to use when the command line contains several metacharacters that need to be escaped.

Use single quotes `' '` around a string. Single quotes protect all characters except the backslash `\`.

Use double quotes `" "`. Double quotes protect all characters except the backslash `\`, dollar sign `$` and grave accent `` ` ``.

Double quotes is often the easiest to use because we often want environment variables to be expanded.

<-----------------DEFINITIONS------------------------------------------------->





