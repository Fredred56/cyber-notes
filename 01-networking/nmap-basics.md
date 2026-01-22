# Nmap Basics

## Why Nmap?
Nmap is the #1 tool for discovery and enumeration in pentesting.

## 1) Full port scan (fast)
```bash
nmap -p- --min-rate 1000 -T4 <ip>
```
## 2) Services & version detection
```bash
nmap -sC -sV -p <ports> <ip>
```
## 3) Output saving
```bash
nmap -sC -sV -oN nmap.txt <ip>
```
## 4) UDP scan (basic)
```bash
nmap -sU --top-ports 200 <ip>
```
Common workflow
1. Full scan ports
2. Target scan on found ports
3. Enumerate services (HTTP/SMB/FTP/SSH)
4. Look for attack suface

Notes
* -p- = all ports
* -sC- = default scripts
* -sV- = detect versions
* -oN- = normal output file
