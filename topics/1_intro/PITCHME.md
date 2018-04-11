@title[Computers and the CLI]
## Computers and the CLI 

### Interacting with operating systems 

Who needs a mouse when we have keys! <!-- .element: class="fragment" -->

---
@title[Introduction]
<p><span class="slide-title">Introduction</span></p>

To begin, double-click a web browser (GitBash, Terminal) icon...  <!-- .element: class="fragment" -->
with your mouse <!-- .element: class="fragment" -->

@fa[arrow-down]

+++?image=assets/bg_images/green_moon.jpg
@title[Introduction - Learning Objectives]
<p><span class="slide-title">Learning Objectives</span></p>

- Understand how computers represent information |
- Understand how to interact with the computer using commands |
- Understand how to organise your digital work in directories |

@fa[arrow-down]

+++?image=assets/bg_images/green_moon.jpg&color=orange
@title[Introduction - Assumptions]
<p><span class="slide-title">Assumptions</span></p>

- Laptop computer with internet access
- Familiarity with GUIs (Windows, Mac OS)
- Terminal emulator program installed 
  - Terminal on Mac OS
  - GitBash on Windows
- Git program installed (by default on most Macs, comes with GitBash for Windows)

  
[comment]: # (the image color directive does nothing here - the slide bg image is 1x1px and fills the frame)  
  
+++?image=assets/bg_images/green_moon.jpg
@title[Introduction - Interfaces]
<p><span class="slide-title">Interfaces</span></p>

- GUI - graphical user interface
  - "windows" of work            <!-- .element: class="fragment" -->
  - mouse input                  <!-- .element: class="fragment" -->
  - user-friendly & wide-angle   <!-- .element: class="fragment" -->

- CLI - command-line interface
  - "lines" of work              <!-- .element: class="fragment" -->
  - keyboard input               <!-- .element: class="fragment" -->
  - efficient & myopic           <!-- .element: class="fragment" -->

[comment]: # (this slide seems to fit vertically - 12 H including Title and Breaks)  

---
@title[Computer Intro - Components] 
<p><span class="slide-title">Computer Components</span></p>

- Computers have hardware & software:
![computer hw sw](assets/path.jpg)


+++
@title[Computer Intro - Features]
<p><span class="slide-title">Computer Features</span></p>

- They receive **input** & produce **output**:
![terminal IO kb chart](assets/path.jpg)

+++
@title[Computer Intro - Purpose]
<p><span class="slide-title">Computer Purpose</span></p>

Computers are built to help _process information_.  
They only dish out what we _instruct_ them to.  

@fa[arrow-down]

+++
@title[Computer Intro - Abilities]
<p><span class="slide-title">Computer Abilities</span></p>

- Computers: 
  - accept instructions |
  - store & access information |
  - perform calculations & tasks |
  
That's it.  <!-- .element: class="fragment" -->

+++
@title[Computer Intro - Information] 
<p><span class="slide-title">How computers represent information</span></p>

- To a computer, all information is either:
  - a **file** (stored data, static) |
  - a **process** (active instructions, dynamic) |

Note:
"Folders" are also files (more on this later)
  
+++
@title[Computer Intro - Instructions] 
<p><span class="slide-title">How computers process information</span></p>

- **Files** just sit there |
- **Processes** do all the work |
  - "follow orders" | 
  - accept _input_ 
  - provide _output_ | 

+++
@title[Computer Intro - Orders]
<p><span class="slide-title">How computers take orders</span></p>

- Input can be: |
  - "stuff we're typing right now" (live stream) |
  - "stuff we typed a while ago" (a file) |

> How do we give them orders?   <!-- .element: class="fragment" -->

@fa[arrow-down]

+++
@title[Computer Intro - Input, live]
<p><span class="slide-title">Computer Input - live</span></p>

> live input:  typing, mousing 
> ![keyboard, mouse](assets/path.jpg)

@fa[arrow-down]

+++
@title[Computer Intro - Input, stored]
<p><span class="slide-title">Computer Input - stored</span></p>

> stored input:  finding files on a disc 
> ![files](assets/path.jpg)

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
@title[Exercise:  Open a web browser]
## Exercise:  Open a web browser 
### using live & stored inputs 

