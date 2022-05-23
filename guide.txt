$ curl cheat.sh/
nmap
 cheat.sheets:nmap 
# Single target scan:
nmap [target]

# Scan from a list of targets:
nmap -iL [list.txt]

# Scan port for all available A records
# (useful when multiple A records are returned by the DNS server)
nmap --script resolveall \
    --script-args newtargets,resolveall.hosts=[target] -p [port]

# iPv6:
nmap -6 [target]

# OS detection:
nmap -O --osscan_guess [target]

# Save output to text file:
nmap -oN [output.txt] [target]

# Save output to xml file:
nmap -oX [output.xml] [target]

# Scan a specific port:
nmap -p [port] [target]

# Do an aggressive scan:
nmap -A [target]

# Speedup your scan:
# -n => disable ReverseDNS
# --min-rate=X => min X packets / sec
nmap -T5 --min-parallelism=50 -n --min-rate=300 [target]

# Traceroute:
nmap -traceroute [target]

# Ping scan only: -sP
# Don't ping:     -PN <- Useful if a host doesn't reply to a ping.
# TCP SYN ping:   -PS
# TCP ACK ping:   -PA
# UDP ping:       -PU
# ARP ping:       -PR

# Example: Ping scan all machines on a class C network
nmap -sP 192.168.0.0/24

# Force TCP scan: -sT
# Force UDP scan: -sU

# Use some script:
nmap --script default,safe

# Loads the script in the default category, the banner script,
# and all .nse files in the directory /home/user/customscripts.
nmap --script default,banner,/home/user/customscripts

# Loads all scripts whose name starts with http-,
# such as http-auth and http-open-proxy.
nmap --script 'http-*'

# Loads every script except for those in the intrusive category.
nmap --script "not intrusive"

# Loads those scripts that are in both the default and safe categories.
nmap --script "default and safe"

# Loads scripts in the default, safe, or intrusive categories,
# except for those whose names start with http-.
nmap --script "(default or safe or intrusive) and not http-*"

# Scan for the heartbleed
# -pT:443 => Scan only port 443 with TCP (T:)
nmap -T5 --min-parallelism=50 -n --script "ssl-heartbleed" -pT:443 127.0.0.1

# Show all information (debug mode)
nmap -d ...

# Discover DHCP information on an interface
nmap --script broadcast-dhcp-discover -e eth0

 cheat:nmap 
---
tags: [ networking ]
---
# Single target scan:
nmap [target]

# Scan from a list of targets:
nmap -iL [list.txt]

# iPv6:
nmap -6 [target]

# OS detection:
nmap -O --osscan_guess [target]

# Save output to text file:
nmap -oN [output.txt] [target]

# Save output to xml file:
nmap -oX [output.xml] [target]

# Scan a specific port:
nmap -source-port [port] [target]

# Do an aggressive scan:
nmap -A [target]

# Speedup your scan:
# -n => disable ReverseDNS
# --min-rate=X => min X packets / sec
nmap -T5 --min-parallelism=50 -n --min-rate=300 [target]

# Traceroute:
nmap -traceroute [target]

# Ping scan only: -sP
# Don't ping:     -PN <- Use full if a host don't reply to a ping.
# TCP SYN ping:   -PS
# TCP ACK ping:   -PA
# UDP ping:       -PU
# ARP ping:       -PR

# Example: Ping scan all machines on a class C network
nmap -sP 192.168.0.0/24

# Force TCP scan: -sT
# Force UDP scan: -sU

# Use some script:
nmap --script default,safe

# Loads the script in the default category, the banner script, and all .nse files in the directory /home/user/customscripts.
nmap --script default,banner,/home/user/customscripts

# Loads all scripts whose name starts with http-, such as http-auth and http-open-proxy.
nmap --script 'http-*'

# Loads every script except for those in the intrusive category.
nmap --script "not intrusive"

# Loads those scripts that are in both the default and safe categories.
nmap --script "default and safe"

# Loads scripts in the default, safe, or intrusive categories, except for those whose names start with http-.
nmap --script "(default or safe or intrusive) and not http-*"

# Scan for the heartbleed
# -pT:443 => Scan only port 443 with TCP (T:)
nmap -T5 --min-parallelism=50 -n --script "ssl-heartbleed" -pT:443 127.0.0.1

# Show all informations (debug mode)
nmap -d ...

# Scan for available SSH connections (use root for additional output)
nmap -p 22 192.168.0.0/24

## Port Status Information
- Open: This indicates that an application is listening for connections on this port.
- Closed: This indicates that the probes were received but there is no application listening on this port.
- Filtered: This indicates that the probes were not received and the state could not be established. It also indicates that the probes are being dropped by some kind of filtering.
- Unfiltered: This indicates that the probes were received but a state could not be established.
- Open/Filtered: This indicates that the port was filtered or open but Nmap couldn’t establish the state.
- Closed/Filtered: This indicates that the port was filtered or closed but Nmap couldn’t establish the state.

## Additional Scan Types

nmap -sn: Probe only (host discovery, not port scan)
nmap -sS: SYN Scan
nmap -sT: TCP Connect Scan
nmap -sU: UDP Scan
nmap -sV: Version Scan
nmap -O: Used for OS Detection/fingerprinting
nmap --scanflags: Sets custom list of TCP using `URG ACK PSH RST SYN FIN` in any order

### Nmap Scripting Engine Categories
The most common Nmap scripting engine categories:
- auth: Utilize credentials or bypass authentication on target hosts.
- broadcast: Discover hosts not included on command line by broadcasting on local network.
- brute: Attempt to guess passwords on target systems, for a variety of protocols, including http, SNMP, IAX, MySQL, VNC, etc.
- default: Scripts run automatically when -sC or -A are used.
- discovery: Try to learn more information about target hosts through public sources of information, SNMP, directory services, and more.
- dos: May cause denial of service conditions in target hosts.
- exploit: Attempt to exploit target systems.
- external: Interact with third-party systems not included in target list.
- fuzzer: Send unexpected input in network protocol fields.
- intrusive: May crash target, consume excessive resources, or otherwise impact target machines in a malicious fashion.
- malware: Look for signs of malware infection on the target hosts.
- safe: Designed not to impact target in a negative fashion.
- version: Measure the version of software or protocols on the target hosts.
- vul: Measure whether target systems have a known vulnerability.

 tldr:nmap 
# nmap
# Network exploration tool and security / port scanner.
# Some features only activate when Nmap is run with privileges.
# More information: <https://nmap.org>.

# Check if an IP address is up, and guess the remote host's operating system:
nmap -O ip_or_hostname

# Try to determine whether the specified hosts are up and what their names are:
nmap -sn ip_or_hostname optional_another_address

# Like above, but also run a default 1000-port TCP scan if host seems up:
nmap ip_or_hostname optional_another_address

# Also enable scripts, service detection, OS fingerprinting and traceroute:
nmap -A address_or_addresses

# Assume good network connection and speed up execution:
nmap -T4 address_or_addresses

# Scan a specific list of ports (use `-p-` for all ports `1-65535`):
nmap -p port1,port2,…,portN address_or_addresses

# Perform TCP and UDP scanning (use `-sU` for UDP only, `-sZ` for SCTP, `-sO` for IP):
nmap -sSU address_or_addresses

# Perform full port, service, version detection scan with all default NSE scripts active against a host to determine weaknesses and info:
nmap -sC -sV address_or_addresses

$
