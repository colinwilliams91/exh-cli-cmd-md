```ts
this is a cataloging of commands and shortcuts i have found useful along my coding journey
-
ctrl + f to search for the cli term you are looking for (annotated w/ keywords and descriptions)
-
search using the roman numeral indexed legend for system or technology lookup
```

| Index | Technology         | System           |
| :---: | ------------------ | ---------------- |
| I     | Visual Studio Code | IDE              |
| II    | Visual Studio      | IDE              |
| III   | Bash               | Terminal         |
| IV    | Powershell         | Terminal         |
| V     | Command Prompt     | Terminal         |
| VI    | Oh My Zsh!         | Terminal         |
| VII   | Node               | Framework        |
| VIII  | .Net               | Framework        |
| IX    | Ubuntu             | Operating System |
| X     | Windows            | Operating System |
| XI    | Cron               | Misc.            |
| XII   | Postman            | Misc.            |
| XIII  | Tree               | Misc.            |

---
---

# :: IDE ::
---

# I. VSCode
`open file "side by side" (in new panel)`
```ts
ctrl + \
```

`open file in second panel`
```ts
ctrl + enter
```

`focus file explorer panel`
```ts
ctrl + 0 // <<-- 1, 2, 3 etc.. == panels
```

`focus terminal`
```ts
ctrl + `
```

`focus source control view`
```sh
ctrl + shift + g
```

`inside terminal to do "reverse lookup history" (commands entered)`
```ts
ctrl + r
```

`goto/go to definition`
```
fn + f12
```

`goto/go to references`
```sh
shift + fn + f12
```

`select current line`
```sh
ctrl + l
```

`open markdown preview`
```sh
ctrl + shift + v
```

`Side by side Markdown edit and preview`
```sh
ctrl + k, v # ctrl + k, then release, press v
```

`change coding language` (inside text editor)
```sh
ctrl + k, m # release ctrl + k, then press m
```

`navigate history (tabs?)`
```sh
ctrl + tab
alt + left # navigate back
alt + right # navigate forward
```

`navigate to specific line`
```sh
ctrl + g
```

`add additional cursors to all occurrences`
```sh
ctrl + shift + l
```

`ctrl + K + M` --> "change language mode" --> JSON to format JSON stringified object grabbed from browser

# II. Visual Studio

`run application`
```sh
ctrl + fn + f5 # <<-- default run
fn + f5 # <<-- debug run (slower)
```

`open terminal (View.Terminal) shortcut added`
```sh
ctrl + shift + t
```

`quick launch`
```sh
ctrl + q # search commands keywords e.g: "new"
```

`multiline comment`
```sh
shift + alt + a # multi line /* */

ctrl + k, ctrl + / # single line (can be multi) //

ctrl + k, ctrl + c # alternate single line comment
ctrl + k, ctrl + u # uncomment
```

`see all references`
```C#
alt + 2 // <<-- shows where used
```

`<summary></summary> C#Docs`
```C#
/// <-- will auto populate this...
/// <summary>
/// Comment goes here
/// </summary>

// e.g.
/// <summary>
/// Comment goes here
/// </summary>
///
```
### Create
`create a new file in project`
```sh
shift + fn + f2 # with Add New File extension
---
ctrl + shift + a
ctrl + n # alternate option
ctrl + shift + n # new project
```

`create new Class in project` (custom) (j === insert)
```c#
ctrl + shift + j, c // release then press c
```

`create new Interface in project` (custom) (j === insert)
```c#
ctrl + shift + j, i // release then press i
```

`format`
```sh
ctrl + k, ctrl + d # formats entire DOCUMENT (d = doc)
ctrl + k, ctrl + f # formats selection (f = format)
```
### Navigate

`focus text editor`
```sh
esc # literally, just hit escape once...
```

`navigate tabs | close tabs`
```sh
ctrl + tab # next tab
ctrl + shift + tab # prev tab
ctrl + fn + f4 # close active tab
alt + w + l # close all tabs
```

`navigate to solution explorer`
```sh
ctrl + alt + l # ctrl + tab navigate tabs here too
ctrl + ; # to solution explorer w/ search bar
```

