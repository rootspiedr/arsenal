# smb

% windows, samba, smb, 139, 445

## nbtscan - scan network looking for hosts
```
nbtscan -r <ip_range>
```

## smbclient with username and password
```
smbclient \\\\<ip>\\<share> -U "<user>%<pass>"
```

## smbclient sessions without password
```
smbclient \\\\<ip>\\<share> -U "<user>%"
```

## smbclient null session
```
smbclient \\\\<ip>\\<share> -U "%"
```

## smb - find not signed  smb
```
nmap -Pn -sS -T4 --open --script smb-security-mode -p445 <ip>
```

## smb mount folder
```
mount -t cifs //<ip>/C\$ /tmp/mnttarget/ -o username=<user> -o domain=<domain>
```


