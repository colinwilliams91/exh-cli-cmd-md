```ts
this is a cataloging of commands and shortcuts i have found useful along my coding journey
-
ctrl + f to search for the cli term you are looking for (annotated w/ keywords and descriptions)
-
search using the roman numeral indexed legend for system or technology lookup
```

| Index | Technology         | System           |
| :---: | ------------------ | ---------------- |
|   I   | Visual Studio Code | IDE              |
|  II   | Visual Studio      | IDE              |
|  III  | Bash               | Terminal         |
|  IV   | Powershell         | Terminal         |
|   V   | Command Prompt     | Terminal         |
|  VI   | Oh My Zsh!         | Terminal         |
|  VII  | Node               | Framework        |
| VIII  | .Net               | Framework        |
|  IX   | CSS                | Framework        |
|   X   | Ubuntu             | Operating System |
|  XI   | Windows            | Operating System |
|  XII  | SQL                | DB               |
| XIII  | Cron               | Misc.            |
|  XIV  | Postman            | Misc.            |
|  XV   | Tree               | Misc.            |
|  XVI  | Git                | Misc.            |

---
---

# :: IDE ::
---

# I. VSCode
`command palette`
```ts
ctrl + shift + p
```

`enable psehll integrated terminal enhancements (preferences settings json)`
```ts
"terminal.integrated.suggest.enabled": true
```

`ScreenCast Mode (great for presentations)`
```ts
ctrl + shift + p
// type "screencast"
// select Developer Toggle Screencast Mode
```

`Clear command suggestions for integrated terminal (for powershell can reduce time to activate shell from ~600ms -> ~50ms`
```ts
ctrl + shift + p
Terminal: Clear Suggest Cache
```

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

`search file explorer`
```ts
ctrl + p
```

`focus terminal`
```ts
ctrl + `
```

`focus source control view`
```sh
ctrl + shift + g
```

`check for changed settings`
```ts
ctrl + shift + p // cmd palette
// search by "@modified"
// this will filter only settings
// you have made changes to
```

`inside terminal to do "reverse lookup history" (commands entered)`
```ts
ctrl + r
```

`open/close sidebar`
```ts
ctrl + b
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

`copy file relative path`
```ts
ctrl + k, ctrl + shift + c
```

`go to line #`
```ts
ctrl + shift + p
:# 
// backspace the > then :number
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

`replace all occurrences in the open file`
```typescript
ctrl + h
```

`ctrl + K + M` --> "change language mode" --> JSON to format JSON stringified object grabbed from browser

`JavaScript Console Debugging`
```js
console.log({object}) /* will print as console.log("object:": { ... }); */  
  
console.dir(object, {depth: null}) /* will print all of the data rather than compared to console.log which only returns top level, not nested data */
```

# II. Visual Studio

`run application`
```sh
ctrl + fn + f5 # <<-- default run
fn + f5 # <<-- debug run (slower)
```

`build project`
```C#
ctrl + shift + b
```

`open breakpoints window`
```C#
ctrl + alt + b
```

`open terminal (View.Terminal) shortcut added`
```sh
ctrl + shift + t
```

`quick launch`
```sh
ctrl + q # search commands keywords e.g: "new"
```

`extract code snippet to new Method`
```C#
// highlight target code
ctrl + r, ctrl + m
// this will move the highlighted code to a new method with this signature:

// private void NewMethod()
// the targeted code will be the body of this new method
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

`link proj dependencies, link proj as reference`
```C#
cd \IntoProj
dotnet add reference ..\ParentProj\Proj.csproj
// find the .csproj level to link
// requires dotnet sln command to be complete..
```

`link VS solution files dotnet sln`
```C#
cd .. // cd to root or whatever .sln level you want to link to
dotnet sln add YourProj\WithSolution.csproj
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

`search file name`
```sh
ctrl + , # type name of file to find
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

`navigate back to prev window`
```sh
ctrl + -
```