`go to line start`
```sh
fn + k # k === "home"
ctrl + / + leftArrow # Edit.LineStart
```

`go to line end`
```sh
fn + , # , === "end"
ctrl + / + rightArrow # Edit.LineEnd
```

`go to Class(?)`
```C#
ctrl + click // highlighted class
```

`Go To`
```sh
ctrl + g # go to line
fn + f12 # go to definition
ctrl + fn + f12 # go to declaration
ctrl + d # go to next (highlighted selection)
```

`Go To All` (NICE)
```sh
ctrl + t # backspace to clear out "symbol"
```

`find closing brace`
```sh
ctrl + ]
```

`add cursor above/below`
```sh
ctrl + alt + upArrow
ctrl + alt + downArrow
```

`collapse/expand code blocks`
```sh
ctrl + m, ctrl + m
```

`replace`
```sh
ctrl + h
```

`replace all occurrences`
```sh
alt + a # once you have entered what you would like to sub
```

`delete to...`
```sh
ctrl + delete # delete to start of word
ctrl + backspace # delete to end of word
```

`save all`
```sh
ctrl + shift + s
```

`view in browser`
```sh
ctrl + shift + w
```

`bookmark` (_a keyboard chord is multiple shortcuts in a row_)
```sh
ctrl + k, ctrl + k
```
- `View >> Bookmark Window` to view all Bookmarks

`next split pane`
```sh
fn + f6
```

`collapse markup element (html)`
```C#
ctrl + m, ctrl + m
```
### Debugger:
`add breakpoint (highlight line first)`
```sh
fn + f9 # <<-- press again to remove
```
`continue to next breakpoint (inside debugger)`
```sh
fn + fn5
```
`step over (inside debugger)`
```sh
fn + f10
```
`step into method (inside debugger)`
```sh
fn + f11
```
`step out of method (if accidentally stepped in)`
```sh
shift + fn + fn11
```
`exit debugger`
```sh
ctrl + shift + fn + f5
```

`replace (find and replace)`
```
ctrl + h
```

`rename all properties`
```sh
ctrl + r, ctrl + r
```

`solution explorer (folder explorer)`
```
ctrl + alt + l
```

`copyLinesDown (without VSCode extra mappings`
```
ctrl + d
```

`alternate copyLinesDown option`
```sh
# without any selection
ctrl + e
ctrl + v
alt + up/down # <<-- to move
```

`extensions with .user will not get checked-in`
```
httpenv.json.user
```

`auto fix suggestions`
```sh
alt + enter
```

`compile/build application` show error/warning outputs
```sh
ctrl + shift + b
```

### Refactor
`extract method`
```C#
ctrl + r, ctrl + m
```

