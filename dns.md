# DNS

% DNS Enumeration

#plateform/linux #target/local #cat/MISC/RECON #port/53

## Subdomain Enumneration

```
for subd in $(cat <wordlist>); do host $subd.<domain>; done
```
