Introduction to NMAP
Nmap is an open source port scanning tool that was first published in September 1997. The source code was
posted in an article in Phrack Magazine, and it was further developed by the community. The latest release,
as of this post date, is Nmap 7.92, released in August 2021.

Nmap is the cornerstone of the recon phase for network 
security testing, and for good reason, it comes with a
library of Lua scripts that add a lot of utility. There 
are scripts for everything from scanning for
vulnerabilities to conducting brute force attacks. 
These scripts are all handled by the Nmap Scripting 
Engine (NSE), and we will go over that
once we’ve dialed in on some of the basics.


As always during reconnaissance, scanning is the initial stage for information gathering.

## What is reconnaissance?

Reconnaissance is to collect as much as information about a target network as possible.From a hacker’s 
perspective, the information gathered is very helpful to make an attack, so to block that type of malicious 
attempt, generally a penetration tester tries to find the information and to patch the vulnerabilities if found. 
This is also called Footprinting. Usually by information gathering, someone can find the below information:

E-mail Address
Port no/Protocols
OS details
Services Running
Traceroute information/DNS information
Firewall Identification and evasion
And many more…



So for information gathering, scanning is the first part.
For scanning, Nmap is a great tool for discovering Open ports, 
protocol numbers, OS details, firewall details, etc.




Before we can understand Nmap we have to understand port scanning.
Computers communicate using ports. There are a total of 65,535 ports, 
but few of these ports will be utilized yet alone open.

Within these large number of ports, there are whats known as common or 
well-known ports which range from 0 to 1023. Here are some examples:

<ul><li>port 20 (FTP)
  </li><li>port 22 (SSH/SCP)
  </li><li>port 23 (Telnet)
  </li><li>port 53 (DNS)
  </li><li>port 80 (HTTP)
  </li><li>port 443 (HTTPS)
  </li></ul>
  
  
  
  
