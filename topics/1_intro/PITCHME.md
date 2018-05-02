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





---?image=assets/orange_moon.jpg
<p><span class="slide-title">Exercise:  Open a web browser </span></p>

### using live & stored inputs 

- mouse to a shortcut icon & click it (live) 
- activate a browser program (stored) 
- launch a web browser process (live) 

@fa[arrow-down]

Note: 
<--------------------EXERCISE------------------------------------------------->

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






---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  make an order, GUI</span></p>

### Visit the GitHub website:

  - open a new tab 
  - visit seminar GitHub link <!-- PUT LINK HERE -->
  - look at some files 
  - (log in, if you have an account)

@fa[arrow-down]

Note:
<-----------------EXERCISE---------------------------------------------------->

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





---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  recipes</span></p>

- in GitHub online, look at (stored) **pie.sh** recipe 
  - format:  stored (file on disc) |
  - language:  Bash (sh) |
  - type:  interpreted |
- With your hands, use your (active) **mouse** process 
  - format:  live (user input, active instructions) |
  - language:  your OS suite (likely C) |
  - type:  compiled |

Note:
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





---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  hail a robot waiter</span></p>

- launch Terminal or GitBash 
  - look at the Waiter's prompt 
  - (we'll come back to this in a moment) 

---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  make orders</span></p>

- send some orders to Robot Waiter
  - `who` is logged in 
  - `ps` _what_ else this Waiter is doing 
  - `pwd` _where_ you are in the kitchen pantry
  - `ls` _list_ any other items on this shelf 

@fa[arrow-down]

Note:
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







---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - Computer terms</span></p>

- **Program** -- set of instructions for a computer to follow
- **Operating System** -- programs that work together to manage computer resources

- **File** -- stored information (can be a program)
- **Process** -- active program

- _**Program File** -- special file with instructions for a computer_

Note:
<-----------------------DEFINITIONS------------------------------------------->

---
@title[Robot Kitchen Staff]

- In Robot Kitchen, staff includes: |
  - Waiters to take orders 
    ![Waiter Shells](assets/path.jpg) |
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






---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  GUI orders, browser recipe</span></p>

## Exercise:  GUI orders, browser recipe   

- tab or mouse back to browser window 
- order another tab or window (process) 
  - mouse the + icon
  - or `CTRL-T` keyboard

What follows your orders?
> the active browser process 

@fa[arrow-down]

Note:
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






---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  ping google.com</span></p>

## Exercise:  use a Waiter to check google.com  

- Tab into Terminal or GitBash
- make a `ping` order: 
  - `ping google.com` to check if Waiter Shell can reach Google 
  - `CTRL-C` (Windows & Linux) or `CMD-C` (Mac) to quit active process 

---?image=assets/orange_moon.jpg
@title[Exercise:  time an order)]

## Exercise:  use a Waiter to time an order   

- `time` your `ping` order:
  - `time ping google.com` 
  - `CTRL-C` or `CMD-C` to quit active process
- examine _real_, _user_ (CPU), and _sys_ (CPU) time values 

What keeps track of this information?
  
@fa[arrow-right]

Note:
<-----------------EXERCISE---------------------------------------------------->

---
@title[How computers follow recipes]

### Computer System staff 

- For computers, we have:
  - **Operating Systems!**

- Waiter **Shells** take orders |
- **System Programs** use equipment & ingredients |
- Head Chef **Kernel** oversees programs & kitchen use |







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

Note:
<-----------------DEFINITIONS------------------------------------------------->

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

### Waiter Shells (the interpreters):

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
 
When your order comes in from Waiter Shell, Chef Kernel delegates some work to the saucier & patissier demi-chefs

- What if pie isn't on your Robot Kitchen menu?
  - We'll need to provide a recipe

- How?
> First, we add a pie recipe to our pantry 






---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  Download files, GUI</span></p>

## Exercise:  Download files, GUI

- Tab back to web browser 
- Get pie recipe from a web browser:
  - From GitHub 
  - Download `pie.sh`

@fa[arrow-down]

Note:
<-----------------EXERCISE---------------------------------------------------->


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





---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  GUI, find pie.sh</span></p>

## Exercise:  GUI, find pie.sh

- open GUI pantry doors:  `Finder` on Mac, `Explorer` on Windows
- mouse navigate, probably to your `Downloads` shelf 
- find `pie.sh` file 