- mouse to a shortcut icon & click it (live) 
- activate a browser program (stored) 
- launch a web browser process (live) 

@fa[arrow-down]
<----------------------------------------------------------------------------->

+++
@title[Orders:  Behind the scenes]

### GUI orders, behind the scenes:

- "Open a web browser"
  - Navigation (IO):  mouse to icon |
  - Order (input):  mouse click |
  - Recipe (IO):  web browser program |
  - Dish (output):  web browser page | 

+++
@title[Computer Intro - Processing]

### Computer Information Processing

- How did we **really** tell the computer to _process_ our inputs? |
  - with _special directives_ called **commands** |
  
> commands are like **orders** for a computer 

+++ 
@title[Computer Intro - Programs]

- How _does_ the computer process our information? |
  - by following _special instructions_ called **programs** |
  
> programs are like **recipes** for a computer  

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
@title[Exercise:  make an order ]
## Exercise:  make an order, GUI
### Visit the GitHub website:

  - open a new tab 
  - visit seminar GitHub 
  - look at some files 
  - (log in, if you have an account)

@fa[arrow-down]
<----------------------------------------------------------------------------->

+++
@title[Orders:  Behind the scenes]

### GUI orders, behind the scenes:

- "Visit a website & log in" |
  - Navigation (IO):  mouse to address bar, login fields |
  - Orders (input):  keyboard & mouse clicks |
  - Recipes (IO):  browser tab program, send text to internet |
  - Dish (output):  display website, display results |

---
@title[Robot Kitchen to the rescue]

How do **orders** & **recipes** help us _understand_ computers?

Let's dig in with a metaphor!
![kitchen, chef images](assets/path.jpg)

@fa[arrow-right]

---
@title[Robot Kitchen]

## Robot Kitchen

Computers are like commercial kitchens:
- full of machinery & instructions
- need "guidance" (staff, recipes, orders)

![more kitchen & computer images](assets/path.jpg)
![including a pantry](assets/path.jpg)

@fa[arrow-down]

[comment]: # (Robots from Dubstep Dispute)

+++
@title[Robot Kitchen]

- What do commercial kitchens & staff do?
  - facilitate food processing & service (fill **orders**) |

- How?  In these 2 ways: |
  - _store_ ingredients & **recipes** |
  - _follow_ recipes |

This should be familiar... <!-- .element: class="fragment" -->

+++
@title[Kitchens & Computers]

### Kitchens & Computers 

- Robot Kitchens:
  - _take_ **orders** |
  - _store_ ingredients & **recipes** |
  - _follow_ recipes |

@fa[arrow-down]  
  
+++  
@title[Kitchens & Computers]

- Computers: 
  - _accept_ **commands** |
  - _store_ & access data (including **programs**) |
  - _perform_ calculations & tasks (run programs) |

@fa[arrow-down]    
  
+++
@title[Robot Kitchen]

- Like kitchen equipment, computer equipment: 
  - only does what **ordered** to do 
  - by following special instructions 

Special files called **program files** contain these instructions for the computer:
![bin or exe images, MS Office icons](assets/path.jpg)

@fa[arrow-down]

+++

For example, a stand mixer...

@fa[arrow-down]

+++
@title[Robot Kitchen Equipment]

## Robot Kitchen Equipment

Robot Kitchen's Stand Mixer:
![stand mixer](assets/path.jpg)

> Until a robot chef pushes some buttons, it doesn't do anything  
> 
> If Robot Chef pushes the _wrong_ buttons, the mixer might ruin your order


---
@title[Robot Kitchen Equipment]

Let's push some (GUI) buttons!

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
@title[Exercise:  recipes)]

## Exercise:  "recipes"

- in GitHub online, look at (stored) **pie.sh** recipe 
  - format:  stored (file on disc) |
  - language:  Bash (sh) |
  - type:  interpreted |
- With your hands, use your (active) **mouse** process 
  - format:  live (user input, active instructions) |
  - language:  your OS suite (likely C) |
  - type:  compiled |

<-----------------EXERCISE---------------------------------------------------->

