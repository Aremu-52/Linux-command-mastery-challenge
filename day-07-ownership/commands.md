# Day 7 Commands – Ownership & Special Bits

### 1. `chown`
**Syntax:** `chown new_owner filename`  
**What it does:** Changes the owner of a file or directory.  
**When I use it:** When I need to transfer ownership of a file to another user.

### 2. `chown user:group`
**Syntax:** `chown user:group filename`  
**What it does:** Changes both the owner and the group of a file or directory at the same time.  
**When I use it:** This is the most common form I use when setting ownership.

### 3. `chown -R`
**Syntax:** `chown -R user:group foldername`  
**What it does:** Changes ownership recursively for a directory and everything inside it.  
**When I use it:** When I need to fix ownership of an entire project folder.

### 4. `chgrp`
**Syntax:** `chgrp newgroup filename`  
**What it does:** Changes only the group of a file or directory.  
**When I use it:** When the owner is already correct and I only need to change the group.

### 5. `chmod u+s` (SUID)
**Syntax:** `chmod u+s filename`  
**What it does:** Sets the Set User ID bit so the program runs with the permissions of the file owner.  
**When I use it:** On special programs that need temporary elevated privileges (example: `passwd`).

### 6. `chmod g+s` (SGID)
**Syntax:** `chmod g+s foldername`  
**What it does:** On a directory, new files automatically inherit the group of that directory.  
**When I use it:** On shared project folders so team members get the correct group automatically.

### 7. `chmod +t` (Sticky Bit)
**Syntax:** `chmod +t foldername`  
**What it does:** Prevents users from deleting files they do not own, even if they have write permission on the directory.  
**When I use it:** On shared directories such as `/tmp`.

### 8. `find -perm /4000`
**Syntax:** `find / -perm /4000 2>/dev/null`  
**What it does:** Searches the system for files that have the SUID bit set.  
**When I use it:** During security audits to find programs that can run with elevated privileges.

### 9. `getfacl`
**Syntax:** `getfacl filename`  
**What it does:** Displays the Access Control List (extra permissions) of a file or directory.  
**When I use it:** When I need to see advanced permissions beyond the normal owner/group/others.

### 10. `setfacl -m`
**Syntax:** `setfacl -m u:username:rwx filename`  
**What it does:** Sets or modifies Access Control Lists for a specific user or group.  
**When I use it:** When I need to give special permission to one user without changing the main ownership.