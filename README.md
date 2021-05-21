# Maximizing the benefits of VSCode

## Safety moment and intro

Discuss importance of testing of GFCI outlets. 

The purpose is for everyone to follow along but to get through the agenda, please reserve most questions till the end or place them in the chat to answer after. 

## 1. Customizing VSCode

### 1.1 Icons

Show group how to select icon theme and install a new one/activate it.

> File > Preferences > File Icon Theme

Toggled all options, select material theme icons light.

### 1.2 Themes

Show group the theme categories and how to install/activate a new one.

> File > Preferences > Color Theme

Dark, light or high contrast are categories.

Toggled all options, select atom one dark theme.


### 1.3 Programming fonts

What is a programming font?

- Use `https://www.jetbrains.com/lp/mono/` to explain

Show group how to download and install jetbrains mono and enable it VS Code + enabling font ligatures.

> Right click install

> File > Preferences > Settings > Text Editor > Font > Font family > Jetbrains Mono

> File > Preferences > Settings > Text Editor > Font > Font size > 14  

> File > Preferences > Settings > Text Editor > Font ligatures > Edit settings.json > editor.fontLigatures: true


### 1.4 Tweaking vscode

- Move the bar right or left
  > View > Appearance > Move side bar right
- Hide/show options for bottom bar
  > Right click > uncheck Tweet feedback
- Removing minimap
  > View > Show minimap


### 1.5 Language support

- Configure language file association
  > Click bottom right language > configure file extension
- Adding Cisco language extension
  > Extensions tab > cisco ios language package
  > Create myscript.cisco file and create association
  > Demo highlighting

### 1.6 Extensions

How to navigate extensions:

> Extensions > Flters > Categories

> Expand to see download & star counts

My extension suggestions:

- Cisco IOS Syntax
- Cisco IOS-XR Syntax
- Remote Development Bundle
- Python
- language-Ansible
- Markdown preview enhanced

### 1.7 Remote Development Bundle

> Extension > Remote Development Bundle

> Click on bottom left corner icon > Connect to host > Add new SSH Host > Enter connection string

> right click on bottom bar + check remote host, if missing the icon is missing from the bar

### 1.8 Git integration

> Open a new window with ctrl + shift + n

> Click explorer icon and clone repository ->
`https://github.com/aaronhuff/vscode-demo.git`

> Click on git tab on left bar

> Click current branch in bottom bar to create a new branch

> Click + to add file to pending commit

> Enter commit message in box

> Click checkmark to commit to staging

> Click push icon in bottom bar


## 2. Maximizing VSCode [25 minutes]

### 2.1 Shortcuts & cheatsheet

 Enjoy the productivity benefits of not having to switch between using the keyboard and mouse via keyboard shortcuts.

`https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf`

```list of my favourite shorcuts
General
=====================================
Ctrl+Shift+P or F1     Show Command Palette
Ctrl+Shift+N            New window/instance

Basic editing
=====================================
Ctrl+X   Cut line (empty selection)
Ctrl+V   Paste

Search and replace
=====================================
Ctrl+F  Find
Ctrl+H  Replace

Multi-cursor and selection
=====================================
Alt+Click           Insert cursor
Ctrl+Alt+ ↑ / ↓     Insert cursor above / below

Rich languages editing
=====================================
F2      Rename Symbol
F12     Go to Definition

File management
=====================================
Ctrl+N  New File
Ctrl+O  Open File
Ctrl+S  Save

Display
=====================================
Ctrl+B  Toggle Sidebar visibility

Debug
=====================================
F5  Start/Continue

Integrated terminal
=====================================
Ctrl+`  Show integrated terminal
```
> Customize keyboard shortcuts under file > preferences  > keyboard shortcuts


### 2.2 Quickcut and paste

> Ctrl + X without selection to cut line

> Ctrl + v to paste line

### 2.3 Multiline Edit

> Ctrl + Alt + ↑ / ↓

Use content block below to demo

``` sample code block
  neighbor 192.168.0.1 remote-as 100
  neighbor 192.168.0.1 description my first neighbor
  neighbor 192.168.0.1 send-community both
  neighbor 192.168.0.1 advertisement-interval 10
```

### 2.4 Intellisense

Show how intellisense helps save time via a new python file.

```
from time import sleep

# define messages
msg1 = "Wait, a second..."
msg2 = "You did it"

# run program
print(msg1)
sleep(5)
print(msg2)

```

### 2.5 Snippets

With custom user snippets, we can build the full ios autocomplete functionality in or build even more advanced standard templates to streamline the code process.

```sample commands
router ...
interface ...
neighbor ...
```

## 3. Using the terminal [10 minutes]

### 3.1 Picking your default terminal

Change and set a default terminal

> Ctrl+` to open termina

> Click + to the right 1: active_terminal > select a different terminal type

> Click + > Select default profile to set default terminal

### 3.2 Quick talk about terminal options

- Powershell is great for windows
  - I suggest adding "oh my posh" and "posh-git" to make it much more useable
- Z-Shell is my favorite for Linux
  - I suggest adding "oh my zsh" to make it much more useable

## 4. Debugging code [10 minutes]

> Click debug tab

> Click to the left of code to add breakpoints

> Click run and debug to start 

> Show variable definitions on left bar was assigned

## 5. Additional content

- Tips and tricks 

    `https://code.visualstudio.com/docs/getstarted/tips-and-tricks?ref=hackernoon.com`

- Pluralsight course 

    `https://app.pluralsight.com/library/courses/visual-studio-code/table-of-contents`

- Programming Fonts 

    `https://braydoncoyer.dev/blog/6-best-fonts-for-programming-in-2021/`