+++
@title[How computers follow recipes]

## Programs (recipes)  

- In general, recipes can be:
  - live or stored ![input devices, commands](assets/path.jpg)
  - yours or someone else's ![mouse clicks, OS](assets/path.jpg)
  - direct or indirect ![in machine language, needs interpretation](assets/path.jpg)

@fa[arrow-down]

Note:
Live instructions

+++
@title[How computers follow recipes]

## Interpreted recipes 

Indirect (_interpreted_):  recipes like shell scripts
- the **program file** is in "human" language
  - Robot Kitchen staff has an interpreter
  - each instruction is converted into machine language **live**
  - there is only 1 file, yay!

@fa[arrow-down]

+++
@title[How computers follow recipes]

## Compiled recipes 

Direct (_compiled_):  recipes like your web browser, C code
- the **program file** is in machine language
  - Robot Kitchen staff doesn't have an interpreter
  - all instructions must be translated into machine language first 
  - there are two files:  
  'source code' (our recipe) &  
  'compiled code' (Robot Kitchen's recipe)

@fa[arrow-right]

Note:
For 'interpreted' languages 


---
@title[How computers take orders]

### What does all this mean?  

_Everything we can do graphically, we can also do with the keyboard:_

- launch programs (web browser, MS Excel) |
- manage processes (web browser, MS Excel) |
- manage access permissions |
- manage documents (browse, move, rename) |
- search for documents |
- manipulate text in (text) documents |

![GUI drag & drop, search](assets/path.jpg)

@fa[arrow-down]

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
@title[Exercise:  hail a robot headwaiter)]

## Exercise:  hail a robot headwaiter

- launch Terminal or GitBash 
  - look at the Headwaiter's prompt 
  - (we'll come back to this in a moment) 

---?image=assets/orange_moon.jpg
@title[Exercise:  make some orders)]

## Exercise:  make some orders 
  
- send some orders to Robot Headwaiter
  - `who` is logged in 
  - `ps` _what_ else this Headwaiter is doing 
  - `pwd` _where_ you are in the kitchen pantry
  - `ls` _list_ any other items on this shelf 

@fa[arrow-down]

<-----------------EXERCISE---------------------------------------------------->
+++
@title[How computers take orders]

### Using the keyboard 

- What have we been doing? |
  - ordering items from a menu |
- What has _the computer_ been doing? |
  - finding recipes in our kitchen | 
  - processing our orders |

@fa[arrow-right]

---
@title[How computers take orders]

### Computers & Robot Kitchen 

- In computer systems,
  - **Programs** are like recipes for Robot Kitchen
  - **Operating Systems** are like chefs & kitchen staff
  - **Processes** are the recipes our chefs are making

@fa[arrow-down]

+++
@title[How computers take orders]

- When we place an order, Robot Kitchen staff:
  - check the menu
  - find recipes
  - follow them (make our orders)

+++
@title[Robot Kitchen]

- How well kitchens perform often depends on recipes
- Robot Kitchen staff know about some basic recipes
  - ![system programs image](assets/path.jpg)
- We can provide custom recipes (which we will!)
  - ![pie.sh screencap](assets/path.jpg)


<----------------------------------------------------------------------------->
<-----------------DEFINITIONS------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - Computer terms</span></p>

- **Program** -- set of instructions for a computer to follow
- **Operating System** -- programs that work together to manage computer resources

- **File** -- stored information (can be a program)
- **Process** -- active program

- _**Program File** -- special file with instructions for a computer_

<----------------------------------------------------------------------------->

---
@title[Robot Kitchen Staff]

- In Robot Kitchen, staff includes: |
  - Headwaiters to take orders 
    ![Headwaiter Shells](assets/path.jpg) |
  - Demi-chefs to use equipment & ingredients 
    ![system programs](assets/path.jpg) |
  - Head Chef to oversee demi-chefs & kitchen
    ![system programs](assets/path.jpg) |

@fa[arrow-down]

+++
@title[Robot Kitchen Staff]

- Why must we staff Robot Kitchens, anyway? 
  - Equipment may be shared |
  - Instructions may be in shorthand |
  - Others may be placing orders |

