Day 5 — Links, Paths & Tree Structures
Objective

Learn how to work with filesystem paths, directory trees, hard links, symbolic links, and directory navigation tools in Linux.

Commands Practiced
tree
tree -L
ln
ln -s
readlink
realpath
basename
dirname
pushd
popd
ls -lt
Practical Work

During this exercise, I worked with Linux filesystem paths and created both hard and symbolic links.

I created a symbolic link to /etc/hosts and used readlink and realpath to inspect and resolve the link.

I also created a hard link and compared the inode numbers of the original file and hard link using ls -li.

Hard Link vs Symbolic Link

A hard link is another directory entry referring to the same underlying file and inode.

A symbolic link is a separate link that points to the path of another file or directory.

Hard Link
ln original.txt hardlink.txt
Symbolic Link
ln -s /etc/hosts hosts-link
Key Lessons
tree displays directory structures visually.
ln creates hard links.
ln -s creates symbolic links.
readlink shows the target of a symbolic link.
realpath resolves a path to its absolute path.
basename extracts the final component of a path.
dirname extracts the directory component.
pushd and popd help manage directory navigation.
ls -lt displays files sorted by modification time.
Evidence

Screenshots from the practical exercises are stored in the evidence/ directory.