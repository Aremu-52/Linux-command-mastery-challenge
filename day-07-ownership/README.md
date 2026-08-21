# Day 07: Ownership & Special Bits

**Phase 2 – Permissions, Ownership & Security | Day 7 of 30**

## Commands covered today
See [commands.md](./commands.md) for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.

## What I practiced
I created a shared project folder, applied the SGID bit so that new files inherit the group of the folder, and audited the system for SUID binaries using `find -perm /4000`.

## What surprised me
I was surprised that after setting the SGID bit, any new file I created inside the folder automatically inherited the correct group without me having to change it manually.

## Evidence
Screenshot of the practice drill is stored in the [evidence](./evidence/) folder.

## Related
- Previous day: [day-06-permissions-checkpoint](../day-06-permissions-checkpoint/)
- Next day: [day-08-privilege-escalation](../day-08-privilege-escalation/)