Like our browser recipe from earlier...

@fa[arrow-right]

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
@title[Exercise:  GUI orders, browser recipe]

## Exercise:  GUI orders, browser recipe   

- tab or mouse back to browser window 
- order another tab or window (process) 
  - mouse the + icon
  - or `CTRL-T` keyboard

What follows your orders?
> the active browser process 

@fa[arrow-down]

<-----------------EXERCISE---------------------------------------------------->
+++
@title[Robot Kitchen Staff]

### Robot Kitchen staff monitor your active recipes: 

- web browser & tabs |
- Terminal emulator & commands |
- any Office programs you may have open |

@fa[arrow-down]

+++
@title[Robot Kitchen Staff]

### Robot Kitchen staff know about: 

- your recipes |
- kitchen equipment being used |
- time spent on each piece of equipment |

@fa[arrow-right]

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
@title[Exercise:  make an order)]

## Exercise:  use a Headwaiter to check google.com  

- Tab into Terminal or GitBash
- make a `ping` order: 
  - `ping google.com` to check if Headwaiter Shell can reach Google 
  - `CTRL-C` (Windows & Linux) or `CMD-C` (Mac) to quit active process 

---?image=assets/orange_moon.jpg
@title[Exercise:  time an order)]

## Exercise:  use a Headwaiter to time an order   

- `time` your `ping` order:
  - `time ping google.com` 
  - `CTRL-C` or `CMD-C` to quit active process
- examine _real_, _user_ (CPU), and _sys_ (CPU) time values 

What keeps track of this information?
  
@fa[arrow-right]
<-----------------EXERCISE---------------------------------------------------->

---
@title[How computers follow recipes]

### Computer System staff 

- For computers, we have:
  - **Operating Systems!**

- Headwaiter **Shells** take orders |
- **System Programs** use equipment & ingredients |
- Head Chef **Kernel** oversees programs & kitchen use |


<----------------------------------------------------------------------------->
<-----------------DEFINITIONS------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Operating System Components</span></p>

## OS Components - Kernel 

- **Kernel**
  - core component of an operating system
  - responsible for resource management & program execution

+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Operating System Components</span></p>
## OS Components - Shell 
  
- **Shell**
  - interfaces with the **kernel**
  - interprets user commands

+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Operating System Components</span></p>
## OS Components - System Programs 

- **System Programs**
  - implement most OS functions, like: 
  - input devices |
  - user environments |
  - schedulers |

<----------------------------------------------------------------------------->

---
@title[Robot Kitchen Staff]

### Robot Kitchen Staff 

- During kitchen prep, staff:
  - check the pantry |
  - read recipes | 
  - follow instructions | 
- Once the kitchen opens, staff: |
  - take & process orders | 

@fa[arrow-down]

+++

### Chef Kernel (the manager):  

- knows the equipment in our kitchen (from mixing bowls to stove tops) and how to use it |
- speaks low-level languages like machine code (binary) and assembly (symbolic binary) |
- does not speak high-level languages (requires an interpreter) |

@fa[arrow-down]

+++

### Headwaiter Shells (the interpreters):

- check that your items are on the Robot Kitchen menu |
- tell Chef Kernel about your order |
- speak some high-level languages |
- speak enough assembly to interpret for Chef Kernel | 

@fa[arrow-down]

+++ 

### Demi-chefs (the helpers):  

- receive tasks from Chef Kernel |
- use kitchen equipment |
- sort the pantry ingredients | 

---
@title[How computers take orders]
 
When your order comes in from Headwaiter Shell, Chef Kernel delegates some work to the saucier & patissier demi-chefs

- What if pie isn't on your Robot Kitchen menu?
  - We'll need to provide a recipe

- How?
> First, we add a pie recipe to our pantry 

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  Download files, GUI</span></p>

## Exercise:  Download files, GUI

- Tab back to web browser 
- Get pie recipe from a web browser:
  - From GitHub 
  - Download `pie.sh`

@fa[arrow-down]
<----------------------------------------------------------------------------->

+++
@title[How computers take orders]
How computers take orders

- What happened behind the web browser scenes? 
  - some **orders** & **recipes** 

@fa[arrow-down]