@fa[arrow-down]

Note:
<-----------------EXERCISE---------------------------------------------------->


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

We'll need to ask Waiter Shell:  <!-- .element: class="fragment" -->
![chef, waiter, restaurant table, patron](assets/path.jpg) 

@fa[arrow-down]

+++
@title[How computers take orders]

- How do we ask a Waiter for a menu item?
  - type **commands** into a **shell** |
  
recall our `who, ls, pwd` from earlier...









---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  Waiter Shell's (interactive) prompt</span></p>

- tab to GitBash / Terminal (Interactive Shell)
- examine your shell prompt (Bash) 

```bash
[username @ hostname ~]$ 
```

Note:
<-----------------EXERCISE---------------------------------------------------->









+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">CLI Components</span></p>

- **Terminal emulator** (GitBash, Terminal) 
  - keyboard input & screen output
  - an interface between you and the Shell 
- **Shell** (Bash)
  - command-line interpreter
  - an interface between your commands and the Operating System
- **Command**
  - keyword for the computer
  - represents an executable set of instructions
  
Note: 
<-----------------DEFINITIONS------------------------------------------------->







---
@title[How computers take orders]

- **Interactive** shells "wait" for your keyboard input 
- interactive prompts typically show:
  - who you are (_username_) 
  - what kitchen you're at (_hostname_) 
  - where you're looking in the pantry (_directory_) 


Note:
Waiter Bash doesn't have "windows" for navigation.
We'll need to make orders _without a mouse_ - using **commands**
The Bash shell **process** will take our orders.
How?



---
@title[How computers represent information -- streams]

### Robot Kitchen's Process Streams 

for receiving _**input**_ and sending _**output**_ 

  - **input**, for information needed to complete the process
  - **output**, for information generated by the process
  - **error**, for diagnostic messages generated by the process

Note: 
These concepts also apply to other Operating Systems like Windows

---
@title[How computers take orders]

- When we provide _input_ to make _orders_, we can use: 
  - keyboard (live input, device) 
  - file (stored input)

- Waiter Bash can stream any _output_ (& _errors_) to: 
  - screen or terminal window, for interactive shells 
  - another process or file, for batch shells (or using redirect operators)

---
@title[How computers take orders]

- Unlike files (which live on hard discs), 

- **Processes** (like our Bash window) live in volatile storage like RAM
  - ![RAM](assets/path.jpg)
  - active instructions
  - "short-term" memory
  - only exist while the computer is on

---
@title[How computers take orders]

- The Bash processes' instructions are: 
> Check for orders (_input_)
> ..from us, the user

Let's order an appetizer!







---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  order the date</span></p>

```bash
[username @ hostname ~]$ date
Wed Mar 14 11:50:33 EDT 2018
```
  - the `date` **command** tells Bash we want some date information 
  - the **process** outputs this information (usually to the screen) 

@fa[arrow-down]

Note:
By default, date shows your current timezone.  This may be irritating when working with files from around the globe.  Let's try to get UTC


+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  order modifications</span></p>

Many menu items are configurable.  Before we get into the 

```bash
[username @ hostname ~]$ date -u
Wed Mar 14 08:50:33 EDT 2018
```
  - the `-u` **parameter** tells Bash we want the date it UTC format 
  - the **process** outputs this information (usually to the screen) 


Note:
<-----------------EXERCISE---------------------------------------------------->







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

Note:
Many commands have a `--help` parameter 

<-----------------DEFINITIONS------------------------------------------------->










---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  command --help</span></p>

```bash
[username @ hostname ~]$ ls --help
```
- **ls --help** for GitBash (Windows) 
- **man ls** for Linux & Mac "manual pages" 
- `q` to quit pagers 

Note:
The `--help` option prints brief command information directly to the screen.
Only the Linux & Mac `man` pages use pagers. 

We can pipe output to a pager in GitBash:  `ls --help | less`
More on piping later in the course. 

<-----------------EXERCISE---------------------------------------------------->








---?image=assets/green_moon.jpg
<p><span class="menu-title slide-title">Definitions:  IO streams</span></p>

- **stdin** -- standard input data stream 
  - keyboard, for interactive Bash Shells 
- **stdout** -- standard output data stream, for results 
  - screen or terminal window (interactive) 