### Object Browser
```sh
ctrl + alt + j
```
- `ctrl + click` on `var` or `type identifier` to open object definition, which will show all attributes and methods on datatype "constructor" parent object ("`struct`" in C#) (available methods)

### Code Snippets (inside VS)
- enter these aliases inside your IDE text editor
`Console.WriteLine()`
```sh
cw # press tab twice
```
`public CodeSnippetExamples() { }` "Constructor"
```sh
ctor # press tab twice
```
`public string LastName { get; set; }` "Property"
```sh
prop # press tab twice
propfull # <-- creates FULL prop w/ getter & setter
```
`try { } catch (Exception) { throw; }` try/catch block
```sh
try # press tab twice
tryf # try/finally block
```
- instantiate the Exception inside `catch (... ex)`
`for loop`
```sh
for # press tab twice
forr # for loop decrement
```
`foreach loop` including collection
```sh
var names = new List<string>();
foreach # press tab twice
```
- will output: `foreach (var name in names) { }`
`while loop`
```sh
while # press tab twice
```
`do { } while (true);`
```sh
do # press tab twice
```

`populate snippets from context menu`
```sh
ctrl + k, ctrl + x
# for example, surround With or e.g. Wrap {} w/ braces
```

---
---

# :: TERMINAL ::
---

# III. Bash
`following are bash specific`

**Explorer Windows File System** (so helpful connecting sub-system partition to main OS)
`open windows file explorer GUI for WSL`
```sh
explorer.exe .
```
##### How to `echo` or `cat` write to a file with Bash:
```bash
cat >> /path/to/existingFile.text<< EOF
some text line 1
some text line 2
some text line 3
EOF
```
switch `cat >>` to `cat >` to create a file instead of append
```bash
cat > /path/to/newFile.text<< EOF
some text line 1
some text line 2
some text line 3
EOF
```

`(( expression ))` <-- this will execute/perform an expression

`print BASH env`
```sh
printenv
```

`echo variables` (example how to access vars in BASH)
```sh
echo $LANG # <-- LANG env var (bash)
```

`$RANDOM in BASH will create a random number`
```sh
echo $RANDOM # <-- 22024 : between 0 and 32767
```

```sh
I=0 # <-- passing this in the terminal will persist a var
(( I++ )) # <-- I will now become 1 and persist
# we don't need to prepend $ for vars in (( expression ))
```

`this will print expressions for (( expression )) operations`
```sh
help let
```
##### `View file "long" with permissions list`
```sh
ls -l
```

`-rw-r--r--` in front of the file indicates the permissions: **`r` = read, `w` = write, `x` = execute**
**output:** `-rwxr-xr-x` <-- see **`x`** by 3 different "users" (all users can execute now)
##### `Give executable permissions to a file`
```sh
chmod +x filename.whatever
```

`man` command is "manual" (like `help`)
```sh
man bash # <-- prints manual for bash
man sleep # <-- prints manual for sleep (binary)
```

**`-e` flag needed for special characters**
```sh
echo -e "\n~~ Countdown Timer ~~\n"
```

`lists root of the file system`
```sh
ls /
```
_ls /bin will list all binaries on the file system. Bash lives here: #!/bin/bash which will use bash commands. we can access other binaries or libraries here_


`lists bash commands`
```sh
help
```

`things we can pass to the bash TEST command (for testing true/false (for ifs or [[ EXPRESSIONS ]]))`
```sh
help test
```

```sh
( expression ) # <-- evaluates expression/returns value
```

```sh
help [[ expression ]] # <-- output below
```

      ( EXPRESSION )    Returns the value of EXPRESSION
      ! EXPRESSION              True if EXPRESSION is false; else false
      EXPR1 && EXPR2    True if both EXPR1 and EXPR2 are true; else false
      EXPR1 || EXPR2    True if either EXPR1 or EXPR2 is true; else false

    When the `==' and `!=' operators are used, the string to the right of
    the operator is used as a pattern and pattern matching is performed.
    When the `=~' operator is used, the string to the right of the operator
    is matched as a regular expression.

    The && and || operators do not evaluate EXPR2 if EXPR1 is sufficient to
    determine the expression's value.

    Exit Status:
    Returns success if EXPR evaluates to true; fails if EXPR evaluates to
    false or an invalid argument is given.

**`we can evaluate any expression in the BASH terminal or .sh script:`**
```sh
[[ 4 -le 5 ]] # <-- `-le` === less-than-or-equal
```

`echo $?`
```sh
echo $? # <-- prints last bash command's EXIT STATUS
0 # <-- 0 === true (0 === no errors)

[[ 4 -ge 5 ]]
echo $?
1 # <-- 1 === false (> 0 === contains errors | "false")
```

```sh
[[ 4 -ge 5 ]]; echo $? # <-- run multiple comands on single line with `;`
1 # <-- output
```

**_we can think of `0` return as TRUE but it actually means `command had 0 errors`_** (***EXIT STATUS***)

`check if a file exists (and output EXIT STATUS)` **`-a | -e`**
_THIS WILL CHECK THE FOLDER FROM WHERE THE COMMAND WAS ENTERED_
```sh
[[ -a countdown.sh  ]]; echo $?
0 # <-- output 0 if file exists
```

`to list all variables in BASH`
```sh
declare -p
```


`all variables: @ | *`
```sh
ARR=("a" "b" "c")
echo ${ARR[@]}

declare -p ARR
# --> declare -a ARR=([0]="a" [1]="b" [2]="c")
# --> -a === array
```

`Read (capture user INPUT)`

`capture user input`
```sh
read
```

### Debugging in Bash

`set -x` _at the top of a script enables debugging (printing executed commands to the terminal)_
```bash
#!/bin/bash

set -x

# Your script goes here
```

# IV. Powershell

`get powershell version`
```powershell
$PSVersionTable.PSVersion
```

`open persistent PS profile file`
`will create new $PROFILE if not exists`
```powershell
code $PROFILE.AllUsersAllHosts
```

`put this inside your $PROFILE.ps1`
`opens specified dir on shell launch`
```powershell
Set-Location C:\Users\User\Dev
```

`to Set-Alias that takes params`
```powershell
function ListAll { # script block/fn
    Get-ChildItem -Force
}

Set-Alias ls-a ListAll # create Alias/invoke
# Set-Alias -Name list -Value cmdlet/fn
# this above syntax only works for no params
```

`find windows IPs`
```powershell
ipconfig
```

`find WSL IPs`
```powershell
wsl hostname -i
wsl hostname -I
```

`open Visual Studio IDE latest version`
```powershell
start devenv
```

`open Visual Studio IDE specific solution (folder or file)`
```powershell
start devenv solution1.sln # file extension? solution?
# because I have multiple VS installed on my machine, i need to include the entier absolute path to the executable in order to run from CLI
```

`open current folder in windows explorer`
```powershell
ii . # <<-- alias Invoke-item
```

`create a new file`
```powershell
New-Item example.txt
```

`delete recursive rm -rf`
```C#
Remove-Item -Recurse -Force <path>
```

# V. Command Prompt

`display directory contents`
```C#
dir // <<-- windows/cmd version of `ls`
```

# VI. Oh My ZSH!

`runs zsh powerlvl10k setup (prompt styling)`
```sh
p10k configure
```

---
---
# :: FRAMEWORKS ::
---

# VII. Node

`find all running node processes`
```
ps -ef | grep node
```

`find node process by port`
```
lsof -i :3000
```

`kill process`
```
kill -9 PROCESS_ID
```
# VIII. .Net

`restore nuget packages`
```C#
dotnet restore
```

`run C# program.cs (entry point)`
```powershell
dotnet run
```

`create new console app .NET`
```powershell
dotnet new console -o ./CsharpProjects/TestProject
# pass `--use-program-main` for Program Class template
```

**(VSCODE)**
`generate assets for build and debug`
```C#
ctrl + shift + p // cmd pallette
// enter ".net: g"
// select ".NET: Generate Assets for Build and Debug"
```

---
---

# :: Operating System ::
---

# IX. Ubuntu
`check Ubuntu version`
```sh
lsb_release -a
```

`search for software to install` `<application>`
```sh
sudo apt search <audacity>
```

`install from cli`
```sh
sudo apt install audacity
```

`killall <-- terminates process`
```sh
killall <snap-store>
```

# X. Windows

`dumbest windows shortcut ever`
`switch entire windows dekstop`
```C#
ctrl + win + right // next (new)
ctrl + win + left // prev (all old)
```

`inside file explorer:`
```C#
ctrl + l   // focus address bar
cmd        // enter cmd to open cmd in this location
powershell // open powershell in this location
```

`anywhere, but useful inside file explorer`
`more options include copy path, open powershell here, open linux shell here`
```C#
shift + right-click // opens menu with more options
```

---
---

# :: Misc. ::
---

# XI. Cron
**For Ubuntu/Debian, you can find `cron`logs at:**
```bash
/var/log/syslog
```

# XII. Postman

`variables created/stored in "Environments" in postman can be passed into fields using {{}}`
```sh
Client ID: {{google_client_id}}
Client Secret: {{google_client_secret}}
```

```bash
grep nri // <--
```

`To get a list of all listening TCP ports using lsof`
```bash
sudo lsof -nP -iTCP -sTCP:LISTEN
```

`using ss tool (formerly netstat) to list all open ports`
```bash
ss -tulpn
```

#  XII. Tree

`tree [OPTIONS] [directory]` ("`.`" might not be necessary)
`List folder structure only directories from current directory`
```sh
tree -d .
```

`List folder structure only directors at depth 1`
```sh
tree -d -L 1 .
```

`List folder structure and all hidden files`
```sh
tree -a .
```

---

