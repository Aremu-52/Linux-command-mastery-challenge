Day 5 — Practice Drill
Objective

Practise Linux filesystem links, paths, directory trees, and navigation.

Task 1 — Create a Symbolic Link

I created a symbolic link to the /etc/hosts configuration file.

Command
ln -s /etc/hosts hosts-link
Verification
ls -l hosts-link

The output showed:

hosts-link -> /etc/hosts
Task 2 — Resolve the Symbolic Link

I used readlink to display the link target.

readlink hosts-link

Result:

/etc/hosts

I also used:

realpath hosts-link

to resolve the link to its actual path.

Task 3 — Display the /etc Directory Tree

I displayed the /etc filesystem structure up to two levels deep.

tree -L 2 /etc

This helped me understand how directories and files are organised under /etc.

Task 4 — Create and Test a Hard Link

I created a test file:

echo "Day 5 hard link practice" > original.txt

Then created a hard link:

ln original.txt hardlink.txt

I compared their inode numbers:

ls -li original.txt hardlink.txt

The files had the same inode number, demonstrating that both names referred to the same underlying file.

I then removed the original filename and confirmed that the hard link could still access the file's contents.

Task 5 — Path Commands

I practised:

basename /etc/hosts
dirname /etc/hosts
realpath hosts-link

These commands helped me understand the different parts of a filesystem path.

Task 6 — Directory Navigation

I practised:

pushd /etc
popd

This demonstrated how Linux can temporarily move between directories while maintaining a directory stack.

Task 7 — File Modification Order

I used:

ls -lt

to display files in long format, sorted by modification time.

Key Learning

The main concept I learned today was the difference between hard links and symbolic links.

A hard link refers to the same underlying file and inode.

A symbolic link points to another file or directory by its path.

This distinction is important for Linux system administration and DevOps work.