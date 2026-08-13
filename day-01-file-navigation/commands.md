# Day 1 Commands: Where Am I? Basic Orientation

## 1. pwd

### Syntax
```bash
pwd
What it does

Shows the full path of the directory I am currently working in. I use it when I need to confirm exactly where I am in the Linux filesystem.

2. ls
Syntax
ls
What it does

Lists the files and directories in my current location. It gives me a quick view of what is available in a directory.

3. ls -l
Syntax
ls -l
What it does

Shows directory contents in a detailed long-list format. It gives me more information about each item than a normal ls.

4. ls -a
Syntax
ls -a
What it does

Shows all files and directories, including hidden ones. Hidden files are normally not displayed by a basic ls.

5. ls -la
Syntax
ls -la
What it does

Combines the detailed listing of -l with the hidden-file visibility of -a. I can use it when I want a complete and detailed view of a directory.

6. ls -lh
Syntax
ls -lh
What it does

Shows a detailed directory listing while displaying file sizes in a human-readable format. This makes sizes easier for me to understand.

7. cd (absolute path)
Syntax
cd /var/log
What it does

Moves me directly to a directory using its full path. An absolute path starts from the root of the filesystem, so it does not depend on my current location.

8. cd ..
Syntax
cd ..
What it does

Moves me one level up to the parent directory. I use it when I want to move back toward the directory above my current location.

9. cd ~
Syntax
cd ~
What it does

Takes me directly to my home directory. The ~ symbol represents my home directory.

10. cd -
Syntax
cd -
What it does

Takes me back to the previous directory I was working in. It is useful when I need to switch between two locations.