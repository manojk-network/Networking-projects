# Nmap Vulnerability scan

## Objective
Scan a website to identify open ports, detect service versions, and check for known vulnerabilities.

## Tools Used
- Nmap
- Kali Linux (Terminal)

## What I Did
- Ran a SYN scan on the top 100 ports of the target website:
  ```bash
  nmap -sS -Pn -T4 --top-ports 100 scanme.nmap.org
  ```
  Reason: Used SYN scan because it's fast and stealthy compared to a full TCP scan.
  
- Detected service versions:
  ```bash
  nmap -sV -Pn -T4 --top-ports 100 scanme.nmap.org
  ```
  Reason: Used version detection to map services to CVEs.

## Result
- Open ports identified.
- Service versions detected.
- Potential vulnerabilities based on version info

## Video Link
   
