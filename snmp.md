# SNMP

% SNMP Simple Network Management Protocol

#plateform/windows #target/remote #protocol/snmp #port/161

## onesixtyone - find SNMP hosts

```
echo "<ip>" >> 161.ips; echo public > community; echo private >> community; echo manager >> community; onesixtyone -c community -i 161.ips; rm community 161.ips
```

## nmap - find SNMP hosts

```
sudo nmap -sU --open -p 161 <ip> -oG open-snmp.txt
```

## snmp list system processes

```
snmpwalk -c <comunity-string> -v1 <ip> 1.3.6.1.2.1.25.1.6.0
```

## snmp list running programs

```
snmpwalk -c <comunity-string> -v1 <ip> 1.3.6.1.2.1.25.4.2.1.2
```

## snmp list process path

```
snmpwalk -c <comunity-string> -v1 <ip> 1.3.6.1.2.1.25.4.2.1.4
```

## snmp list storage units

```
snmpwalk -c <comunity-string> -v1 <ip> 1.3.6.1.2.1.25.2.3.1.4
```

## snmp list installed software

```
snmpwalk -c <comunity-string> -v1 <ip> 1.3.6.1.2.1.25.6.3.1.2
```

## snmp list user accounts

```
snmpwalk -c <comunity-string> -v1 <ip> 1.3.6.1.4.1.77.1.2.25
```

## snmp list listening TCP ports

```
snmpwalk -c <comunity-string> -v1 <ip> 1.3.6.1.2.1.6.13.1.3
```
