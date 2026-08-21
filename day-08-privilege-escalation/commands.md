# Day 8 Commands – Privilege Escalation & Identity

### 1. `sudo`
**Syntax:** `sudo command`  
**What it does:** Runs a single command with root privileges.  
**When I use it:** When a normal command fails because of permission denied.

### 2. `sudo -i`
**Syntax:** `sudo -i`  
**What it does:** Opens a full root shell (like logging in as root).  
**When I use it:** When I need to run many commands as root.

### 3. `sudo -u`
**Syntax:** `sudo -u username command`  
**What it does:** Runs a command as a different user.  
**When I use it:** When I need to run something as another specific user.

### 4. `sudo !!`
**Syntax:** `sudo !!`  
**What it does:** Re-runs the previous command with `sudo`.  
**When I use it:** When I forget to type `sudo` and get a permission error.

### 5. `visudo`
**Syntax:** `sudo visudo`  
**What it does:** Safely edits the sudoers file (the file that controls sudo permissions).  
**When I use it:** When I need to give or remove sudo access for a user.

### 6. `su`
**Syntax:** `su`  
**What it does:** Switches to another user (usually root) while keeping the current environment.  
**When I use it:** Quick switch to another account.

### 7. `su -`
**Syntax:** `su -`  
**What it does:** Switches to another user with a full login environment.  
**When I use it:** Better way to become root or another user.

### 8. `whoami`
**Syntax:** `whoami`  
**What it does:** Shows the current username.  
**When I use it:** To confirm which user I am currently logged in as.

### 9. `sudo -l`
**Syntax:** `sudo -l`  
**What it does:** Lists the sudo privileges available to my account.  
**When I use it:** To see exactly which commands I am allowed to run with sudo.

### 10. `id`
**Syntax:** `id`  
**What it does:** Shows my user ID, group ID, and all groups I belong to.  
**When I use it:** To check my full identity and group memberships.