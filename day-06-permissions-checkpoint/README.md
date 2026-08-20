Day 6 — Permissions Checkpoint
Objective

Learn how to read, modify, and verify Linux file permissions using ls -l, chmod, umask, and stat.

Commands Practiced
ls -l
chmod using relative permissions
chmod using assignment
chmod 755
chmod 644
chmod 600
chmod -R
umask
umask -S
stat -c '%A %U %G'
Permission Structure

Linux permissions are represented using three groups:

rwx r-x r-x
│   │   │
│   │   └── Others
│   └────── Group
└────────── Owner

Where:

r = read
w = write
x = execute

The target permission used in the practical was:

rwxr-xr-x

This corresponds to:

755
Practical Exercise

I created a script file called script.sh and changed its permissions to rwxr-xr-x using three different chmod methods.

Relative Method
chmod u+rwx,g+rx,o+rx script.sh
Assignment Method
chmod u=rwx,g=rx,o=rx script.sh
Octal Method
chmod 755 script.sh

After each method, I used ls -l script.sh to confirm the resulting permissions.

Recursive Permissions

I created a test directory and applied permissions recursively:

chmod -R 755 permissions-test

The -R option applies the permission change recursively to the directory and its contents.

Umask

I checked the current default permission mask using:

umask

and:

umask -S
Permission and Ownership Verification

I used:

stat -c '%A %U %G' script.sh

to display the file's permissions, owner, and group.

Key Lessons
ls -l can be used to inspect file permissions.
chmod can modify file permissions.
Relative permissions use + and -.
Assignment permissions use =.
Octal permissions such as 755, 644, and 600 provide a compact way to set permissions.
chmod -R applies permissions recursively.
umask controls the default permission mask for newly created files and directories.
stat can be used to inspect permissions and ownership.
Evidence

The practical evidence is stored in the evidence/ directory.