`find closing brace`
```sh
ctrl + ]
```

`open toolbox`
```sh
ctrl + alt + x
```

`multi cursor edit (also in Edit menu)`
```C#
ctrl + alt + click // add 2nd caret
ctrl + alt + dbl-click // add 2nd word selection
ctrl + alt + click + drag // add 2nd selection
shift + alt + . // add next matching text
shift + alt + ; // add all matching text
shift + alt + , // rm last selected occurence
shift + alt + / // skip next matching occurence
alt + click // add a box selection
esc OR click // clear all selections
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

`open Test Explorer`
```sh
ctrl + e, t
```

`run tests`
```C#
ctrl + r, t // runs selectred
ctrl + r, a // runs all tests
ctrl + r, l // "repeat last run"
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

### Unity in VS

`view Unity Project Explorer`
```c#
alt + shift + e
// filters sln/proj to unity files
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

`get current path`
```powershell
(Get-Item .).FullName
```

`pipe to clipboard`
```powershell
(Get-Item .).FullName | Set-Clipboard
```

`run cmd prompt in pshell`
```C#
cmd  // starts cmd prompt in window
exit // returns to pshell in window
```

```
run "external commands" like .bat or .cmd, executables (.exe) or non-native cmdlets and command-line tools (like in your PATH or full pathed)... 
```
`&` call operator
```C#
& notepad.exe
& calc.exe

& "C:\Path\To\SomeExecutable.exe"
```

`run single cmd prompt command in pshell`
```C#
cmd /c <command>
// e.g.
cmd /c dir // like ls
cmd /c set # displays your system env
cmd /c set > file_name.txt // like cat
```

`list all running processes w/ binary program names`
```powershell
netstat -ba # will require elevated perm
netstat -ban # this will also show IPs
```

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

`create a symbolic link shortcut to path`
```powershell
New-Item -itemtype symboliclink -Path "PathWhereYouWantToPutShortcut" -name "NameOfShortcut" -value "PathOfWhatYourTryingToLinkTo"
```

`start transcript of entire session to local file`
```powershell
Start-Transcript
Stop-Transcript # stop when done
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

`Rename directory (like bash mv)`
```powershell
Rename-Item "D:\temp\Test Test1"
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
ni example.txt -type file
```

`append to file`
```powershell
"content to add" | add-content -path .\README.md
# OR
"content to add" >> .\README.md
```

`overwrite file contents`
```powershell
"overwrite stuff" > .\README.md
```

`string literals vs evaluation`
```powershell
'Hello $ man' # doesn't evaluate special characters or anything
"../blob/$Version" # $Version is evaluated as a variable expression
```

`delete recursive rm -rf`
```C#
Remove-Item -Recurse -Force <path>
```

`move item(s)`
```powershell
Move-Item -Path .\whatever\files -Destination .\destination -force
```

`copy item(s) -recurse if folder`
```powershell
Copy-Item -Path .\the\files -Recurse -Destination .\the\destination -force
```

# V. Command Prompt

`display directory contents`
```C#
dir // <<-- windows/cmd version of `ls`
```

`display system env`
```C#
set
```

`write env to file`
```C#
set > file_name.txt
```

`pipe to clipboard`
```C#
// ... | clip
where pip3 | clip
```

`initiate reboot ("windows terminal")`
```cmd
shutdown /r /t 0
(this might only work in windows terminal)
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

`push package to nuget.org`
```C#
dotnet nuget push <.\path\to\packed.1.0.0.nupkg> --api-key <abcdef12345> --source https://api.nuget.org/v3/index.json
```

**(VSCODE)**
`generate assets for build and debug`
```C#
ctrl + shift + p // cmd pallette
// enter ".net: g"
// select ".NET: Generate Assets for Build and Debug"
```

`CSS Caching with ASP.NET`
```html
<!-- tick disable browser cache in browser dev tools... and/or... -->
<!-- in html markup (razor or w/e framework working w/ .NET)... -->
<link rel="stylesheet" href="~/css/site.css" asp-append-version="true">
<!-- asp-append-version="true" will append a new version ID to the css file that is compiled down... -->
 <!-- ...this ensures proper caching on changes to source -->
