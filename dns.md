# DNS

% DNS Enumeration

#plateform/linux #target/local #cat/MISC/RECON #port/53

## Subdomain Enumneration

```
for subd in $(cat <wordlist>); do host $subd.<domain>; done
```

## Reverse DNS Enum

```
for ip in $(seq <start> <end>); do host <IP-FORMAT>; done | grep -v "not found"
```
