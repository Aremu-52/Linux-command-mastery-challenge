# Day 3 — Reading & Inspecting Files

## Objective

Learn how to read, inspect, count, and monitor the contents and metadata of files using Linux commands.

## Commands Practiced

- `cat`
- `less`
- `head`
- `head -n`
- `tail`
- `tail -n`
- `tail -f`
- `wc`
- `wc -l`
- `file`
- `stat`

## Practical File

For the practical drill, I used:

`/var/log/syslog`

This is a system log file containing records of events and activities on the Ubuntu system.

## What I Practiced

- Viewed the complete log using `cat`
- Paged through the log using `less`
- Displayed the first 15 lines using `head -n 15`
- Displayed the last 15 lines using `tail -n 15`
- Counted the lines using `wc -l`
- Inspected line, word, and byte counts using `wc`
- Identified the file type using `file`
- Inspected detailed file metadata using `stat`
- Followed new log entries in real time using `tail -f`

## Evidence

Screenshots of the practical work are stored in the `evidence/` directory.