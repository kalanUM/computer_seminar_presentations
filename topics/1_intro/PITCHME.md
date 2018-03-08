@title[these are Table of Contents Labels and do not show on slides]

None of these @titles or @fa work in local preview 
Check if alternate slide syntax works 
text sizing is also not working in local preview  

#VSLIDE

Vertical slide examples, made entirely of images (in assets)

#VSLIDE?image=assets/img0.png
<!-- .slide: data-background-transition="none" -->
#VSLIDE?image=assets/img1.png
<!-- .slide: data-background-transition="none" -->

#HSLIDE

## Single element fragment HTML 

<span class="fragment">
**synchronous** *adj.* - existing or occurring at the same time.
</span>

#HSLIDE

## Computers and the CLI 

### Interacting with operating systems 

Who needs a mouse when we have keys! 

To begin, double-click a web browser (GitBash, Terminal) icon...  
with your mouse

---
@title[Introduction Slides]

### Learning Objectives

None of these pipes are working in preview 

- Understand how computers represent information |
- Understand how to intercat with the computer using commands |
- Understand how to organise your digital work in directories |

@fa[arrow-down]

+++?color=orange

### Assumptions

- Laptop computer with internet access
- Familiarity with GUIs (Windows, Mac OS)
- Terminal emulator program 
  - Terminal on Mac OS
  - GitBash on Windows

+++?image=assets/green_moon.jpg
<p><span class="menu-title slide-title">HTML Version of a GitPitch Slide Title</span></p>

HTML titles work, and they display in regular font at top of slide 
HTML fragments work, too 

## Interfaces

- GUI - graphical user interface
  - "windows" of work            <!-- .element: class="fragment" -->
  - mouse input                  <!-- .element: class="fragment" -->
  - user-friendly & wide-angle   <!-- .element: class="fragment" -->

- CLI - command-line interface
  - "lines" of work              <!-- .element: class="fragment" -->
  - keyboard input               <!-- .element: class="fragment" -->
  - efficient & myopic           <!-- .element: class="fragment" -->

@fa[arrow-right]

[comment]: # (images are the GitPitch way to control individual slide bgs without custom CSS)

[comment]: # (comments like this, with newline above, should not render in HTML or GitPitch)

---
@title[How computers represent information]

## How computers represent information 

Everything we can do graphically, we can also do with the keyboard:
- manage documents (move, rename)
- manage permissions 
- search
- manipulate text

![GUI drag & drop, search](assets/path.jpg)

@fa[arrow-down]


[comment]: # (add '?n=true' to GitPitch URL to view Speaker Notes)

[comment]: # (press 's' on keyboard to enter GitPitch Seaker Notes Pane view)

Note:
- How?  Computers take the same orders, regardless of the interface.


+++
@title[How computers represent information]

Computers have hardware & software:
![computer stuff](assets/path.jpg)

They're built to help process information: 
- store & access data
- perform calculations & tasks 

They receive input & produce output:
![terminal stuff](assets/path.jpg)

Note:
"Folders" are also files (more on this later)

+++
@title[How computers represent information]

How do we give them information to process?
> by typing it, traditionally

How do they process it?
> by following special instructions (that someone else typed)

To a computer, all information is either:
- a **file** (stored data, static)
- a **process** (active instructions, dynamic)

+++
@title[How computers take orders]

- **Files** just sit there
- **Processes** do all the work
  - they accept _input_ and provide _output_

- Input can be:
  - "stuff we typed a while ago" (a file)
  - "stuff we're typing right now" (live stream)

+++
@title[How computers take orders]

How do processes work?
> by following detailed instructions!

Special files called **program files** contain procedures * instructions for the computer:
![bin or exe images, MS Office icons](assets/path.jpg)

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

What do commercial kitchens do?
- facilitate food processing & service (fill orders)

How?  In these 2 ways:
- store ingredients (& recipes)
- follow recipes

Like kitchen equipment,  
computer equipment only does _what instructed to do_

+++
@title[Robot Kitchen Equipment]

## Robot Kitchen Equipment

Robot Kitchen's Stand Mixer:
![stand mixer](assets/path.jpg)

> Until a robot chef pushes some buttons, it doesn't do anything  
> 
> If Robot Chef pushes the _wrong_ buttons, the mixer might ruin your order


---?image=assets/orange_moon.jpg
@title[Exercise:  make an order (push GUI buttons)]

## Exercise:  make an order
### (push GUI buttons)

- Visit a website:
  - open a web browser (launch a process)
  - visit GitHub or some other file host
  - Log into the site

@fa[arrow-down]

+++
@title[How computers take orders]

### GUI orders, behind the scenes:

- "Open a web browser"
  - Navigator (input):  mouse to icon
  - Action (input):  mouse double-click
  - Recipe (output):  launch a web browser
- "Visit a website & log in"
  - Navigator (input):  mouse to address bar, login fields
  - Action (input):  keyboard & mouse clicks
  - Recipe (output):  display website in browser, send text to website


---
@title[How computers take orders]

- In computer systems,
  - **Programs** are like recipes for Robot Kitchen
  - **Operating Systems** are like chefs & kitchen staff
  - **Processes** are the recipes our chefs are making

- When we place an order, Robot Kitchen staff:
  - check the menu
  - find recipes
  - follow them (make our orders)

---
@title[Robot Kitchen]

- How well kitchens perform often depends on recipes
- Robot Kitchen staff know about some basic recipes
  - ![system programs image](assets/path.jpg)
- We can provide custom recipes
  - ![pie.sh screenshot](assets/path.jpg)