+++
@title[How computers take orders]
<p><span class="menu-title slide-title">How computers take orders GUI delivery</span></p>

## Third-party GUI delivery service

- We _order_ the browser (with our mouse) to fetch a file 
- The browser _orders_ menu item X from the kitchen staff:
  - "download web data into my pantry"
- Kitchen staff finds & follows _recipes_ to get `pie.sh`:
  - get contents from web
  - save in my pantry (as an item, on a shelf)

@fa[arrow-down]

+++
@title[How computers represent information]

- Kitchen staff notifies the browser when finished downloading 
- Browser GUI notifies us:
>`pie.sh` is now in your pantry!

@fa[arrow-down]

+++
@title[How computers organise information]

- Where did our file go?
> _onto a shelf_ (in the pantry) 

@fa[arrow-right]

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  GUI, find pie.sh</span></p>

## Exercise:  GUI, find pie.sh

- open GUI pantry doors:  `Finder` on Mac, `Explorer` on Windows
- mouse navigate, probably to your `Downloads` shelf 
- find `pie.sh` file 

@fa[arrow-down]
<----------------------------------------------------------------------------->

---
@title[How computers represent information]

### How computers represent information 

- Files (like recipes) live in non-volatile storage, like hard discs
  - ![hard disc/drive](assets/path.jpg)
  - stored data |
  - "long-term" memory |
  - persist through power loss |

How do computers keep track of this data?

---
@title[How computers represent information]

- Computers parallel paper filing systems: 
  - recipes & notes, kept in folders, kept in drawers or on shelves
  - ![pantry, discs](assets/path.jpg) |
  - hands, to sort & hold notes |
  - ![hands, RAM](assets/path.jpg) |

@fa[arrow-down]
  
+++
@title[How computers represent information]

  - calculators, scales, & measuring equipment 
  - ![CPU, cale, tablespoons](assets/path.jpg) |
  - instructions & manuals |
  - ![software, stand mixer manual](assets/path.jpg) |

@fa[arrow-right]
  
---
@title[How computers represent information] 

- How does Robot Kitchen organise ingredients in the pantry? 
  - with shelves, or **directory trees** |

@fa[arrow-right]
  
+++
@title[How computers represent information]

- Each pantry is logically organised into shelf-like hierarchies called directories (or folders) 
- Shelves can be nested (have more shelves) |
  - ![pantry with items](assets/path.jpg) |
  - ![put mini-shelves on a shelf](assets/path.jpg) | 

---
@title[How computers take orders]

- If we know what items we want in our pantry, 
  - _we can skip_ "GUI delivery services" like web browsers 

- For more power & control, 
  - order from Robot Kitchen staff |
  - ...using the _keyboard_! |

@fa[arrow-down] 
  
+++
@title[How computers take orders]

Reminder:  we can't communicate directly with Chef Kernel 

We'll need to ask Headwaiter Shell:  <!-- .element: class="fragment" -->
![chef, waiter, restaurant table, patron](assets/path.jpg) 

@fa[arrow-down]

+++
@title[How computers take orders]

- How do we ask a Headwaiter for a menu item?
  - type **commands** into a **shell** |
  
recall our `who, ls, pwd` from earlier...


<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  Headwaiter Shell's (interactive) prompt</span></p>

## Exercise:  Headwaiter Shell's (interactive) prompt

- tab to GitBash / Terminal (Interactive Shell)
- examine your shell prompt (Bash) 

```bash
[username @ hostname ~]$ 
```

@fa[arrow-down]

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  Headwaiter Shell's prompt</span></p>

## Exercise:  Headwaiter Shell's prompt

- **Interactive** shells "wait" for your keyboard input 
- interactive prompts typically show:
  - who you are (_username_) 
  - what kitchen you're at (_hostname_) 
  - where you're looking in the pantry (_directory_) 

<----------------------------------------------------------------------------->


<----------------------------------------------------------------------------->
<-----------------DEFINITIONS------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">CLI Components</span></p>

## CLI Components 

- **Terminal emulator** (GitBash, Terminal) 
  - keyboard input & screen output
  - an interface between you and the Shell 
