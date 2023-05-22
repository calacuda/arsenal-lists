# SMB

% SMB

#plateform/linux #target/remote #cat/MISC/RECON #port/445

## SMB Name Enum

```
nbtscan -r <start IP>/<Network Bits>/
```

## Nmap find SMB servers

```
nmap -v -p 139,445 -oG smb.txt <ip-range>
```
