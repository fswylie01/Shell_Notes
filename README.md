# Shell_Notes
All the basic shell commands



1. Shell Workshop
- Simple video about the Shell
- Use the shell command line for your computer to run & interact with programs.

2. Windows: Installing Git Bash
- This section is for Windows-only!  Mac and Linux users, skip ahead to the next page.

3. Opening a Terminal
- Mac Terminal - Open terminal window - Command + space bar, type terminal
- The terminal is just an interface to the shell.
- Every terminal program has a number of settings you can adjust.
- You can open up many terminals at once.

4. Your First Command (echo)
- Open the terminal window and you will see the following:

Last login: Tue Oct  3 19:08:48 on console
Franks-MacBook-Air:~ frankwylie$
- This is the shell prompt with a simple message provided above.

A. First Shell Command - echo
- The Echo will print a message back to the user.
Franks-MacBook-Air:~ frankwylie$ echo 'Hello, Frank!'
- It will print the following:  Hello, Frank!
- Use single quotes or it will be printed multiple times.

B. What size is your terminal window?
Franks-MacBook-Air:~ frankwylie$ echo $COLUMNS x $LINES
128 x 37
Franks-MacBook-Air:~ frankwylie$

5. Navigating Directories (ls, cd, ..)
- Command ls - used to print the contents of the current directory
- Command cd - used to change directory

Which of these would list the contents of the Pictures directory?
a. ls Pictures - this is the most direct way to do it.
b. cd Pictures; ls - changes the directory to the Pictures subdirectory, then runs ls in that directory
c. ls Pictures/../Pictures - this is unnecessarily verbose, but it does also work.

Note: If you want to GO BACK a directory then use....  cd.. or cd..; ls

6. Current Working Directory (pwd)
- Command pwd - stands for print working directory
- The result is known as the PATH and separated with forward / slashes

Franks-MacBook-Air:~ frankwylie$ pwd
/Users/frankwylie
- is the PATH

- Command cd ..  - will go up one directory
- Command ls . - will list the contents of the current directory
- Command ls - will list the contents of the current directory
- Command ls ~ - will provide the home directory (pronounced ls tilda)

7. Parameters & Options (ls -l)
- Command ls -l  - will print out a longer / more detailed list of files
- Command ls -l Documents/*.pdf - will print out all documents ending in (dot) pdf

Q1 - Which pieces of information can you find out from ls -l?
- The name of each listed file or directory
- The date and time that a file was last modified
- The size of a file, in bytes

Q2 - If you wanted to list all the files whose names start with the word bear, how would you do it?
- ls bear*

notes:
ls *.bear - if you wanted all the files that end with bear
ls bear - will only list a file whose name is exactly bear... if there is one
ls * bear * - will list the files is the name bear shows up anywhere

8. Organizing You Files (mkdir, mv)
- Command mkdir  - stands for make a directory
i.e. mkdir Documents/Books

- Command mv  - stands for move

Move Files Individually:
i.e. mv 'Documents/1911 Webster Dictionary.epub' Documents/Books/
> Basically what you want to move and where you want to move it.

Move All Files At The Same Time:
i.e. mv Documents/*.epub Documents/Books
> Basically what you want to move and where you want to move it.

Q - lets say you want to move the epub files back from Documents/Books to Documents.
How can you do this?
- mv 'Documents/Books' Documents
-
-

Ask my mentor about the correct answer!!!

By the way, when you quote something in the shell, you always use straight quotes. This is what you'll get if you type into a terminal window. However, if you copy and paste from a web page or document, you should be really careful to make sure that it hasn't accidentally been written with “curly quotes”. Curly quotes will not work in the shell.

9. Downloading (curl)
- Command curl  - stands for C URL (or see URL) used to get the code from any webpage
i.e. curl 'http://google.com'

RESULT:

<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">

<TITLE>301 Moved</TITLE></HEAD><BODY>

<H1>301 Moved</H1>

The document has moved

<A HREF="http://www.google.com/">here</A>.

</BODY></HTML>

Franks-MacBook-Air:~ frankwylie$

Not enough information, then add a big L,
i.e. curl -L . 'http://google.com' - means to follow the redirects to view the compressed source code.

If you want to download the information to a new file:
i.e. curl -o  google.html -L  'http://google.com'
> this will basically download the source code into a file you want to create.

Q - Enter a shell command to download https://tinyurl.com/zeyq9vc and save it as the file dictionary.txt
- Remember to use the option to follow web redirects

Answer:
curl -o dictionary.txt -L ' https://tinyurl.com/zeyq9vc'

By the way, a lot of URLs have special characters in them, such as the & sign, which have unusual meanings to the shell. That's why I'm always putting these URLs in quotes … even though these particular examples would work without them, it's a good practice to get into.

10. Viewing Files (cat, less)
- Simple video explaining sites on mobile.
- klj

11. Removing Things (rm, redir)
- Simple video explaining sites on mobile.
- kljk

12. Searching & Pipes (grep, wc)
- Simple video explaining sites on mobile.
- kjk

13. Shell & Environment Variables
- Simple video explaining sites on mobile.
- lkljj

14. Startup Files (.bash_profile)
- Simple video explaining sites on mobile.
- kkjkj

15. Controlling The Shell Prompt ($PS1)
- Simple video explaining sites on mobile.
- jkjk

16. Aliases
- Simple video explaining sites on mobile.
- kkjkj

17. Keep Learning!
- Simple video explaining sites on mobile.
- kjkjk