- **Shell** (Bash)
  - command-line interpreter
  - an interface between your commands and the Operating System
- **Command**
  - keyword for the computer
  - represents an executable set of instructions
  
<----------------------------------------------------------------------------->
---
@title[How computers take orders]

- Unlike files which live on hard discs, 

- **Processes** (like our Bash window) live in volatile storage like RAM
  - ![RAM](assets/path.jpg)
  - active instructions
  - "short-term" memory
  - only exist while the computer is on

---
@title[How computers take orders]

- The Bash processes' instructions are: 
> Check for orders 
> (from us, the user)

Let's order an appetizer!

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  order from Headwaiter Bash</span></p>

## Exercise:  date command  

```bash
[username @ hostname ~]$ date
Wed Mar 14 11:50:33 EDT 2018
```
  - the `date` **command** tells Bash we want some date information 
  - the **process** outputs this information (usually to the screen) 

<----------------------------------------------------------------------------->

+++
@title[How computers represent information] 

### Order a meal...

- Let's download pie.sh to the pantry using a **command**
  - many recipes can get information from the internet 
  - we want to use a `git` recipe 
  - we'll use a `git` **command** to tell Bash 
  
First, make sure we're home:
```bash
[username @ hostname ~]$ cd ~
[username @ hostname ~]$ 
```

Note:
Bash tilde shortcut for home 


<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git the meal (workshop files)</span></p>
### order from Headwaiter Bash

- ask the Headwaiter what shelf we're on (should be home) 
- order a `git` recipe  
- `git clone` downloads the contents of a remote repository 

```bash
[username @ hostname ~]$ pwd 
/home/username
[username @ hostname ~]$ git clone https://github.com/ccs-training/linux-for-research.git
```

---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  list git repo ingredients</span></p>

```bash
[username @ hostname ~]$ ls
..
linux-for-research
..
[username @ hostname ~]$ ls linux-for-research
..
pie.sh
..
```
- our new git shelf has some ingredients, including `pie.sh`!

<----------------------------------------------------------------------------->

---
@title[How computers organise information]

## How did Headwaiter Bash find our `git clone` and `ls` commands?

- Each shell has a special _menu_
- we can use the **which** command to locate other commands 

@fa[arrow-right] 

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  locate menu items</span></p>

## Exercise:  locate menu items (commands)

```bash
[username @ hostname ~]$ which pwd
/usr/bin/pwd
```
- **which** shows the recipe location for a menu item
- (the _program file_ for a _command_) 
- **whereis** shows the program & manual file (Linux & Mac only)

<----------------------------------------------------------------------------->


---
@title[How computers organise information]

## How does Robot Kitchen track & sort ingredients?

Similar to Bash's order menu: 

- Each pantry has a **master list** of ingredients, and which shelves they're on
- ![spreadsheet](assets/path.jpg)

+++
@title[How computers organise information]

```bash
[username @ hostname ~]$ which ls
/usr/bin/ls
```

- **ls** is the ingredient |
- **/usr/bin** is the shelf's address |
- **/usr/bin/ls** is the **absolute path** to the recipe |

---
@title[How computers organise information]

### Locating items in a computer pantry 

...is like driving a postal route:  
![map, route](assets/path.jpg)  

- start at the post office (pantry root `/`) |
- follow a path of roads to your street (shelves `/home/me`) |
- open your mailbox (your item `/home/me/myfile.txt`) |
- ![GUI directory tree](assets/path.jpg)

---
@title[How computers organise information]

### File system hierarchy 

![Linux & Windows](assets/path.jpg)

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  find Bash's recipe shelf</span></p>

### Exercise:  find Bash's recipe shelf

```bash
[username @ hostname ~]$ which bash
/usr/bin/bash
```
<----------------------------------------------------------------------------->


<----------------------------------------------------------------------------->
<-----------------DEFINITIONS------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">File System Definitions</span></p>

### File System definitions  

- **File system** (logical) -- hierarchy of directories
- **Directory** (folder) -- collection of files
- **Path** -- location of file(s)
  - **Absolute path** -- route, starting from the post office (root)
  - also _**full path**, **complete path**_
  - **Relative path** -- route, starting from some other shelf in the pantry 

