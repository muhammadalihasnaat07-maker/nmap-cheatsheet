# \U0001f5fa\ufe0f Nmap Cheat Sheet

> A comprehensive, dark-themed **Nmap** command and NSE script reference — open directly in your browser.

## \U0001f4cb What's Included

| Section | Details |
|---|---|
| **Scan Types** | TCP SYN, Connect, ACK, FIN, Xmas, Null, UDP, SCTP, IP Protocol |
| **Target Spec** | IPs, CIDR ranges, file input, IPv6, hostname |
| **Port Options** | Single, range, all 65535, top-N, protocol-specific |
| **OS & Version** | Fingerprinting, intensity levels, aggressive mode |
| **Timing** | T0 Paranoid → T5 Insane, min-rate, retries |
| **Evasion** | Packet fragmentation, decoys, IP/MAC spoofing, proxies |
| **Output** | Normal, XML, Grepable, Script Kiddie, All |
| **NSE Scripts** | 50+ scripts: HTTP, SSL/TLS, SMB, FTP, SSH, DNS, DB, Mail, SNMP, RDP, VNC |

## \U0001f680 Live Preview

**[View the Cheat Sheet \u2192](https://muhammadalihasnaat07-maker.github.io/nmap-cheatsheet/nmap-cheatsheet.html)**

## \u26a1 Quick Reference

```bash
nmap -A -T4 <target>                          # Aggressive full scan
nmap -p- -sV <target>                         # All ports + service versions
nmap -sS -D RND:5 <target>                    # Stealth scan with decoys
nmap --script vuln <target>                   # All vulnerability scripts
nmap -p445 --script smb-vuln-ms17-010         # EternalBlue check
nmap -p443 --script ssl-enum-ciphers          # SSL cipher audit
nmap -p443 --script ssl-heartbleed           # Heartbleed test
```

## \u26a0\ufe0f Legal Notice

> Only scan systems you **own** or have **explicit written permission** to test.
> Unauthorized port scanning is illegal in many jurisdictions.
> Use `scanme.nmap.org` for authorized practice scanning.

---
*Built with Claude Sonnet 4.6 \u2022 [nmap.org](https://nmap.org)*
