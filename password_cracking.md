# Password Cracking

% password cracking

#platform/linux #target/local #cat/MISC/RECON

## Medusa Telnet

brute forces telnet passwords using Medusa

```
medusa -h <id> -m telnet -U <usernames-file> -P <passwords-file>
```

## Get Medusa Modules

lists what protocols Medusa can brute-force

```
medusa -d
```

## Rainbow Table Crack

uses rcracki_mt and rainbow tables to crack passwords

```
rcracki_mt -h <hash> -t 4 *.rti
```
