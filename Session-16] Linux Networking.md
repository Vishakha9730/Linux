# Linux Networking -

## ifconfig -
- ifconfig (short for Interface Configurer) is a command used to view and configure network interfaces (like Ethernet, Wi-Fi, or virtual connections).
- It shows:
  - Your IP address
  - MAC address (hardware ID)
  - Network status (UP/DOWN)
  - Data transfer stats (sent/received packets)

## ping – 
- Check internet connection.
- Tests if your computer can reach a server (like Google) and measures response time (latency).

#### Syntax:

    ping [website/IP]

####  Example:

    ping google.com


## nslookup -
- A basic tool to find IP addresses and DNS records (installed by default on most systems).

#### Basic Syntax

    nslookup [domain/IP] [DNS-server]

#### Examples

    nslookup google.com


## dig (Advanced DNS Lookup) -
- A more powerful DNS tool that provides detailed DNS records (needs dnsutils or bind-utils).

#### Install dig (if missing) -

    sudo apt install dnsutils     # Debian/Ubuntu
    sudo yum install bind-utils   # RHEL/CentOS

#### Basic Syntax -

    dig [domain/IP] [record-type] @[DNS-server]

#### Examples -

    dig google.com
    dig AAAA google.com --> IPv6 add

## netstat -tuln -
- Shows listening ports (services waiting for connections) and active connections.

#### Install net-tools (if missing)

    sudo apt install net-tools     # Debian/Ubuntu
    sudo yum install net-tools    # RHEL/CentOS

#### Basic Syntax -
  
    netstat -tuln
    
###### Options -

    -t	Show TCP ports
    -u	Show UDP ports
    -l	Show listening ports only
    -n	Show numeric IPs (no DNS resolution)

## ss -tuln -
- Does the same as netstat but faster (uses kernel sockets directly).

#### Basic Syntax

    ss -tuln

## traceroute – 
- Shows every hop (router) your connection passes through to reach a destination (e.g., Google).

#### Install traceroute (if missing)-

      sudo apt install traceroute   # Debian/Ubuntu
      sudo yum install traceroute  # RHEL/CentOS

#### Basic Syntax

      traceroute [domain/IP]

#### Example: 

      traceroute google.com

## mtr -
- A continuous traceroute + ping combo that shows live network stats (packet loss, latency).

#### Install mtr (if missing) -

    sudo apt install mtr  
    sudo yum install mtr

#### Syntax -

    mtr [domain/IP]

- Press q to quit.

#### Example -

    mtr google.com

## wget (Download Files from Internet) -
- Downloads files from the web via terminal.

#### Syntax:

  wget [URL]

#### Example:

  wget https://example.com/file.zip

## scp (Securely Copy Files to Another PC) -
- Transfers files securely between Linux machines.

#### Syntax:

   scp [file] [user@remoteIP:/path]

#### Example -

    scp report.txt user@192.168.1.5:/home/user/

## iptables (Check Firewall Rules)-
- Lists firewall rules (if using iptables).
#### Syntax:

    iptables -L

## ufw (Simple Firewall Manager - Ubuntu) -
- Manages firewall settings easily.

#### Syntax:

        ufw [enable/disable/status]










    
