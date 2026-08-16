# Day 4 — Filesystem Search & Disk Usage

## Objective

Learn how to search for files and directories, identify files by different properties, and inspect disk usage on a Linux system.

## Commands Practiced

- `find -name`
- `find -type`
- `find -size`
- `find -mtime`
- `find -perm`
- `locate`
- `updatedb`
- `du`
- `du -sh`
- `df -h`

## Practical Work

For this day's practical exercises, I worked with directories including:

- `/etc`
- `/var`
- `/home`
- `/`

I searched for configuration files, identified files based on type, size, modification time, and permissions, used `locate` to search the filesystem database, and checked disk usage and available storage.

## Key Lessons

I learned that different Linux commands answer different filesystem questions.

- `find` provides flexible real-time filesystem searches.
- `locate` provides fast searches using a database.
- `updatedb` updates the database used by `locate`.
- `du` shows how much disk space files and directories are using.
- `df` shows available and used filesystem space.

## Permission Issue Encountered

While searching `/etc`, I initially received a `Permission denied` message when `find` reached a protected directory.

I resolved this by using `sudo`:

```bash
sudo find /etc -name "*.conf"

This helped me understand that Linux permissions affect filesystem searches.

The evidence/ directory contains screenshots from the practical exercises.