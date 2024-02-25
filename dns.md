# DNS

% DNS Enumeration

#platform/linux #target/local #cat/MISC/RECON #protocol/dns #port/53

## Bash - Subdomain Enumneration (brute-force)

```
for subd in $(cat <wordlist>); do host $subd.<domain>; done
```

## Bash - Reverse DNS Enum (brute-force)

```
for ip in $(seq <start> <end>); do host <IP-FORMAT>; done | grep -v "not found"
```

## dnsrecon - Subdomain Enumeration (brute-force)

```
dnsrecon -d <domain-name> -D <wordlist> -t brt
```

## dnsenum2 - normal DNS recon

```
dnsrecon <domain-name>
```
