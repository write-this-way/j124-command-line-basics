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
| `pwd`            | Present working directory         | `$ pwd`           |

*Pro tip: Use a [table generator](https://www.tablesgenerator.com/markdown_tables#) to make a table this large and complex in Markdown.*

####The following instructions are for Mac OS.

**How do I get into a specific file directory on the command line? **
1. Open Finder. Click on the folder you want to open in terminal.
2. Click `Ctrl + C` to copy the name of the folder to the clipboard.
3. Open a terminal window. After the `%`, type `cd` and click the space once. Then click `Ctrl + C` to paste in the name of the folder.
4. Click `Enter`. 
5. Look at the file location listed before the `%`. It should be the name of the folder you pasted in. Type `pwd` to confirm where you are in the file structure.
