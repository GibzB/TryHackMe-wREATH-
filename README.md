# TryHackMe-wREATH-

Steps taken in completing this room starting from task 5 onwards

### Task 5: Webserver

1. How many of the first 15000 ports are open on the target?
Code: nmap -p 1-15000 -oA webserve 10.200.181.200

Ans: 4

2. Perform a service scan on these open ports. What OS does Nmap think is running?
code: nmap -p 22,80,443,10000 -sV -oA webserve-service 10.200.181.200

Ans: CentOs
