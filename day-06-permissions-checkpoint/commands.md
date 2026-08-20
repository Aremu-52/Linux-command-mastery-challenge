Day 6 — Command Journal
1. ls -l
Purpose

Displays detailed information about files and directories, including their permission string.

Example
ls -l script.sh

The permission string can look like:

-rwxr-xr-x
2. chmod — Relative Permissions
Purpose

Adds or removes specific permissions.

Example
chmod u+rwx,g+rx,o+rx script.sh

Where:

u = user/owner
g = group
o = others
+ = add permission
3. chmod — Assignment Permissions
Purpose

Sets the permissions for the specified users exactly.

Example
chmod u=rwx,g=rx,o=rx script.sh
4. chmod 755
Purpose

Sets permissions using octal notation.

chmod 755 script.sh

The permission breakdown is:

7 = rwx
5 = r-x
5 = r-x

Therefore:

755 = rwxr-xr-x
5. chmod 644
Purpose

Sets permissions to:

rw-r--r--
Example
chmod 644 file.txt
6. chmod 600
Purpose

Sets permissions to:

rw-------
Example
chmod 600 file.txt
7. chmod -R
Purpose

Applies a permission change recursively to a directory and its contents.

Example
chmod -R 755 permissions-test
8. umask
Purpose

Displays the current default permission mask.

Example
umask
9. umask -S
Purpose

Displays the current umask using symbolic permission notation.

Example
umask -S
10. stat -c '%A %U %G'
Purpose

Displays the permissions, owner, and group of a file.

Example
stat -c '%A %U %G' script.sh

The format codes are:

%A = permissions
%U = owner
%G = group
Permission Reference
4 = read
2 = write
1 = execute

Therefore:

7 = 4+2+1 = rwx
6 = 4+2   = rw-
5 = 4+1   = r-x
4 = 4      = r--
0 =          ---