- **stderr** -- standard error data stream, for warnings & diagnostic messages
  - also screen or terminal window (interactive) 

Note:
We will learn how to redirect these streams later in the course.  

<-----------------DEFINITIONS------------------------------------------------->






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








---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git the meal (workshop files)</span></p>

### order from Waiter Bash

- ask the Waiter what shelf we're on (should be home) 
- order a `git` recipe: 
  - `git clone` downloads the contents of a remote repository 

@fa[arrow-down]

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git the meal (workshop files)</span></p>

### order from Headwaiter Bash

```bash
[username @ hostname ~]$ pwd 
/home/username
[username @ hostname ~]$ git clone https://github.com/ccs-training/linux-for-research.git
```

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  list git repo ingredients</span></p>

```bash
[username @ hostname ~]$ ls
..
linux-for-research
..
```
There's the repository directory!  Let's see what's in it.

@fa[arrow-down]

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  TAB completion</span></p>

### Waiter Bash can finish text for you

```bash
[username @ hostname ~]$ ls lin[TAB]
```

- Waiter Bash will show possible targets, starting with `lin`
- If there is only one possible target, Bash will complete the target for you.

@fa[arrow-down]

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  TAB completion</span></p>


```bash
[username @ hostname ~]$ ls lin[TAB]
[username @ hostname ~]$ ls linux-for-research
..
pie.sh
..
```
- our new git shelf has some ingredients, including `pie.sh`!

Note:
<-----------------EXERCISE---------------------------------------------------->



---
@title[How computers organise information]

### How did Waiter Bash find our `git clone` and `ls` commands?

- Each shell has a special _menu_
- we can use the **which** command to locate other commands 

@fa[arrow-right] 











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

Note:
<-----------------EXERCISE---------------------------------------------------->



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








---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  find Bash's recipe shelf</span></p>

### Exercise:  find Bash's recipe shelf

```bash
[username @ hostname ~]$ which bash
/usr/bin/bash
```

Note:
<-----------------EXERCISE---------------------------------------------------->








---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - File System, logical</span></p>

> Definitions
>> File System details 

**File system** (logical) -- hierarchy of directories 
**Directory** (folder) -- collection of files 
**Path** -- location of file(s)


Note:
<-----------------DEFINITIONS------------------------------------------------->




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

- The "salt" container on our shelf **points** to each salt granule in the pile.
- One of these granules contains metadata about the container   
- Why? 
  - So we aren't restricted by “shelf” or “container” size 
  - So we can have a pantry full of salt, if we want   

Note:
In some filesystems, the salt container keeps a sequential list of **pointers** to each Salt granule (data node).

In other filesystems, the salt container keeps a **pointer** to the first granule only.
Each granule then keeps a **pointer** to the _next_ granule.

Both are (usually) done "behind the scenes" -- all we users "see" is the file.







---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - File Systems, details</span></p>

**File system** (logical) -- hierarchy of directories 
**Directory** (folder) -- collection of files 
**Path** -- location of file(s)

**File system** (structural) -- type of data structures used to store information 
**Metadata** -- data that describes other data 
**Block** -- group of sectors on a hard disc 
**Sector** -- group of bytes (usually 512 bytes), minimum addressable unit of storage 
**Byte** -- unit of digital information (usually 8 bits, "octet") 
**Bit** -- binary digit, 0 or 1

Note:
<-----------------DEFINITIONS------------------------------------------------->





---
@title[How computers organise information -- linked lists]

### Linked Lists, Shelves, & Git 

The Salt data container in the pantry works like a _linked list_:
 - **granules** of data in the pantry are found by 
 - **references** (that point to specific ***granules***)

![filesystem linked list image](assets/path.jpg)

+++
@title[How computers organise information -- linked lists]

Each **granule** contains some data for a single file. 

_We_ typically interact with _all the granules at once_ (an entire linked list of data). 

_The filesystem_ maintains **reference pointers** to the hard drive.  
Robot Kitchen interacts with & maintains the filesystem. 



 
+++
@title[How computers organise information -- linked lists]

### Linked Lists, Shelves, & Git 

Git also works like a _linked list_:
  - **commits** / ***versions*** of files (in the repository) are found by 
  - **references** / ***branches*** (that point to specific ***commits***)

![git linked list image](assets/path.jpg)

+++
@title[How computers organise information -- linked lists]

