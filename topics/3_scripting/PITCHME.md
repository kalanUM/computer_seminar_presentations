@title[Scripting with the CLI]
## Scripting with the CLI

### Using the Shell

Something clever! <!-- .element: class="fragment" -->

---
@title[Scripting -- Intro]
<p><span class="slide-title">Introduction</span></p>

To begin, open GitBash  <!-- .element: class="fragment" -->

@fa[arrow-down]

+++?image=assets/bg_images/green_moon.jpg
@title[Scripting -- Learning Objectives]
<p><span class="slide-title">Learning Objectives</span></p>

- Understand how to redirect input & output |
- Understand how to chain sequences of commands |
- Understand how to save a set of commands in a script |





---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  navigate to git branch</span></p>

```bash
$ cd ~
[username @ hostname ~]$ cd lfr
[username @ hostname lfr](master)$ git branch -v
* ,rchkcp master*
* pk rc p pie
* cuk  p  cdc-data
* krp     cdc-file
* .rc,uh  cdc-script
* pr,pck  shell-env 
[username @ hostname lfr](master)$ git checkout cdc-data
..
[username @ hostname lfr](cdc-data)$ ll
total 44M
drwx------. 1 kalan kalan 4.0K Apr 10 13:47 ./
drwx------. 1 kalan kalan 4.0K Apr 10 13:47 ../
-rw-------. 1 kalan kalan 7.7K Apr 10 13:47 cdc_split.sh
drwx------. 1 kalan kalan 4.0K Apr 10 13:47 data_groups/
drwx------. 1 kalan kalan 4.0K Apr 10 13:47 ftables/
drwx------. 1 kalan kalan 4.0K Apr 10 13:47 meta/
-rw-------. 1 kalan kalan  44M Apr 10 13:47 U.S._Chronic_Disease_Indicators__CDI_mod.csv
```

Note:
<-----------------EXERCISE---------------------------------------------------->





---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  get file headers</span></p>

```bash
[username @ hostname lfr](cdc-data)$ head -n 1 U[TAB]
[username @ hostname lfr](cdc-data)$ head -n 1 U.S._Chronic_Disease_Indicators__CDI_mod.csv 
YearStart,YearEnd,LocationAbbr,LocationDesc,DataSource,Topic,Question,DataValueUnit,DataValueType,DataValue,DataValueAlt,DataValueFootnoteSymbol,DatavalueFootnote,LowConfidenceLimit,HighConfidenceLimit,StratificationCategory1,Stratification1,GeoLocation,LocationID,TopicID,QuestionID,DataValueTypeID,StratificationCategoryID1,StratificationID1
```

Note:
Recall `head` prints the first 10 lines, by default. 

***option*** `-n 1` to get only the first line. 

<-----------------EXERCISE---------------------------------------------------->




---
@title[Scripting - head & sed]

`head -n 1` output matches the file type, CSV - comma-separated values

What if we want a list instead?

Let's start by making our work a bit easier with a _shell variable_:




---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  set CSV shell variable</span></p>

```bash
[username @ hostname lfr](cdc-data)$ MYFILE="U[TAB]"
[username @ hostname lfr](cdc-data)$ MYFILE="U.S._Chronic_Disease_Indicators__CDI_mod.csv"
[username @ hostname lfr](cdc-data)$ echo $MYFILE
U.S._Chronic_Disease_Indicators__CDI_mod.csv
```

@[fa-arrow-down]

Note:
Bash expanded the **special character** `$` to use the _contents_ of the variable.  
What if we typed `echo MYFILE` (without the `$` special character)?

```bash
$ echo MYFILE
MYFILE
```

Let's run `head -n 1` using our new _shell variable_..


+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  use CSV shell variable</span></p>

```bash
[username @ hostname lfr](cdc-data)$ head -n 1 $MYFILE
YearStart,YearEnd,LocationAbbr,LocationDesc,DataSource,Topic,Question,DataValueUnit,DataValueType,DataValue,DataValueAlt,DataValueFootnoteSymbol,DatavalueFootnote,LowConfidenceLimit,HighConfidenceLimit,StratificationCategory1,Stratification1,GeoLocation,LocationID,TopicID,QuestionID,DataValueTypeID,StratificationCategoryID1,StratificationID1
```

Note:
<-----------------EXERCISE---------------------------------------------------->





---
@title[Scripting -- head & sed]

What can we do about these commas?

Let's try using the `sed` stream editor to replace strings.  










