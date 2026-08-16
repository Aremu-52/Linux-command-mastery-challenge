```markdown
# Day 4 — Command Journal

## 1. find -name

### Purpose

Searches for files or directories based on their names.

### Example

```bash
sudo find /etc -name "*.conf"
What I Learned

find -name is useful when I know the name or extension of the files I am looking for.

2. find -type
Purpose

Searches for items based on their type.

Example
find /etc -type f
What I Learned

-type f searches for regular files, while -type d searches for directories.

3. find -size
Purpose

Searches for files based on their size.

Example
sudo find /var -type f -size +1M
What I Learned

This can be used to locate files that are larger than a specified size.

4. find -mtime
Purpose

Searches for files based on their modification time.
Example
find /etc -type f -mtime -1
What I Learned

-mtime is useful for finding files that were modified recently or a certain number of days ago.

5. find -perm
Purpose

Searches for files with specific permissions.

Example
find ~/linux-command-mastery-challenge -type f -perm 644
What I Learned

-perm can be used to locate files based on their permission settings.

6. locate
Purpose

Quickly searches for files using a database of file locations.

Example
locatepasswd
What I Learned

locate is usually faster than find because it searches a database instead of scanning the filesystem directly.

7. updatedb
Purpose

Updates the database used by locate.

Example
sudo updatedb
What I Learned

Running updatedb ensures that newly created files can become available to locate.

8. du
Purpose

Displays disk usage.

Example
du /home
What I Learned

du can show how much disk space directories and their contents are using.

9. du -sh
Purpose

Displays a summary of disk usage in a human-readable format.

Example
du -sh /home
What I Learned

The -s option provides a summary, while -h makes the size easier to read.

10. df -h
Purpose

Displays filesystem disk space usage in human-readable format.

Example
df -h
What I Learned

df -h shows total, used, and available filesystem space.

Important Difference
du

Shows how much space files and directories are using.
du -sh /home
df

Shows filesystem capacity and how much space is available.

df -h