```markdown
# Day 4 Practice Drill

## Objective

Use Linux filesystem search and disk-usage commands to investigate a real Ubuntu system

## Task 1 Find Configuration Files

I searched for all `.conf` files under `/etc`.

### Command

```bash
sudo find /etc -name "*.conf"
Result

The command returned configuration files located in different directories under /etc.

I initially encountered a Permission denied message when searching a protected directory. Using sudo allowed the search to access the protected location.

Task 2 — Find Files Larger Than 1 MB

I searched /var for regular files larger than 1 MB.

Command
sudo find /var -type f -size +1M
Result

The command searched /var and returned files that matched the specified size condition.

Task 3 — Check Total Disk Usage of /home

I checked how much disk space the /home directory was using.

Command
du -sh /home
Result

The command displayed the total disk usage of /home in a human-readable format.

Task 4 — Check Free Space on the Root Filesystem

I checked the available disk space on the filesystem containing /.

Command
df -h /
Result

The command displayed the total, used, available, and percentage-used space for the root filesystem.

Additional Practice

During the Day 4 practical, I also practiced:

find /etc -type f
find /etc -type f -mtime -1
find ~/linux-command-mastery-challenge -type f -perm 644
locate passwd
sudo updatedb
du /home
df -h
What I Learned

This drill helped me understand how Linux administrators can locate files, investigate filesystem contents, identify large files, check file permissions, and monitor available storage.

I also learned that permissions can affect filesystem searches and that sudo may be required when inspecting protected system directories.



