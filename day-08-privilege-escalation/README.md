# Day 08: Privilege Escalation & Identity

**Phase 2 – Permissions, Ownership & Security | Day 8 of 30**

## Commands covered today
See [commands.md](./commands.md) for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.

## What I practiced
I attempted a command that failed due to lack of permission, re-ran it instantly with `sudo !!`, checked my identity with `whoami` and `id`, listed my sudo privileges with `sudo -l`, and practiced switching users with `sudo -i` and `su`.

## What surprised me
I was surprised how useful `sudo !!` is. Instead of retyping a long command, I can just add `sudo` to the previous command instantly.

## Evidence
Screenshot of the practice drill is stored in the [evidence](./evidence/) folder.

## Related
- Previous day: [day-07-ownership](../day-07-ownership/)
- Next day: [day-09-integrity-firewall](../day-09-integrity-firewall/)