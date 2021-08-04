# J124 Command Line Basics
Command line cheatsheet for Intro to Data Journalism class

| Command          | Description                       | Example                 |
|------------------|-----------------------------------|-------------------------|
| `>`              | Redirect output to filename       | `$ echo foo > foo.txt`  |
| `>>`             | Append output to filename         | `$ echo bar >> foo.txt` |
| `cat <file>`     | Print contents of file to screen  | `$ cat hello.txt`       |
| `ls`             | List directory or file            | `$ ls hello.txt`        |
| `ls -a`          | List all (including hidden files) | `$ ls -a`               |
| `touch <file>`   | Create an empty file              | `$ touch foo`           |
| `mv <old> <new>` | Rename (move) from old to new     | `$ mv foo bar`          |
| `cp <old> <new>` | Copy old to new                   | `$ cp foo bar`          |
| `rm <file>`      | Remove (delete) file              | `$ rm foo`              |
| `rm -f <file>`   | Force-remove file                 | `$ rm -f bar`           |
| `pwd`            | Present working directory         | `$ pwd`                 |
| `clear`          | Clear contents of terminal window | `$ clear`               |

*Pro tip: Use a [table generator](https://www.tablesgenerator.com/markdown_tables#) to make a table this large and complex in Markdown.*

**How do I find the command line on my computer?**

*macOS*
You can open a terminal window using the macOS application Spotlight, which you can launch either by typing ⌘␣ (Command-space) or by clicking on the magnifying glass in the top right corner of your screen. Once you’ve launched Spotlight, you can start a terminal program by typing “terminal” in the Spotlight search bar. Click `Return` to open the Terminal application.

*Windows*
The recommended option is to install Linux (which, Microsoft supports natively). Once Linux is installed, you should look for a terminal icon in your menubar. Click the icon to launch a terminal window.

**How do I get into a specific file directory on the command line (on a Mac)?**
1. Open Finder. Click on the folder you want to open in terminal.
2. Click `Command + C` to copy the name of the folder to the clipboard.
3. Open a terminal window. After the `%`, type `cd` and click the space once. Then click `Command + C` to paste in the name of the folder.
4. Click `Return`. 
5. Look at the file location listed before the `%`. It should be the name of the folder you pasted in. 

**Where am I?** <br>
Type `pwd` to confirm where you are in the file structure.

**What files are in my directory?** <br>

`$ ls` 
Long listing of all the files and directories in the current directory *except* for those that are hidden.

`$ ls -a`
Long listing of all the files and directories in the current *including* those that are hidden. 

Unix has the concept of “hidden files (and directories)”, which don’t show up by default when listing files. Hidden files and directories are identified by starting with a dot ., and are commonly used for things like storing user preferences.

```
$ ls -a
.           .gitignore      sonnet_1_reversed.txt
..          sonnet_1.txt
```

The `ls` command can be used to check if a file (or directory) exists, because trying to `ls` followed by a nonexistent file name results in an error message,

**What does a terminal window look like?** <br>
Regardless of which operating system you use, your terminal window should look something like this.

!['Terminal','Terminal window screenshot'](/terminal.png)

Every command line starts with some symbol or symbols designed to “prompt” you to action. The prompt usually ends with a `$` or a `%`, and is preceded by information that depends on the details of your system. For example:

`danaamihere@MacBook-Pro / %`

### Getting started with command line <br>
If your in the file location you want to be in, you're ready to run commands.

**Print a statement** <br>
Print *hello, goodbye*

```
$ echo hello, goodbye
hello, goodbye
$ echo "hello, goodbye"
hello, goodbye
$
```

**Uh-oh...** <br>
What happens if there the quotation marks aren't matched in my command?

```
$ echo "hello, goodbye
>
```

At this point, it seems we’re stuck. You can get out of trouble by clikcing `Ctrl + C`.

**Redirecting and appending** <br>
Let's start with some text. We'll use the first line of Shakespeare’s first sonnet to work with.

```
$ echo "From fairest creatures we desire increase,"
From fairest creatures we desire increase,
```
Create a file containing this line. You can do this without a text editor using the redirect operator, `>`.

`$ echo "From fairest creatures we desire increase," > sonnet_1.txt`

Did our command work? Use the `cat` command. The name `cat` is short for “concatenate”, which is a hint that it can be used to combine the contents of multiple files, but it can also be used as a “quick-and-dirty” way to dump the contents of a single file to the screen. 

```
$ cat sonnet_1.txt
From fairest creatures we desire increase,
```

In order to add the second line of the sonnet (in modernized spelling), we can use the append operator >>
`$ echo "That thereby beauty's Rose might never die," >> sonnet_1.txt`

And here's the result: 
```
$ cat sonnet_1.txt
From fairest creatures we desire increase,
That thereby beauty's Rose might never die,
```
