# SNMP

% SNMP Simple Network Management Protocol

#plateform/linux #target/remote #protocol/snmp #port/161

## onesixtyone - find SNMP hosts

```
echo "<ip>" >> 161.ips; echo public > community; echo private >> community; echo manager >> community; onesixtyone -c community -i 161.ips; rm community 161.ips
```

## nmap - find SNMP hosts

```
sudo nmap -sU --open -p 161 <ip> -oG open-snmp.txt
```
