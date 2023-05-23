# SNMP

% SNMP Simple Network Management Protocol

#plateform/linux #target/remote #cat/RECON #port/161

## onesixtyone - find SNMP hosts

```
echo "<ip>" >> 161.ips; echo public > community; echo private >> community; echo manager >> community; onesixtyone -c community -i 161.ips; rm community 161.ips
```