Each **commit** contains a collection of file versions. 

We typically interact with _individual commits_, one node in a list. 

_We help_ maintain git **reference pointers** to commits. 
_Git_ maintains the underlying version control system.


---
@title[How computers organise information -- linked lists]

### Linked Lists, Shelves, & Git 

In **filesystems**, we work with _the entire linked list_ (the file).
In **git**, we work with _individual nodes_ in the git linked list (the commit). 

These individual nodes contain files.

Thus, **git** is a linked-list collection -- of other linked-lists!

Note:
The concept of **git** as a collection of linked-lists will become important during git collaborations. 









---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - Linked Lists</span></p>


**Linked List** -- sequential set of data elements, each linked to a successor 

**node** -- a data element 
**pointer** -- a link to the next data element 

***Doubly-Linked List*** -- ...each node also linked to a _predecesor_ (previous node) 

Note:
Though filesystem linked-lists take place "behind the scenes",
git linked lists are somewhat under our control.
Let's take a look.
<-----------------DEFINITIONS------------------------------------------------->









---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  navigate to git shelf</span></p>

## Exercise:  navigate to `git` shelf

```bash
[username @ hostname ~]$ cd linux-for-research
[username @ hostname lfr](master)$ ls -l 
..
```

Note:
on a git shelf, the Bash prompt also shows your git branch 


---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  check git status</span></p>

```bash
[username @ hostname lfr](master)$ git status
On branch master
nothing to commit, working tree clean

[username @ hostname lfr](master)$ ls 
data_groups/       ftables/              meta/      
pie/               pie.sh     pie_full.sh
```

Note:
The working tree is our git _workspace_, the hard drive as Waiter Bash see's it 

<-----------------EXERCISE---------------------------------------------------->



---
<p><span class="menu-title slide-title">Git branches</span></p>

**Branches** in git are _references_ to specific versions, or _commits_ 

Most repositories will have a `master` branch by default.

Let's see what other branches we have...








---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git branches</span></p>

## Terminal - git branches 

```bash
[username @ hostname lfr](master)$ git branch -v
* ,rchkcp master*
* pk rc p pie
* cuk  p  cdc-data
* krp     cdc-file
* .rc,uh  cdc-script
* pr,pck  shell-env 
```

Note:
<-----------------EXERCISE---------------------------------------------------->



---
@title[How computers organise information -- git]

The git prompt shows us the **branch** our local workspace is using (in parenthesis). 

For ordering pie, let's stay on the `master` branch.  

Note:
For those of you familiar with git branches, we can also use the `pie` branch 









---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - Git</span></p>

### Git filesystem concepts 

**workspace** -- local hard drive versions, "as seen by Bash" 
**index** -- staged versions, as seen by git 
**repository** -- committed versions, as seen by git 
***branch*** -- the head of a list of committed versions 

`git status` should be clean of any uncommitted changes before changing git branches. 

Note:
Our newly-cloned git repository is free of any uncommitted changes.  

+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - Git</span></p>

### Git commands 

`git branch -v` -- show branches & brief version information 
`git status` -- show differences between _workspace_ and git spaces (index, stage) 

- `git checkout <branch>` -- change _workspace_ to head `branch` node   


Note:
<-----------------DEFINITIONS------------------------------------------------->







---
@title[How computers represent information]

Recall Unix's 3 streams of information:
  - **stdin**, for information needed to complete the process
  - **stdout**, for information generated by the process
  - **stderr**, for diagnostic messages generated by the process
  
If we order an item that isn't on Waiter Bash's menu, we might get an _error_


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

