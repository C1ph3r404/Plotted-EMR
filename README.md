# README.md — Plotted-EMR (TryHackMe)

Short repo summary for the box I did on TryHackMe.

## Plotted-EMR — quick summary
TryHackMe Plotted-EMR walkthrough: used OpenEMR site setup + patched PoC to get RCE as `www-data`, abused a cron/rsync job by injecting `-e sh shell.sh` via crafted filenames to get `plot_admin`, and then used `perl` with an `fowner` capability to `chmod` `/root/root.txt` and read the root flag.

## Files
- `WriteUp.md` — detailed walkthrough with commands & explanations  
- `screenshots/` — evidence (nmap, ffuf, exploit patch, cron/rsync, flags)

## Disclaimer

For learning & lab use only. Don’t run these techniques on networks/systems you don’t own or have permission to test.

---
