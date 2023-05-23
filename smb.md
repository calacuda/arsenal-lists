# SMB

% SMB

#plateform/linux #target/remote #protocol/smb #port/445/139

## SMB Name Enum

```
nbtscan -r <start IP>/<Network Bits>/
```

## Nmap - find SMB servers

```
nmap -v -p 139,445 -oG smb.txt <ip-range>
```