---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  sed script</span></p>

```bash
[username @ hostname lfr](cdc-data)$ man sed
/match

  s/regexp/replacement/
..
```

@fa[arrow-down]

Note:
Search the sed man pages for key terms `match`, `replacement`, `substitution`

Unfortunately, `sed --help` does not show syntax details.  Windows/GitBash users, try online man pages:

http://man7.org/linux/man-pages/man1/sed.1.html





+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  sed pipe test</span></p>

**Pipe** ` | ` the output of `head` to an empty `sed` script 

```bash
[username @ hostname lfr](cdc-data)$ head -n 1 $MYFILE | sed ""
YearStart,YearEnd,LocationAbbr,LocationDesc,DataSource,Topic,Question,DataValueUnit,DataValueType,DataValue,DataValueAlt,DataValueFootnoteSymbol,DatavalueFootnote,LowConfidenceLimit,HighConfidenceLimit,StratificationCategory1,Stratification1,GeoLocation,LocationID,TopicID,QuestionID,DataValueTypeID,StratificationCategoryID1,StratificationID1
```

@fa[arrow-down]

Note:
This confirms `sed` at least _receives_ the output of our `head` command.



+++?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  sed substitution syntax</span></p>

Fill-in _sed substitution_ syntax, using slash delimiter ` / `  

```bash
[username @ hostname lfr](cdc-data)$ head -n 1 $MYFILE | sed "s///"
sed: -e expression #1, char 0: no previous regular expression

[username @ hostname lfr](cdc-data)$ head -n 1 $MYFILE | sed "s/,//"
YearStart,,,YearEnd,LocationAbbr,LocationDesc,DataSource,Topic,Question,DataValueUnit,DataValueType,DataValue,DataValueAlt,DataValueFootnoteSymbol,DatavalueFootnote,LowConfidenceLimit,HighConfidenceLimit,StratificationCategory1,Stratification1,GeoLocation,LocationID,TopicID,QuestionID,DataValueTypeID,StratificationCategoryID1,StratificationID1
```

`sed "s/,//"` replace the first `,` with ` ` (nothing, i.e. remove it)


Note:
With an empty regexp, sed complains that there is no pattern to match (true). 

<-----------------EXERCISE---------------------------------------------------->


---
@title[Scripting -- sed]

### sed substitution syntax 

- `'s/<find>/<replace>/'` -- replace the 1st occurrence of `find` on each line 
  - `'s:<find>:<replace>/'` -- same, using `:` delimiter 
  
- `'s/<find>/<replace>/g'` -- replace all occurrences of `find` on each line 
  - `'s:<find>:<replace>:g'` -- same, using `:` delimiter 

Note:
`sed` can use nearly any character as a _delimeter_ (useful for expressions that use `/`)

+++
@title[Scripting -- sed]

### more sed substitution examples 

- `'s/<find>/<replace>/g'` -- replace all occurrences of `find` on each line 
- `'s/<find>/<replace>/g'` -- replace all occurrences of `find` on eachline 

GNU sed:
- `'2 s/<find>/<replace>/'` -- replace the 1st occurrence of `find` on the 2nd line 
  - `'3,5 s/<find>/<replace>/'` -- replace the 1st occurrence of `find` on lines 3-5
  - `'7,$ s/<find>/<replace>/'` -- replace the 1st occurrence of `find` on lines 7-last
- `'s/<find>/<replace>/2'` -- replace the 2nd occurrence of `find` on each line 



Note:
Use double-quotes ` " " ` to evaluate any $VARIABLE names
Use singe-quotes ` ' ' ` to prevent special character evaluation 


---?image=assets/orange_moon.jpg
<p><span class="menu-title slide-title">Exercise:  sed</span></p>

### sed replace , with [space]

```bash
[username @ hostname lfr](cdc-data)$ head -n 1 $MYFILE | sed 's:,: :g'
YearStart YearEnd LocationAbbr LocationDesc DataSource Topic Question DataValueUnit DataValueType DataValue DataValueAlt DataValueFootnoteSymbol DatavalueFootnote LowConfidenceLimit HighConfidenceLimit StratificationCategory1 Stratification1 GeoLocation LocationID TopicID QuestionID DataValueTypeID StratificationCategoryID1 StratificationID1
[username @ hostname lfr](cdc-data)$ head -n 1 $MYFILE | sed 's:,: :g'
```

Note:

<-----------------EXERCISE---------------------------------------------------->