```

# IX. CSS
`copy css class declarations from web browser`
```css
/* When inspecting and adjusting CSS in browser dev tools... */
/* ...highlight all class declarations you made... */
/* ...right click and select "copy all declarations" */
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

`turn on/off windows features`
```C#
Control Panel > Programs > Programs and Features > Turn Windows featrures on or off
```

`telnet "allows connecting to other computers remotely"`
```C#
// In "Turn Windows features on or off"
// ... check the Telnet box
[x] Telnet
```

`Use Telnet to check the port`
```powershell
telnet <address> <port_number>
telnet google.com 80
```

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
# :: Databases ::
---
### MS SQL Server

`FIND COLUMNT in DB`
```SQL
SELECT * FROM information_schema.columns WHERE column_name = 'My_Column'
```

`SELF REFERENCING TABLE`
```SQL
SELECT a.something, b.other
FROM mytable a, mytable b
WHERE a.sometest val ...
AND b.othertest val...
```

`WHEN to clean up CURSOR`
```SQL
IF CURSOR_STATUS('local', 'X') >= -1
BEGIN
    CLOSE X;
    DEALLOCATE X
END;
```

`list all schemas in DB`
```SQL
SELECT name FROM sys.schemas
-- dbo -> [dbo].table
-- lu  -> [lu].table
-- etc
```
### SSMS

`fix SSMS won't see new objects/tables`
```SQL
Edit > Intellisense > Refresh Local Cache
OR
ctrl + shift + r
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

# XIV. Git
`tagging commits, usually for release`
```bash
git tag -l # the -l (list) flag is opt
# lists all current tags
git tag v1.0.0 2261e84e
# tags a commit by sha
git tag v1.0.1
# tags your current commit
git tag -a v1.0.2 -m "annotate this tag"
# -a flag for annotate -m for message

git show v1.0.0
# this will show associated commit

git log --pretty=oneline
# shows all commits pretty

git push origin --tags
# this will push all tags that aren't already on the remote up
```

`if you have changes on your remote that you didn't mean to track:`
`add dir and/or files to .gitignore`
`then use this command to remove from the index (the actual location in <baseOfRepo>/.git/index which is your staging area)`
```bash
git rm --cached put/here/your/file.ext # for files
git rm --cached folder/\* # for directory of files
# append --dry-run # to see what will happen w/o executing
git push ... # to update removal and untrack to remote
```
`CAUTION: i have only used this on auto-generated files, so i safely know they will be recreated locally upon deletion...`
`proceed with caution by backing up files if this is not the case for you...`

`bring committed changes back to working directory (e.g. for committed files you want to stash that have not been pushed`
```bash
git reset HEAD~1 --soft
```

`probably best reset option. discard 2 of 3 git areas`
```bash
git reset --mixed
# discards commit and staged changes (in the git index) but KEEPS changes in your working dir (files in IDE)
```

`show remote repo branches state compared with local branches`
```bash
# git remote show <remote alias>
git remote show origin
```

`git add --patch "hunks"`
```bash
git add -p # shows hunks diff in CLI
```

`tool for giff from all commits on current branch`
```shell
gitk --all
```

`switch to FILE and discard changes (destructive)`
```bash
git restore
```

`move between branches (replaces checkout) doesn't discard changes`
```bash
git switch # only takes branch as arg
# checkout is for switching tags and commits
```
#### Rebase
`how to proceed in interactive rebase`
```bash
# git rebase -i or something
# once you decide the strategy for rebasing (specific files squash, pick, reword, etc)
# then how to continue after handling merge conflicts and whatnot
git add README.txt && git rebase --continue
```

---

