# Day 7 Practice Drill

## Task
Create a shared project folder, apply the SGID bit so new files inherit its group, then audit the whole system for unexpected SUID binaries.

## Commands I ran

```bash
mkdir shared-project
cd shared-project
sudo chown $USER:$USER .
sudo chgrp $USER .
sudo chmod g+s .
ls -ld .
touch testfile.txt
ls -l testfile.txt
sudo chmod +t .
getfacl .
sudo setfacl -m u:$USER:rwx .
cd ~
find / -perm /4000 2>/dev/null | head -20