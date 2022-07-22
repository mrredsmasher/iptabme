# Introduction

This is a simple script which will create some iptables rules to isolate you from other TryHackMe VPN users. 

Inspired on https://github.com/Wh1teDrvg0n/safeVPN-THM.git

# Usage

Once connected to the VPN, deploy a machine, grab the IP address and then use the script:

```bash
88 88""Yb 888888    db    88""Yb 8b    d8 888888 
88 88__dP   88     dPYb   88__dP 88b  d88 88__   
88 88"""    88    dP__Yb  88""Yb 88YbdP88 88""   
88 88       88   dP""""Yb 88oodP 88 YY 88 888888 


                        Author: @Mr_RedSmasher

Usage: ./iptabme <clean>: Deletes TryHackMe chain and related links
Usage: ./iptabme <create> <IP>: Deletes previous TryHackMe chain and create a new chain + add the rules
Examples:
        - ./iptabme create 10.10.12.21
        - ./iptabme clean
```


# Notes
The "create" subcommand will try to remove old Tryhackme rules.
This way you can create rules for a machine, deploy a new machine and execute "create" which will clean the old one for you.
