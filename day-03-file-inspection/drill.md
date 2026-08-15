# Day 3 — Practice Drill

## Log File Used

`/var/log/syslog`

## Tasks Completed

### 1. View the complete log

Used:

```bash
cat /var/log/syslog

2. Page through the log

Used:
less /var/log/syslog

and existed using q

3. Show the first 15 lines

Used: 
head -n 15 /var/log/syslog

4. Show the last 15 lines

Used: 
tail -n 15 /var/log/syslog

5. Count the lines

Used:
wc -l /var/log/syslog

6. Display lines, words, and bytes

Used:
wc /var/log/syslog

7. Identify the file type

Used:
file /var/log/syslog

8. Inspect file metadata

Used:
stat /var/log/syslog

9. Follow the log in real time

Used:
tail -f /var/log/syslog

Stopped with:
Ctrl + C

What I Learned

This practical helped me understand how Linux commands can be used to inspect files from different perspectives. I learned how to read complete files, navigate large files, inspect specific sections, count contents, identify file types, examine metadata, and monitor log files in real time.