<----------------------------------------------------------------------------->
---
@title[How computers organise information]

### Navigating a pantry 

Let's look on our git shelf,  
with assistance from Headwaiter Bash 

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  navigate to git shelf</span></p>

## Exercise:  navigate to `git` shelf

```bash
[username @ hostname ~]$ cd linux-for-research
[username @ hostname lfr](master)$ ls -l 
..
```
<----------------------------------------------------------------------------->
---
@title[How computers represent information]

### Bash shell prompt with `git` 

- on a git shelf, the Bash prompt also shows your git branch 
- _branches_ in git are names for versions (or nodes) 
- `ls -l` for long format item list 
- `git status` for local git repository information 


<----------------------------------------------------------------------------->
<-----------------DEFINITIONS------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Command Anatomy</span></p>

> command -parameter(s) argument(s)

- **Argument** 
  - input passed to the command
  - often the target of the command
- **Parameter**
  - term that modifies what the command does
  - also called a "flag"
- _**Option**_ -- a type of parameter that can be passed a value_
<----------------------------------------------------------------------------->

---
@title[How computers take orders]

### IO streams intro 

- We provide _input_ to make _orders_: 
  - keyboard (live input, device) 
  - file (stored input)

- Headwaiter Bash streams any results (& errors) as _output_: 
  - screen or terminal window, for interactive shells 
  - (redirected to) another process or file, for batch shells 

For example, help with commands 

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  command --help</span></p>

```bash
[username @ hostname lfr](master)$ ls --help
```
- **ls --help** for GitBash (Windows) 
- **man ls** for Linux & Mac "manual pages" 
- `q` to quit pagers 

<----------------------------------------------------------------------------->

---
@title[How computers represent information]

- Unix processes handle 3 streams of information:
  - **input**, for information needed to complete the process
  - **output**, for information generated by the process
  - **error**, for diagnostic messages generated by the process
  
- These concepts apply to other Operating Systems like Windows
- Let's see an error...

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  IO command error</span></p>

### Exercise:  try to order pie 

```bash
[username @ hostname lfr](master)$ pie
bash: pie: command not found...
[username @ hostname lfr](master)$ pie.sh
bash: pie.sh: command not found...
```
@fa[arrow-down]

<----------------------------------------------------------------------------->
+++
@title[How computers take orders]

Our Headwaiter Bash says `pie.sh` isn't on the menu.  
But we know this is a shell script.  

Let's order Bash to execute `pie.sh` anyway.  We can use: 

- the _absolute path_ (`/home/username/linux-for-research/pie.sh`)
- the Bash "dot" shorthand path (`./pie.sh`)  
- the Bash **command** & a _relative path_ (`bash pie.sh`) 

@fa[arrow-down] 

Note:
dot for 'current directory', like ~ for 'home directory' 

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  borrow Bash</span></p>

### Give pie recipe to another Bash (as input)  

```bash
[username @ hostname lfr](master)$ bash pie.sh
             (
              )
         __,.---.,__
     ,-='  /  |  \  '=-.
    :--.,___________,.--;
     \.,_____________,./ 

```
+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  use path</span></p>

### Use Bash dot-shortcut to order pie.sh 

similar to using the _absolute path_ (less typing) 

```bash
[username @ hostname lfr](master)$ ./pie.sh
             (
              )
         __,.---.,__
     ,-='  /  |  \  '=-.
    :--.,___________,.--;
     \.,_____________,./ 

```

<----------------------------------------------------------------------------->

+++
@title[How computers take orders]

What happened?  In both exercises, 
- another Bash process accepted _input_:  `pie.sh` 
- sub-shell Bash followed the recipe
- sub-shell Bash _output_ pie (& exited) 

Bash also has a **source** built-in command, which execute scripts directly (without a sub-shell).

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  source Bash scripts (import)</span></p>

### Source (import) script contents 

execute the contents of a script _in the current Bash_ 

```bash
[username @ hostname lfr](master)$ source pie.sh
             (
              )
         __,.---.,__
     ,-='  /  |  \  '=-.
    :--.,___________,.--;
     \.,_____________,./ 

```

