Day 6 — Practice Drill
Objective

Create a script file and set its permissions to rwxr-xr-x using three different chmod methods.

Step 1 — Create the Script
touch script.sh
Step 2 — Relative chmod Method

Set the permissions using the relative + method:

chmod u+rwx,g+rx,o+rx script.sh

Confirm the result:

ls -l script.sh

Expected permission:

-rwxr-xr-x
Step 3 — Assignment chmod Method

Set the permissions using the assignment method:

chmod u=rwx,g=rx,o=rx script.sh

Confirm the result:

ls -l script.sh

Expected permission:

-rwxr-xr-x
Step 4 — Octal chmod Method

Set the permissions using octal notation:

chmod 755 script.sh

Confirm the result:

ls -l script.sh

Expected permission:

-rwxr-xr-x
Step 5 — Recursive Permissions

Create a test directory and file:

mkdir permissions-test
touch permissions-test/test.txt

Apply permissions recursively:

chmod -R 755 permissions-test

Verify:

ls -l permissions-test
Step 6 — Check umask

Display the current umask:

umask

Display it in symbolic form:

umask -S
Step 7 — Verify Permissions and Ownership

Run:

stat -c '%A %U %G' script.sh

This verifies:

File permissions
File owner
File group
Result

The script was successfully assigned:

rwxr-xr-x

using:

Relative chmod
Assignment chmod
Octal chmod 755

The results were confirmed using ls -l.