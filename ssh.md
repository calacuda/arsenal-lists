# SSH

% remote shell (secure)

#plateform/linux #target/local #cat/MISC/RECON #protocol/ssh #port/22

## Remote SSH access

ssh with out adding the remote host to KnownHosts file also, ignore if host key and host name don't match

```
ssh -o "UserKnownHostsFile=/dev/null" -o "StrictHostKeyChecking=no" <remote-username>@<ip>
```
