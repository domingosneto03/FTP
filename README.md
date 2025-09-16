# RCOM Project 2

## Project Overview

- **Part 1:** Develop a basic FTP download client in C using sockets  
- **Part 2:** Configure and study a local network with Linux machines and routers

## Part 1 – FTP Download Application

### Objectives

- Develop an application to download a file from  
  `ftp://ftp.netlab.fe.up.pt/pub/...`
- Implement FTP protocol behavior according to **RFC 959**
- Use passive mode and URL structure from **RFC 1738**
- Practice:
  - Sockets in C
  - DNS resolution
  - Control/data connection management
  - TCP/IP understanding

### To test:

```bash
$ gcc -Wall -o download clientTCP.c
$ ./download ftp://ftp.up.pt/pub/gnu/emacs/elisp-manual-21-2.8.tar.gz
$ ./download ftp://demo:password@test.rebex.net/readme.txt
$ ./download ftp://anonymous:anonymous@ftp.bit.nl/speedtest/100mb.bin

$ ./download ftp://rcom:rcom@ftp.netlab.fe.up.pt/README
$ ./download ftp://rcom:rcom@ftp.netlab.fe.up.pt/pipe.txt
$ ./download ftp://rcom:rcom@ftp.netlab.fe.up.pt/files/crab.mp4
```
---

## Part 2 – Network Configuration & Analysis

### Topics Covered

- IP configuration using `ifconfig`, `route`, `arp`
- Packet capture with Wireshark
- Network experiments:
  - ARP inspection
  - IP routing
  - Creating and managing Linux bridges
  - Configuring routers and NAT
  - DNS testing
  - TCP connection and congestion analysis

---

## Key Experiments

1. **Basic IP configuration and ARP analysis**
2. **Bridge setup and broadcast domain separation**
3. **Router setup in Linux**
4. **Commercial router with NAT**
5. **DNS usage and packet observation**
6. **TCP connection behavior (with file transfer and Wireshark)**
