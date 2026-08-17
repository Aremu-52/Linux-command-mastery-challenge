Day 5 — Command Journal
1. tree
Purpose

Displays files and directories in a tree-like structure.

Example
tree
2. tree -L
Purpose

Limits how many directory levels tree displays.

Example
tree -L 2 /etc
3. ln
Purpose

Creates a hard link to an existing file.

Example
ln original.txt hardlink.txt
What I Learned

A hard link points to the same underlying file and inode as the original file.

4. ln -s
Purpose

Creates a symbolic link.

Example
ln -s /etc/hosts hosts-link
What I Learned

A symbolic link points to another file or directory by path.

5. readlink
Purpose

Displays the target of a symbolic link.

Example
readlink hosts-link
Result
/etc/hosts
6. realpath
Purpose

Displays the absolute path of a file or link.

Example
realpath hosts-link
7. basename
Purpose

Extracts the final part of a path.

Example
basename /etc/hosts
Result
hosts
8. dirname
Purpose

Extracts the directory portion of a path.

Example
dirname /etc/hosts
Result
/etc
9. pushd / popd
Purpose

Temporarily changes directories while maintaining a directory stack.

Example
pushd /etc
popd
10. ls -lt
Purpose

Displays files in long format and sorts them by modification time.

Example
ls -lt
Hard Link vs Symbolic Link
Hard Link
ln original.txt hardlink.txt

The hard link refers to the same underlying file and inode.

Symbolic Link
ln -s original.txt softlink.txt

The symbolic link points to the original file's path.