Note:
Waiter Bash says `pie.sh` isn't on the menu.  
But we know this is a shell script (in Bash's language).

Note:
<-----------------EXERCISE---------------------------------------------------->



+++
@title[How computers take orders]

Let's order "off-menu" 
(tell Bash to execute `pie.sh` anyway)

- We can use: 
  - the _absolute path_ (`/home/username/linux-for-research/pie.sh`)
  - the Bash "dot" shorthand path (`./pie.sh`)  
  - the Bash **command** & a _relative path_ (`bash pie.sh`) 

@fa[arrow-down] 

Note:
`.` (dot) for 'current directory', like `~` for 'home directory' 

Later, we will learn how to update Bash's menu. 










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

Note
<-----------------EXERCISE---------------------------------------------------->


+++
@title[How computers take orders]

What happened?  In both exercises, 
- another Bash process accepted _input_:  `pie.sh` 
- sub-shell Bash followed the recipe
- sub-shell Bash _output_ pie (& exited) 

Bash also has a **source** built-in command, which execute scripts directly (without a sub-shell).









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

Note:
Pie output is the same.  Functionally, sourcing uses just one Bash process. 
Sourcing (importing) other files will be important for scripting. 

<-----------------EXERCISE---------------------------------------------------->








+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  bash binary error</span></p>

###  Bash cannot follow binary recipes 

```bash
[username @ hostname lfr](master)$ bash bash
/usr/bin/bash: /usr/bin/bash: cannot execute binary file 
```
- recall that binary files are **direct** or **compiled** (like C code) 
- `/usr/bin/bash` is in machine-language, which Bash cannot read 

Note: 
While Bash can _order_ a copy of itself, it can't _read_ it's own recipe. 
(Chef Kernel can read the compiled Bash recipe)

<-----------------EXERCISE---------------------------------------------------->







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
  

Note:
Now, let's checkout the `cdc-data` branch...
<-----------------DEFINITIONS------------------------------------------------->
 
 
 
 
 



---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  git checkout branch </span></p>

## Terminal - git checkout branch 

```bash
[username @ hostname lfr](master)$ git checkout cdc-data 
[username @ hostname lfr](cdc-data)$ ls 
data_groups/       ftables/              meta/
header.list        header_col_names.tab  pie.sh
rename.source      
```

Note:
<-----------------EXERCISE---------------------------------------------------->


---
@title[How computers organise information -- git]

The `cdc-data` branch still has the `pie.sh` script file, 
but not the `/pie` directory.

> What happens if we try to order pie now?
> (remember to order "off-menu")









---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  pie from cdc-data </span></p>

### Exercise - order pie again, from cdc-data branch 

```bash
[username @ hostname lfr](cdc-data)$ ./pie.sh
bash:  source not found:  pie/steam.sh
bash:  source not found:  pie/crust.sh
bash:  source not found:  pie/base.sh
```

Note:
<-----------------EXERCISE---------------------------------------------------->



---
@title[How computers organise information -- git]

The `cdc-data` branch doesn't have all the ingredients!

If we want to order pie, we'll need to go back to the `master` branch.

For now, let's remove `pie.sh` from the `cdc-data` branch 








---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  remove pie recipe </span></p>

### Exercise - remove pie recipe 

```bash
[username @ hostname lfr](cdc-data)$ rm pie.sh
[username @ hostname lfr](cdc-data)$ ls
data_groups/       ftables/              meta/
header.list        header_col_names.tab  rename.source 
```
Note:
<-----------------EXERCISE---------------------------------------------------->



---
@title[How computers organise information]

### File Operation Permanence 

**DELETE IS FOREVER**

**File operations** performed by Shells like Bash are ***PERMANENT*** 

Robot Kitchen CLIs don't have "Recycle" or "Trash" bins.

When you tell the Shell to remove an item from the pantry,
**THAT ITEM IS GONE** 

Note:
But if you've been wondering why we used git to download files...


---
@title[How computers organise information -- git] 

### The Git Repository Copy 

Version control systems like `git` can be used to retrieve **copies** of items, from repositories.

> A version of the item must still exist in the repository. This usually means we haven't told git about our changes (or deletions).  

How can we find out if git still has a copy of our item?  

Check `git status`








---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  check git status</span></p>

### Exercise - check git status

```bash
[username @ hostname lfr](cdc-data)$ git status
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#       deleted:   pie.sh
#
```

Note:
<-----------------EXERCISE---------------------------------------------------->






---
@title[How computers represent information -- git]

### Git status 

Like changing branches, we can use `git checkout` to _retrieve_ copies of files from git (if they exist):

```bash
$ git checkout -- pie.sh
```

We can also **add** and **commit** our changes _to_ the repository, if we're sure about them.  

---
@title[How computers represent information -- git]

## Git commits 

`git commit` copies git _index_ versions into git _repository_ node. 

We'll first need to **add** our changes to the git _index_.

Let's **add** then **commit** our pie recipe removal.  

Note:
If you checked out `pie.sh` again, run `rm pie.sh` from the command-line to remove it (again).   









---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  add & commit changes to local git </span></p>

First, let's check `git status` 

```bash
[username @ hostname lfr](cdc-data)$ git status
On branch cdc-data
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    pie.sh

no changes added to commit (use "git add" and/or "git commit -a")

```

Note:
This shows the differences between our workspace (hard drive) versions,
and the most recent **commit** (git node) version of `cdc-data`. 

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  add & commit changes to git (locally)</span></p>

```bash
[username @ hostname lfr](cdc-data)$ git add .
[username @ hostname lfr](cdc-data)$ git status 
On branch cdc-data
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        deleted:    pie.sh

```

`git rm pie.sh` would also update the git _index_ 

Note: 
**Add** (or remove) the filesystem changes to the git staging area (the index)
Then **commit** the changes using the `-m` flag

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  add & commit changes to git (locally)</span></p>

Each **commit** requires a brief message describing changes.
Use the `-m` option to include the message in your line 

```
[username @ hostname lfr](cdc-data)$ git commit -m "remove pie script"
[cdc-data a2d1600] remove pie.sh.
 1 file changed, 1 deletion(-)
 delete mode 100644 pie.sh
```

Note: 
To save a version of these changes into our (local) git repository, we made a new node in the linked list. 

If you forgot the message flag, git may have launched your default text editor -- exit out, we'll come back to text editors later 

<-----------------EXERCISE---------------------------------------------------->









---?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">Definitions - Git updates</span></p>

### Git commands 

`git status` -- show differences between _workspace_ and git  
`git checkout -- <file>` -- change _workspace_ copy to repository copy    

- `git add .` -- add all _workspace_ changes to the git _index_ (stage)  
  - `git add <file>` -- add individual changes to the git _index_ 
  - `git reset HEAD <file>` -- undo git _index_ changes (unstage) 
- `git commit -m "message"` -- commit all _indexed_ (staged) changes to the git repository (as a new `(branch)` node) 

Note:
<-----------------DEFINITIONS------------------------------------------------->




---
@title[How computers organise information -- file operations]

Back in the `cdc-data` branch, let's take a peak at these header files with `cat` 

@fa[arrow-down]










+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  cat to view text files</span></p>

Recall Waiter Bash's TAB-completion feature

```bash
[username @ hostname lfr](cdc-data)$ cat header.list
YearStart
YearEnd
LocationAbbr
...
[username @ hostname lfr](cdc-data)$ cat header_[TAB]
[username @ hostname lfr](cdc-data)$ cat header_col_names.tab
     1	YearStart
     2	YearEnd
     3	LocationAbbr
...
```

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  Bash globbing</span></p>

Waiter Bash also has _globbing patterns_ (standard wildcards).

```bash
[username @ hostname lfr](cdc-data)$ cat head*

header.list

YearStart
YearEnd
LocationAbbr
...

header_col_names.tab

     1	YearStart
     2	YearEnd
     3	LocationAbbr
...
```

Note:
The asterisk represents zero or more characters in a pattern. 

For more on globbing, see online Linux manual pages:
http://man7.org/linux/man-pages/man7/glob.7.html

Note:
<-----------------EXERCISE---------------------------------------------------->




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
Similar to the globbing asterisk, Bash expands _directories_ like `meta/` into their contents.

`mv` cannot relocate multiple sources to an individual file 


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
What about creating files? 

<-----------------DEFINITIONS------------------------------------------------->




@title[How programs can be used together]

### Creating text files with redirection 

Waiter Bash's `>` **operator** redirects _outputs_ to a file 

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
 
 
 
 
 
---
@title[Waiter Bash's environment]

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
@title[Waiter Bash's environment -- notebook]

### Bash's Notebook 

- How does Bash keep track of this menu? 
  - with a personal notebook!

@fa[arrow-down]
  
+++
@title[Waiter Bash's environment -- notes]

### Bash's Notebook -- the Variables 

- When we hail Waiters, they bring a notebook & some notes
- Notes keep track of our kitchen preferences.
- _Key notes_ can be marked, to copy into all shell notebooks

--- 
@title[Waiter Bash's environment]

### Environment Variables & Shell Variables

- Waiters (shells) keep track of settings and preferences using variables
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
@title[Waiter Bash's environment -- history]

Recall that we can cycle through our most recent orders using the arrow keys.

- Our order history must be somewhere in the pantry
- `printenv` only prints Bash's _Key notes_ 

Note:
How else can we print a note?

---
@title[Waiter Bash's environment]

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
@title[Waiter Bash's environment -- environment variables]

### Environment Variables
#### Key notes, all shells (and subshells) get copies

- $SHELL -– the current shell (absolute path to Bash recipe)
- $USER -– your username
- $HOME –- absolute path to your home pantry shelf
- $HOSTNAME -– the Robot Kitchen you are in
- $PATH –- Waiter Bash's kitchen menu

`printenv SHELL` or `echo $SHELL` 

---
@title[Waiter Bash's environment -- shell variables]

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
@title[Waiter Bash's environment -- IFS]

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
- Waiters will queue up
- often, we will only see the newest Bash 

```bash
$ bash

$
```

**Environment Variables** to the rescue! 

+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  conga Bash</span></p>

How can we tell where we are in the Waiter line? 
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
@title[Waiter Bash's environment -- command execution]

### Command Execution 

When Bash processes orders, Robot Kitchen executes `fork` & `exec` system calls.

- `fork` starts a new process, by copying the current one
- `exec` replaces old process contents with new process contents 

During **command execution**, our Bash Copy is replaced by the _contents_ of the command's **program file**.

For subshells (_Conga Bash_), our Bash Copy is replaced by a new Waiter Bash (with a clean personal notebook).

Note:
Recall that all Waiters receive copies of **Key notes** (environment variables) for their notebooks 

---
@title[Waiter Bash's environment -- shell variables]

We can ask Bash to keep any note (as a _shell variable_):

```bash
$ MYNOTE="this is my note"
$ echo $MYNOTE
this is my note

$ printenv MYNOTE

```

No results from `printenv` indicate MYNOTE is not a Key note (environment variable).   

---
@title[Waiter Bash's environment -- exporting]

To make MYNOTE a Key note (**Environment Variable**), we can `export` it:

```bash
$ export MYNOTE
$ printenv MYNOTE
this is my note
```

Now `printenv` knows about this note, and subshells will get a copy. 

---
@title[Waiter Bash's environment -- copying]

**Reminder** 

Shell & Environment Variables are not shared.

If you change the value of MYNOTE, `export` it again to copy the new value to subshells. 


---
@title[Waiter Bash's environment -- menu]

### Bash's Menu 

We can check all menu recipes with `which -a`:

```bash
$ which -a ls
/usr/bin/ls
/bin/ls
/usr/bin/ls
```
In Waiter Bash's menu, the `/usr/bin/ls` shelf comes first. 

---
@title[Waiter Bash's environment -- menu]

### Bash's Menu -- PATH Key note 

A colon-separated (:) list of pantry shelves, searched in-order for commands 






---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  show menu/span></p>

```bash
$ printenv PATH
/usr/local/bin:/usr/local/sbin:/usr/bin:/usr/sbin:/bin:/sbin:/home/kalan/.local/bin:/home/kalan/bin
```
```bash
$ which ls
/usr/bin/ls
```

Note:
<-----------------EXERCISE---------------------------------------------------->


---
@title[Waiter Bash's environment  -- menu]

When we check which recipe an order will use, Bash:
- looks in the $PATH note for a list of pantry shelves
- checks each shelf in order for a matching recipe
- prints the absolute path of the first matching recipe


---
@title[Waiter Bash's environment  -- menu]

What if we have a recipe somewhere else in the pantry?
- We can modify Bash's PATH note!

### Bash profile mods section goes here 


+++?image=assets/bg_images/green_moon.jpg
<p><span class="menu-title slide-title">File Operations</span></p>

- `cat` output entire file(s) contents, sequentially 
- `sort` output sorted contents of all file(s) 
- `less` view (& search) file contents by page 
- `head` output first 10 lines of file(s)
  - `head -n X` output first X lines 
- `tail` output last 10 lines of file(s)
  - `tail -n X` output last X lines 

- `wc` print line, word, & byte counts for each file(s) 


Note:

<-----------------DEFINITIONS------------------------------------------------->





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
- `\`	Prevent or escape interpretation of the next character

- `' '`   Single-quotes, for literal characters & escape expansion `\` (backslash)
- `" "`   Double-quotes, to expand `\`, `$`, and `` ` `` (backtick)

