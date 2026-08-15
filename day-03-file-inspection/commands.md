# Day 3 — Command Journal

## 1. cat

### Purpose
Displays the contents of a file.

### Example

```bash
cat /var/log/syslog

What I Learned

cat is useful for quickly viewing the contents of a file, especially when the file is not too large.

2. less
Purpose

Displays a file page by page.

Example
less /var/log/syslog
What I Learned

less is useful for reading large files without flooding the terminal.

3. head
Purpose

Displays the beginning of a file.

Example
head /var/log/syslog
What I Learned

By default, head displays the first 10 lines.

4. head -n
Purpose

Displays a specified number of lines from the beginning of a file.

Example
head -n 15 /var/log/syslog
What I Learned

-n allows me to specify exactly how many lines I want to see.

5. tail
Purpose

Displays the end of a file.

Example
tail /var/log/syslog
What I Learned

By default, tail displays the last 10 lines.

6. tail -f
Purpose

Continuously monitors the end of a file for new entries.

Example
tail -f /var/log/syslog
What I Learned

tail -f is useful for monitoring log files in real time. I used Ctrl + C to stop it.

7. wc
Purpose

Counts lines, words, and bytes in a file.

Example
wc /var/log/syslog
What I Learned

wc provides multiple counts about the contents of a file.

8. wc -l
Purpose

Counts the number of lines in a file.

Example
wc -l /var/log/syslog
What I Learned

wc -l is useful when I only need the total number of lines.

9. file
Purpose

Identifies the type of a file.

Example
file /var/log/syslog
What I Learned

file helps identify what kind of data a file contains.

10. stat
Purpose

Displays detailed information and metadata about a file.

Example
stat /var/log/syslog
What I Learned

stat provides information such as file size, permissions, ownership, inode, and timestamps.