Pie output is the same.  Functionally, sourcing uses just one Bash process. 
Sourcing (importing) will be important for scripting. 

<----------------------------------------------------------------------------->

---
@title[How computers represent information]

### Robot Kitchen's 3 special ingredients 

for receiving _**input**_ and sending _**output**_ 

- **stdin** -- standard input data stream 
  - keyboard, for interactive Bash Shells 
- **stdout** -- standard output data stream, for results 
  - screen or terminal window (interactive) 
- **stderr** -- standard error data stream, for warnings & diagnostic messages
  - also screen or terminal window (interactive) 

---
@title[How computers represent information]

While Bash can _order_ a copy of itself, it can't _execute_ it's own recipe. 

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  bash binary error</span></p>

###  Bash cannot follow binary recipes 

```bash
[username @ hostname lfr](master)$ bash bash
/usr/bin/bash: /usr/bin/bash: cannot execute binary file 
```
- recall that binary files are **direct** or **compiled** (like C code) 
- `/usr/bin/bash` is in machine-language, which Bash cannot read 

<----------------------------------------------------------------------------->


<----------------------------------------------------------------------------->
<-----------------DEFINITIONS------------------------------------------------->
<----------------------------------------------------------------------------->
+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Navigation Commands</span></p>

- **pwd** -- print working directory
  - where we are in the pantry (which shelf) 
- **ls** -- list directory contents (`ls -l` long format)
  - what items are on a shelf 
- **cd** -- change directory (`cd ~` to go home) 
  - go to another shelf in the pantry 
- **history** -- output command history to screen
  - keyboard arrows to browse history 
<----------------------------------------------------------------------------->
---
@title[How computers organise information]

### Git branch prompt brief
 
> branch parenthesis 
> checkout commands 

<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git checkout branch </span></p>

## Terminal - git checkout branch 
- git checkout cdc-data 

<----------------------------------------------------------------------------->
---
@title[Git prompt overview]

### Git prompt overview  


<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  move files</span></p>

## Terminal - move exercises 
- cd cdc-data
- ls 
- mv some files to better directories  

<----------------------------------------------------------------------------->

---
@title[How computers represent information]

### Shelf is a lie/metaphor 

Technically, the "shelf" is a lie... _metaphor_!
![cake on a shelf in a pantry](assets/path.jpg)


+++
@title[How computers represent information]

- The pantry speaks binary, like Chef Kernel.

"pantry shelves" (directories) &  
"ingredient containers" (files) 

...are abstractions we use to navigate computer data.

+++
@title[How computers represent information]

### Salt granules in containers 

- All ingredients are diced & mixed together in the pantry 
![salt container on a shelf](assets/path.jpg)

![pantry with sand art in it](assets/path.jpg)

Each granule contains some data.

+++
@title[How computers represent information]

- The "salt" container on our shelf maps to each salt granule in the pile.
- One of these granules contains metadata about the container   
- Why? 
  - So we aren't restricted by “shelf” or “container” size 
  - So we can have a pantry full of salt, if we want   

---
@title[How computers organise information]

### Linked Lists, Git 

> node concepts 
> like git branch checkout 
> file system 

<----------------------------------------------------------------------------->
<-----------------DEFINITIONS------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - File System, logical</span></p>

> Definitions
>> File System details 

**File system** (logical) -- hierarchy of directories 
**Directory** (folder) -- collection of files 
**Path** -- location of file(s)

---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - File System, structural</span></p>

**File system** (structural) -- type of data structures used to store information 
**Metadata** -- data that describes other data 
**Block** -- group of sectors on a hard disc 
**Sector** -- group of bytes (usually 512 bytes), minimum addressable unit of storage 
**Byte** -- unit of digital information (usually 8 bits, "octet") 
**Bit** -- binary digit, 0 or 1

<----------------------------------------------------------------------------->




<----------------------------------------------------------------------------->
<-----------------EXERCISE---------------------------------------------------->
<----------------------------------------------------------------------------->
---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  check shelf</span></p>

## Exercise:  check shelf 

```bash

```

[comment]: # (exercise slide)

<----------------------------------------------------------------------------->