---?image=assets/orange_moon.jpg
@title[Exercise:  recipes)]

## Exercise:  recipes

- in GitHub online, look at recipe **pie.sh**
  - format:  stored (file on disc)
  - language:  Bash (sh)
  - type:  interpreted
- With your hands, use your **mouse** recipe
  - format:  live (user input, active instructions)
  - language:  your OS suite (likely C)
  - type:  compiled 

---
@title[How computers follow recipes]

- In general, recipes can be:
  - live or stored ![input devices, commands](assets/path.jpg)
  - yours or someone else's ![mouse clics, OS](assets/path.jpg)
  - direct or indirect ![in machine language, needs interpretation](assets/path.jpg)

Note:
Live instructions

+++
@title[How computers follow recipes]

Indirect (_interpreted_):  recipes like shell scripts
- The **program file** is in "human" language
  - Robot Kitchen staff has an interpreter
  - Each instruction is converted into machine language **live**
  - There is only 1 file, yay!

Direct (_compiled_):  recipes like C code
- The **program file** is in machine language
  - Robot Kitchen staff doesn't have an interpreter
  - All instructions must be translated into machine language first 
  - There are two files:  
  'source code' (our recipe) & 'compiled code' (Robot Kitchen's recipe)

Note:
For 'interpreted' languages 

---?image=assets/green_moon.jpg
<p><span class="menu-title slide-title">Definitions</span></p>

## Definitions

- **Program** - set of instructions for a computer to follow
- **Operating System** - programs that work together to manage computer resources

- **File** - stored information (can be a program)
- **Process** - active pogram

- **_Program File_** - _special file with instructions for a computer_

---
@title[Robot Kitchen Staff]

- In Robot Kitchen, staff includes: |
  - Servers to take orders 
    ![Server Shells](assets/path.jpg) |
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

---
@title[How computers follow recipes]

- For computers, we have:
  - **Operating Systems!**

- **Shells** take orders
- **System Programs** use equipment & ingredients
- Head Chef **Kernel** oversees programs & kitchen use 

---?image=assets/green_moon.jpg
<p><span class="menu-title slide-title">Operating System Components</span></p>

## Operating System Components

this slide is too long 

- **Kernel**
  - core component of an operating system
  - responsible for resource management & program execution
- **Shell**
  - interfaces with the **kernel**
  - interprets user commands
- **System Programs**
  - implement most OS functions, like: |
  - input devices
  - user environments
  - schedulers 

---
@title[Robot Kitchen Staff]

- During kitchen prep, staff:
  - check the pantry
  - read recipes
  - follow instructions

- Once the kitchen opens, staff:
  - take & process orders 

@fa[arrow-down]

+++

### Chef Kernel (the manager):  

- knows the equipment in our kitchen (from mixing bowls to stove tops) and how to use it
- speaks low-level languages like machine code (binary) and assembly (symbolic binary)
- does not speak high-level languages (requires an interpreter) 

@fa[arrow-down]

+++

### Server Shells (the interpreters):

- check that your items are on the Robot Kitchen menu
- tell Chef Kernel about your order 
- speak some high-level languages 
- speak enough assembly to interpret for Chef Kernel 

@fa[arrow-down]

+++ 

### Demi-chefs (the helpers):  

- receive tasks from Chef Kernel 
- use kitchen equipment
- sort the pantry ingredients

---
@title[How computers take orders]
 
When your order comes in from Server Shell, Chef Kernel delegates some work to the saucier & patissier demi-chefs

- What if apple pie isn't on your Robot Kitchen menu?
  - We'll need to provide a recipe

- How?
> Let's first add a pie recipe to your pantry 

---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  Download files, GUI</span></p>

## Exercise:  Download files, GUI

- Get pie recipe from a web browser:
  - From GitHub or some file host
  - Download pie.sh
  - (maybe download some profile configs while here) 

- What happens behind the scenes?

---
@title[How computers take orders]

## Third-party GUI delivery service

- We tell the GUI we want this data in our pantry (with our mouse) 
- The browser orders menu item X from the kitchen staff:
  - "download web data into my pantry"
- Kitchen staff finds & follows recipes to get `pie.sh`:
  - get contents from web
  - save in my pantry (as an item, on a shelf)
- Kitchen staff tells the browser when finished
- Browser GUI tells us:

>`pie.sh` is now in your pantry!

---
@title[How computers represent information]

- Where did our file go?
> onto a shelf in the pantry

- Files (like recipes) live in non-volatile storage, like hard discs
  - ![hard disc/drive](assets/path.jpg)
  - stored data
  - "long-term" memory
  - persist through power loss

--- 
@title[How comuters represent information]

- Computers parallel paper filing systems: |
  - recipes & notes, kept in folders, kept in drawers or on shelves
  - ![pantry, discs](assets/path.jpg) |
  - hands, to sort & hold notes 
  - ![hands, RAM](assets/path.jpg) |
  - calculators, scales, & measuring equipment 
  - ![CPU, cale, tablespoons](assets/path.jpg) |
  - instructions & manuals 
  - ![software, stand mixer manual](assets/path.jpg)

---?code=path/to/source.file

@[1](Code Fragmenter line number annotations)
@[3](will be rendered on slide)
@[5-7](under code fragment focus blocks)

---

#### Size 4 Headers
#### Will likely be smaller than regular fonts 

<br>

The *same syntax* you use to create project   
**READMEs** and **Wikis** for your Git repos.

---

### Flux Design

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

![Flux Explained](https://facebook.github.io/flux/img/flux-simple-f8-diagram-explained-1300w.png)
