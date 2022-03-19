# TryHackMe-wREATH-

Steps taken in completing this room starting from task 5 onwards

### Task 5: Webserver

1. How many of the first 15000 ports are open on the target?
Code: nmap -p 1-15000 -oA webserve 10.200.181.200

Ans: 4

2. Perform a service scan on these open ports. What OS does Nmap think is running?
code: nmap -p 22,80,443,10000 -sV -oA webserve-service 10.200.181.200

Ans: CentOs

3. Open the IP in your browser -- what site does the server try to redirect you to?
code: 10.200.181.200 (type in browser)

Ans: https://thomaswreath.thm/

4. Looks like Thomas forgot to set up the DNS!

Add it to your hosts file manually. 
Ans added 10.200.181.200 https://thomaswreath.thm/ in hosts file on /etc/hosts
