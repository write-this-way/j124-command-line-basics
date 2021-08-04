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

**How do I get into a specific file directory on the command line? **
1. Open Finder. Click on the folder you want to open in terminal.
2. Click `Ctrl + C` to copy the name of the folder to the clipboard.
3. Open a terminal window. After the `%`, type `cd` and click the space once. Then click `Ctrl + C` to paste in the name of the folder.
4. Click `Return`. 
5. Look at the file location listed before the `%`. It should be the name of the folder you pasted in. Type `pwd` to confirm where you are in the file structure.

**What does a terminal window look like?**
Regardless of which operating system you use, your terminal window should look something like this.

!['Terminal','Terminal window screenshot'](/terminal.png)

Every command line starts with some symbol or symbols designed to “prompt” you to action. The prompt usually ends with a `$` or a `%`, and is preceded by information that depends on the details of your system. For example:

!['Prompt','Terminal window prompt screenshot'](/prompt.png)



