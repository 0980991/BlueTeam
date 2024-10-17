## Network Topologies
The network topology is t
- POint-to-Point
- Een hub gebruikt een logische STAR-topology en physieke bus
- Mesh (n*(n-1)/2) waar n d ehoeveelheid nodes zijn
  

TCP/IP (DOD) model vs OSI model

TCP/IP combineerd OSI lagen in totaal 4 lagen

1. Process
2. Host-to-HOst
3. Internet
4. Network Access

Preamble het synchronizeren van het zenden en sturen van packages

EAP LEAP PEAP, SIP PROTOCOL 

Physical:
- Switches, (Passive) Hubs, Modems, Tranceivers
- SOHO router
- 
Datalink: De eerste laag van intelligentie,
- NICs, bridge, switch, wireless access point
- Switch is de opvolger van een bridge en kijken naar mac adressen
- Physieke (MAC) Adresseh

Network Layer
- Logische addressering
- Routers kijken naar IP adressen
- Routers, IP, ACL, Basic Firewall

Transport layer:
- tracks communication between applications on source an destination hosts
- Segments data and manages each data piece.
- reassembles segments into application data
- Firewall, IDS (Intrusion detection system), IPS

Session:
- ASP, ASDP

Presentation:
- MIME, encryptie en decryptie, delivers data

Application layer
- SMTP, ftp, DNS

The access point is responsible for communicating with the supplicant and sending information to the authenticating server. This device is called the authenticator. The end device that sends credentials is called the supplicant. The supplicant is a piece of software in the operating system that supplies the credentials for AAA authentication. The AAA server is normally a RADIUS server or TACACS+ server that is configured for 802.1X.

// ADD 1X

## Table of 802 some standards
| Name   | Description                                                                                                                                                                                                                                                           | Related Tags                          |
|--------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|
|        |                                                                                                                                                                                                                                                                       |                                       |
|        |                                                                                                                                                                                                                                                                       |                                       |
| 802.1  | 802.1 looks at LAN/MAN architecture, overall network management and protocol layers above the MAC and LLC layers.                                                                                                                                                     |                                       |
| 802.1d | Remote MAC bridging across LAN                                                                                                                                                                                                                                        |                                       |
| 802.1g | Remote Mac Bridging across non-LAN in accordance with Spanning Tree                                                                                                                                                                                                   | MAC, STP, Bridge                      |
| 802.1Q | Specification for VLANs and VLAN bridges                                                                                                                                                                                                                              | (Native) Trunk, VLAN, VLAN Bridge     |
| 802.1X | Specification for Port Based Access Control (PNAC)                                                                                                                                                                                                                    | PNAC     |
| 802.2  | Defines Logical Link Control (LLC, aka the upper part of layer 2) which handles primarily the (de)multiplexing of signals                                                                                                                                             | Multiplexing, LLC, MAC, Layer 2       |
| 802.3  | Defines the physical and data-link's layer Media Access Control of wired Ethernet.                                                                                                                                                                                    | Ethernet, CSMA/CD                     |
| 802.4  | Defines a Token Bus; a standard for deploying token rings on LAN over a virtual ring which decreases collisions                                                                                                                                                       | Token Bus, Physical Bus, Logical Ring |
| 802.5  | Defines a Token Ring Access Method. Token Ring is a physical and data link layer computer networking technology used to build local area network.                                                                                                                     |                                       |
| 802.6  | Defines a MAN-governed standard that uses the Distributed Queue Dual Bus (DQDB) network form                                                                                                                                                                          | Distributed, Dual Bus,                |
| 802.7  | Defines Broadband Local Area Networks                                                                                                                                                                                                                                 | Broadband LAN                         |
| 802.8  | The Fiber Optic Technical Advisory Group created a LAN standard for fiber optic media used in token passing computer networks like FDDI.                                                                                                                              |                                       |
| 802.9  | IsoEthernet combines 10 megabits per second Ethernet and 96 64Kbs ISDN B channels. It was originally developed to provide data and voice/video over the same wire without degradation by fixing the amount of bandwidth assigned to the Ethernet and B-channel sides. | IsoEthernet, voice/video              |
| 802.10 | A former standard that defined security functions such as security association management and key management, as well as access control, data confidentiality and data integrity.                                                                                     |                                       |
| 802.11 | A LAN standard that specifies layer 1 & 2 protocols for implementing Wireless Local Access Network (WLAN) communications.                                                                                                                                             | Wi-Fi, WLAN,                          |
| 802.11a | 5GHz by using Dynamic Frequency Selection to avoid interference with things like radar. It also uses orthogonal frequency division multiplexing to allow multiple channels to stream at the same frequency                                                           | Wi-Fi, WLAN, DFS, OFDM                |
| 802.11b | 2.4GHz by using Direct Sequence Spread Spectrum                                                                                                                                                                                                                      | Wi-Fi, DSSS,                          |
| 802.11g | 5Ghz  also uses OFDM                                                                                                                                                                                                                                                 | Wi-Fi, WLAN, OFDM                     |
| 802.11g | ?Ghz an incorporates the Temporal Key Integrity Protocol (TKIP)                                                                                                                                                                                                      | Wi-Fi, TKIP                           |
| 802.11n |  Wifi 4 at 2,4/5Ghz of speed 72-600Mbs uses Multiple Input Multiple Output                                                                                                                                                                                           | Wi-Fi 4, MIMO                         |
| 802.11ac | Wifi 5 at 2,4/5Ghz of speed 433-6933Mbs                                                                                                                                                                                                                             | Wi-Fi 5                               |
| 802.11ax | Wifi 6 & 6E at 2,4/5/6Ghz of speed 574-9608                                                                                                                                                                                                                         | Wi-Fi 6, Wifi-6E                      |
| 802.11be | Wifi 6 & 6E at 2,4/5/6Ghz of speed 574-9608                                                                                                                                                                                                                         | Wi-Fi, WLAN                           |
| 802.12 | 100BaseVG (Voice Grade) is a 100 Mbs Ethernet standard specified to run over four pairs of Category 3 cable. It was made it's own standard to meet the need of being long distance.                                                                                   |                                       |



## Table of Application Layer Protocols

| Name                                           | Abbr.  | Port #                   | TCP or UDP | Layer #                      | Description                                                                                                                                                                                                                                                                                                                                                             |
|------------------------------------------------|--------|--------------------------|------------|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Internet Protocol                              | IP     | -                        | -          | Network                      |                                                                                                                                                                                                                                                                                                                                                                         |
| Transmission Control Protocol                  | TCP    | -                        | -          | Transport                    |                                                                                                                                                                                                                                                                                                                                                                         |
| User Datagram Protocol                         | UDP    | -                        | -          | Transport                    |                                                                                                                                                                                                                                                                                                                                                                         |
| Generic Routing encapsulation                  | GRE    | -                        | -          | Network                      | is used by IP Security Protocol (IPSec) for the confidentiality of the payload.                                                                                                                                                                                                                                                                                         |
| Encasulating Security Payload                  | ESP    | -                        | -          | Network                      | A tunneling protocol that encapsulates etwork layer protocols inside virtual point-to-point links or point-to-multipoint links over an IP network.                                                                                                                                                                                                                      |
| Internet Control Message Protocol              | ICMP   | -                        | -          | Network                      | Used by network devices, including routers, to send error messages and operational information indicating success or failure when communicating with another IP   address.                                                                                                                                                                                                                      |                                                                                                                                                                                                                                                                            |
| File Transfer Protocol                         | FTP    | 20/21                    | TCP        | Application                  | FTP is both a protocol and a program used for file transfers between multiple machines                                                                                                                                                                                                                                                                                  |
| Secure Shell                                   | SSH    | 22                       | TCP        | Application                  | SSH sets up a secure telnet session over a standards TCP/IP connection which allows a remote user to execute commands                                                                                                                                                                                                                                                   |
| Secure File Transfer Protocol                  | SFTP   | 22                       | TCP        | Application                  | FTP via a SSH session.                                                                                                                                                                                                                                                                                                                                                  |
| Telnet                                         | -      | 23                       | TCP        | Application                  | Allows a user to initiate a remote session to a (telnet) client. Similar to SSH                                                                                                                                                                                                                                                                                         |
| Simple Mail Transfer Protocol                  | SMTP   | 25                       | TCP        | Application                  | A protocol that uses a queued method of to send mail. A SMTP server regularly checks the the queue for messages and sends them through to their destination                                                                                                                                                                                                             |
| Domain Name System                             | DNS    | 53                       | TCP/UDP    | Application                  | DNS converts hostnames (google.com) to their respective IP addresses. DNS is used to resolve Fully Qualified Domain Names (FQDM or DNS namespaces). These are hierarchical structures that can logically locate a system based on its domain identifier. (e.g. mail.google.com/maps.google.com)                                                                         |
| Dynamic Host Configuration Protocol            | DHCP   | 67/68                    | UDP        | Datalink, Network, Transport | DHCP servers assign IP addresses to hosts using information provided by the server. This information includes but is not limited to: IP addresses, Subnet masks, domain names, default gateways and DNS. A client receives an IP in 4 steps (DORA). Discover, Offer, Request, Acknowledge                                                                               |
| Trivial File Transfer Protocol                 | TFTP   | 69                       | UDP        | Application                  | A compact version of FTP which can only send and receive files and not browse directories. Not commonly used due to inherent security risks.                                                                                                                                                                                                                            |
| Hyper Text Transfer Protocol                   | HTTP   | 80                       | TCP        | Application                  | The protocol used for showing graphics, text, links etc in the form of html files                                                                                                                                                                                                                                                                                       |
| Post Office Protocol (v3)                      | POP(3) | 110                      | TCP        | Application                  | Provides a storage facility for incoming mail by releasing messages for downloading to a specific client when said client connects to the network. Is replaced more and more by IMAP due to flexibility and security.                                                                                                                                                   |
| Network Time Protocol                          | NTP    | 123                      | UDP        | Application                  | Provides the ability to synchronize clocks across computers so that all computers agree on a certain time.                                                                                                                                                                                                                                                              |
| Internet Message Access Protocol               | IMAP   | 143                      | TCP        | Application                  | Provides more control over how you download your mail by peeking at the message header and downloading only parts of the email, thus providing a better defence against malicious emails.                                                                                                                                                                               |
| Simple Network Management Protocol             | SMNP   | 161/162                  | UDP        | Application                  | Provides and manipulates valuable network information. Basically acts as a watchtower that polls devices for certain info at random intervals to determine the status of a healthy network. When aberrations occur, 'agents' send 'trap' or alert to the management station. The Network Management system polls agents through a Management Information Database (MIB) |
| Lightweight Directory Access Protocol          | LDAP   | 389                      | TCP        | Application                  | Provides access to query directory service systems such as Microsoft Active Directory. Is used mostly by system admins that keep track of network resources such as devices and users.                                                                                                                                                                                  |
| Hyper Text Transfer Protocol Secure            | HTTPS  | 443                      | TCP        | Application                  | Provides security to HTTP by encrypting requests made across the network. Prevents things such as MitM attacks                                                                                                                                                                                                                                                          |
| Server Message Block                           | SMB    | TCP:445/UDP:137,138      | TCP/UDP    | Application                  | Used for sharing access to files and printers and other communications between hosts on a MS Windows network                                                                                                                                                                                                                                                            |
| Syslog                                         | -      | 514                      | UDP        |                              | Used for reading system messages from switches' or routers' internal buffer in order to see what happening on the network at a particular time. It labels messages at 1 of 7 8 severity levels (level 0 to 7). 0. Emergency 1. Alert 2. Critical 3. Error 4. Warning 5. Notification 6. Information 7. Debugging                                                        |
| Simple Mail Transfer Protocol Secure           | SMTPS  | 587                      | TCP        | Application                  | A more secure version of SMTP that encrypts the mail before sending it                                                                                                                                                                                                                                                                                                  |
| Lightweigth Directory Access Protocol over SSL | LDAPS  | 636                      | TCP        | Application                  | A more secure version of LDAP that uses an SSH channel to secure the transmission                                                                                                                                                                                                                                                                                       |
| IMAP over SSL                                  | IMAPS  | 993                      | TCP        | Application                  | See above but over SSL                                                                                                                                                                                                                                                                                                                                                  |
| POP3 over SSL                                  | POP3S  | 995                      | TCP        | Application                  | See above but over SSL                                                                                                                                                                                                                                                                                                                                                  |
| SQL Server                                     | -      | 1433                     | TCP        | Application                  | A Microsoft database that is commonly used                                                                                                                                                                                                                                                                                                                              |
| SQLnet                                         | -      | 1521                     | TCP        | Application                  | Oracle database that allows remote acces.                                                                                                                                                                                                                                                                                                                               |
| H.323 (Video)                                  | H232   | 1720                     | TCP        | Application                  | Provides a standard for video on an IP network that defines how real-time audio, video and data information is transmitted.                                                                                                                                                                                                                                             |
| Media Gateway Control Protocol                 | MGCP   | 2427/2727                | TCP        | Application                  | Used for handeling the signaling and session management needed during a multi-media conference. It allows the media gateway to communicate with the media gateway controller. The media gateway converts data from format for a circuit-switched network to the format for a packet-switched network.                                                                   |
| MySQL                                          | -      | 3306                     | TCP        | Application                  | A relational database management system based on SQL most commonly used as a cloud-based database.                                                                                                                                                                                                                                                                      |
| Remote Desktop Protocol                        | RDP    | 3389                     | TCP        | Application                  | A Microsoft based remote desktop tool commonly used in corporate settings.                                                                                                                                                                                                                                                                                              |
| Real-time Transport Protocol (VOIP)            | RTP    | UDP: 5004/TCP: 5005      | TCP/UDP    | Application                  | A packet-formatting standard for delivering audio and video over the internet. It was is initially multicast but now also unicast.                                                                                                                                                                                                                                      |
| Session Initiation Protocol                    | SIP    | TCP, UPD: 5060/TCP: 5061 | TCP/UDP    | Application                  | Used to construct and deconstruct multimedia communication sessions such as audio/video calls. It works in conjunction with RTP.                                                                                                                                                                                                                                        |


                                                                                                                                                                                       |
## Ethernet

Baseband vs Broadband

| Protocol                                               | Abbr.     | Cable Type         | Description                                                                      |
|--------------------------------------------------------|-----------|--------------------|----------------------------------------------------------------------------------|
| Ethernet over Twisted Pair                             | 10BaseT   | UTP                | 10Mbit Baseband Twisted pair cable (Unshielded TP)                               |
| Thin Ethernet (Ethernet over COAX)                     | 10Base2   | Thin Coax          | 10Mbit Baseband over Coax with a max cable length of 200m                        |
| Thicc Ethernet                                         | 10Base5   | Thick Coax         | 10Mbit Baseband over thick coax with a max cable length of 500m                  |
| Ethernet over 2 pairs of cat5 UTP                      | 10BaseTX  | UTP                | 10Mbit Baseband over unshielded twisted pair                                     |
| Ethernet over Optical Fibre                            | 100BaseFX | Fibre Optics       | 100Mbit Baseband over fibre optics                                               |
| Ethernet over Optical Fibre                            | 100BaseSX | Fibre Optics       | 100Mbit Baseband over fibre optics                                               |
| Ethernet over Optical Fibre                            | 100BaseFX | Fibre Optics       | 100Mbit Baseband over fibre optics                                               |


## Routing Protocols Administrative Distance Table
| Protocol | Administrative Distance |
|----------|-------------------------|
| EIGRP    | 90                      |
| IGRP     | 100                     |
| OSPF     | 110                     |
| RIP      | 120                     |


## Netstat parameters
| Command     | Purpose                                                                                                                                      |
|-------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| netstat -a  | Displays all connections and listening ports, including both active and inactive ones .                                                      |
| netstat -c  | Continuously print the selected network statistics at regular intervals. This option is useful for monitoring network activity in real-time. |
| netstat -e  | Displays Ethernet statistics.                                                                                                                |
| netstat -n  | Displays addresses and port numbers in numerical form instead of using friendly names.                                                       |
| netstat -r  | Displays the contents of the routing table.                                                                                                  |
| netstat -s  | Displays statistics categorized by protocol.                                                                                                 |

# Hoofdstuk 2:
- Ethernet
- xBASE-Y (e.g 10Base-T = Unshielded twisted paar)
  - x - snelheid
  - y - het medium
- CSMA/CD --> Carrier Sense Multiple Access with Collision Detection
- UTP cable (100Mb = 4 adertjes, 1Gb = 8 adertjes) (B standaard)
  1. wit/oranje (T+)
  2. orange (T-)
  3. wit/groen (R+)
  4. blauw
  5. wit/blauw
  6. groen (R-)
  7. wit/bruin
  8. bruin

- Kruiskabel heeft een andere volgorde 

- Shielded Twisted Pair - RJ11 - RJ45
- Cable soorten EIA/TIA 568A & B (1 is kruis de ander recht)

- Fiber optic connector types:
  - Subscriber Connector 
  - ...
- Single Mode vs Multimode
  - ...
- WDM (Wavelenght Division Multiplexing)
  - Bidirectional, Coarse, Dense

- Rack systems (servers in kooien)

- HVAC 

- UPS - Uninterruptable powersupply
- 
- Tone generator kan worden gebruikt om uiteinde van dezelfde kabel te identificeren

- TDR - Time Domain Reflectormeter --> Kan je meten waar een bruik in een kabel zit door een signaal te reflecteren. (OTDR voor glas (optical))


# Hoofdstuk 3 - Network Interface:

SFD - Start of Frame Delimiter

- NIC
  - Transceiver component
  - Connects the host to a transmission
  - Can have multiple ports on the same card
  - Has unique MAC
  - Operates on the Data link layer

- NIC Issues
  - Connectivity Failure
  - Slow internet
  - ....

- Ethernet frame --> leer volgorde

-  Switch poort onderscheid een collision domain

- Spanning Tree Diagram (Ensures the network remains working when a bridge breaks or a loop is introduced in the network.)

- Ports kunnen de status: disables, block, listening, learning & forward

- Port cost (BPDU - Bridge Port Data unit)
  - NCN (Network Change Notification)
  - RSTP
  - BPDUGuard & RootGuard configureren (dit kan alleen op managed switches)
  
- PoE (Power over Ethernet)

- Broadcast Storm
  - Monitor the DHCP traffic to diagnose the issue
  - Segment the network using routers to resolve Broadcast Storms
  - 

- Link aggregation = samenlinken van ports op een switch.

# Hoofdstuk 4: 
TCP/IPv4

Zonder routers moeten devices in het netwerk dezelfde network id hebben 

Multicast vs Unicast 

Ontoegangelijke IP adressen:
0.0.0.0
127.0.0.1
169.254.0.0
255.255.255.255 - ff:ff:ff:ff:ff:ff

CIDR notatie: Classless interdomain routing notatie
192.168.1.0/24

/24 geeft aan dat het netwerk mask 3x8 bits is aka 24 aka 255.255.255.0


NAT - Network Address Translation = Het vervangen van de source IP (lokaal netwerk) naar de source IP van de route als je bijvoorbeeld met het internet verbind.

PAT - Port Address Translation = Het vervangen van bijvoorbeeld een well known port (security through obscurity)

IPv4 Datagram Header
- TTL (Time to live aka timeout ) = Max 255 en geeft aan hoeveel hops je mag maken voordat het pakketje gedropt word. (ook terug te zien in de ping output)


IPv6
- Network ID (48 bits)
- Subnet (16 bits)
- Interface ID (64 bits)


Unicast
  - Global Unicast
    - 2/3
    - public
    - routable
  
  - Link-local unicast
    - fe80
    - APIPA (maar die heb je altijd) 169.254.x.x niet routeerbaar
  
  - Unique local unicast

Multicast 


IPv6 gebruikt geen broadcasting maar ipv daarvan Multicast

Ipv6 heeft meer overhead omdat de adressen langer zijn. Eth frame heeft 1500 (ongv) bytes


# Hoofdstuk 5: 

Distance Vector protocol
  - RIP --> Maximaal 15 hops en kan zorgen voor count to infinity loop.
  - 
Linkstate protocol 
  - OSPF (Open shortest path first) --> Gebaseerd op het Dijkstra pathfinding algo
  - ospf backbone (0.0.0.0)

Border Gateway protocol (Hybdride van DVP en LSP)

Firewall types:
- Hardware 
  - Standalone appliances
- Software
- Cloud-based
- Unified Threat Management
  - Alles in 1
- Stateless inspection
  - Acts at the network layer
- Stateful inspection
  - Acts at the session layer
  

VLAN
 - Segmentation
 - Flexibility
 - Simplified Administration
 
 - To connnect VLANs in multiple switches, you must leave 1 port on the switch to link to another. This is called a trunk or a tagged port.
 - Native VLAN is een soort basis VLAN en hoeft niet getagged te worden. Als veel pakketjes via 1 vlan door de trunk komen kan het handiger zijn om die native te maken

Layer 2 en Layer 3 switches ... heeft met (switch) port verdeling te maken. #TODO

PPF Packet Filtering Firewall
1. Source port
2. Source IP
3. Destination Port
4. Destination IP
5. Protocol

NGF Next Generation Firewall (heeft ook nog een andere complexe naam)

# Hoofdstuk 6:

Je kunt processnaam achterhalen met netstat commands zonder admin rechten door het PID te vergelijken met de PID in task manager.

SLAAC (Stateless Address Autoconfiguration) Autoconfig van IPv6

DHCPv6 (Stateful Address Autoconfiguration)

EUI-64 (Interface Identifier)
7 bit van links is inverted (mac id)
interface id + host id + ff:fe
*e.g. 12:ed:23:ga:39:bc ho:st:ff:fe:id*


DHCP Relay Agent (IP Helper *CISCO term*)
 - Omdat DHCP via broadcasting informatie te weten komt, heb je een DHCPRA nodig om de IP address binnen een bepaalde scope in een ander netwerk te halen. 


DHCP stuurt ook DNS, Default Gateway, Primary Suffix ...

## DNS
De provider houd bij hoelang je in de DNS cache mag blijven.

Een lokale computer maakt een 'recursive query' naar de KPN DNS cache. Als het resultaat niet in de DNS cache kan worden gevonden, maakt deze een iterative query naar een server die kijkt naar de URL suffix (eerst .)

DNS gebruikt standaard UDP maar kan ook via TCP

Backup DNS servers worden geupdate door TCP (exclusief)

DNS types

Host record types:
  - SOA Records
  - Host Address Records
  - Mail Exchange Records  (MX)    
  - Pointer Records
  - TXT
  - Service SRV
  - Pointer PTR
  - DNS NS
  - +1

DNSSEC - Wanneer jij een dns query naar de server stuurt, geeft hij aan wie de eigenaar is van het DNS

# Hoofdstuk 7

TLS is een nieuwe versie van SSL met een aantal minder insecurities maar vrijwel hetzelfde protocol. 

Client hello = pakket 1
Server hello = pakket 2


Network Time Protocol (NTP)
- Syncs system clocks to UTC
- Use UDP on port 123
- Organized hierarchically based on distance from clock.
- Uses complex algorithms to compensate network delay and jitter.

HTTP(s)

SFTP (port 22)
FTP (File Transfer Protocol) port 23
- TCP protocol
- Passive
  - 
- Active
  - Gebruiker laat toe dat de server een connectie initieerd 


## SMB (Server Message Block)
- Purpose: Allows computers in the same network to share resources
- Usage: Windows, Linux using Samba
- SMB1 en 2 zijn niet secure
- SMB3 wel

NAS (Network Attached Storage) vs SAN (Hele Scusi verhaal)
- NAS gebruikt SMTP en NFS
- Purpose
  - Provides Remote File access
  - Concurrent resource access for multiple devices
- Components 
  - Processor, Memory, Hard drives
  - Bespoke OS, usually Linux

RDBMS - Relational Databases
Vertical scalabe

NoSQL - niet relationeel
horizontaal scalable

## SMTP (Simple Mail Transfer Protocol)
- port 25, 465 (implicit TLS), 587 (explicit TLS)
- Used for sending emails, communicate between mail servers.
- Routes emails from sender's email client to recipient's email server
- Combinable with TSL to encrypt emails

## IMAP (Internet Message Access Protocol)
- Purpose to access and manage servers remotely. Works between client and server
- Secure port 993
- Insecure port 143

## POP Post Office Protocol 
port 110
pop secure 995



## Voice en Video
- VOIP
  - Real-Time Protocol (audio streaming)
  - Session Initiation Protocol (sip)
- PBX (Private Branch Exchange)
- Voice enabled PBX
  
## Disaster Recover Concepts
- Disaster Recovery Plan (DRP)
- Table Top excercies
- Validation Tests
- Business Continuity Plan (BCP)

## Disaster Recovery Metrics
- (HA) High Availability: Ensures consistent uptime
- (MTD) Maximum Tolerable Downtime: Longest Disruption without severe impact
- (RTO) Recovery Time Objective: Time to restore services after disruption
- (WRT) Work Recovery Time: Time to confirm system/data integrity post-recovery
- (RPO) Recovery Point Objective: Maximum acceptable loss after event

## Fault Tolerance & Redundancy

## KPI (Key Performance Indicators)
- Mean time between failures (MTBF)
- Mean time to failure (MTTF)
- Mean time to repair (MTTR)

## Load Balancers
- Servers die taken verdelen

## First hop redundancy


# Hoofdstuk 8 Policies & Documentatie

Documentatie: 
  - **Configuration Management**
    - identify service assests
    - consider CMS solutions
    - identification strategy
    - configuration drift
    - establish CI management plan
  
  - **Network Device Backup Management**
    - Document backups & procedures
    - Maintain a regular backup schedule
    - audit en verify backups 
    - maintain version history
    - configure remote logging
  
  - **Change Management**
    - Establish a documentation protocol
    - Consistent use of templates
    - Version control & access management
    - incorporate a feedbackloop
    - Regularly review and update documentation
  
  - **Asset Management**
    - Update inventory documentation regularly
    - Record asset description, purchase date, service history, status and location
    - Adopt asset management software tools
    - Implement stric access controls to inventory documentation
    - Automation

  - **Network Management**
    - Physical network diagram
      - Detail hardware components
      - Record location information
      - Specify cabling details
    - Logical Network Diagrams
      - Display protocols being used
      - Organize by function vs physical location
    - IP address management


Network discovery 
 - (ze)nmap
 - angryIP
 - PRTG

Discovery protocols

Performance monitoring
  - Metrics tracking
    - 4 die je moet weten (Bandwith, throughput, CPU/Memory/ Storage)
  - Baseline establishment
  - Threshold alerts

Proactief vs reactief netwerken


## SNMP (Simple Network Managment Protocol)
- Monitor machines on the network (161), Als er iets boven een bepaalde waarde komt geeft een waarschuwing via port 162 (traps)
- Operates at the applications layer
- Uses UDP ports 161/162
- Monitor network devices
- Detect network faults
- configure remote devices
- Gebruik alleen v3


## Network Device logs
SIEM is een correlerende log manager

Log collectors zijn centralized to simply network management

Agregate log data into a single repository

Efficient
Scalable

## Packet analysis
 - tcpdump
 - wireshark
 - ngrep


## Bandwidth management

## Traffic Shaping

# Hoofdstuk 9:

## CIA triad

risico = kans x impact

## Security audits

fileless malware --> Malware dat wordt opgeslagen in het geheugen

Arp cache poisoning --> Kan worden gebruikt als je een MitM aanval wil doen door je voor te doen als de server door constant berichtjes te sturen.

MAC flooding attack

# Hoofdstuk 10:

Authentication method
 - Password
 - Smartcard
 - Fingerprint
 - Gait
 - Geofencing (GPS, IPS)
 - Time restrictions

Single Sign on 
- Kerberos SSO 
- Microsoft Defender for identity

Access Control
- DAC Discretionary Access Control (list = folder>properties>security)
- RBAC Role Based Access Control

Access Management
- Priviledged Account
- Priviledged Access Management (PAM)
- Least Privilege
- Separation of Duties


Defense in Depth
- Policies, procedures and awareness --> Physical Security --> Digital Sec:
  - Data
  - Application
  - Hst
  - Internal Network
  - Perimeter


Switch security 
 - NAC --> Network Access Control
 - Switch ports locken (digital or physical)
 - 

Port Security:
 - Secure physical Access
 - Regularly update switch firmware
 - Disable unneeded ports
 - Configure MAC filtering
 - Enbable Router advertisement Guard (RA)
 - Configure DHCP snooping
 - Implement 802.1x


Firewalls:
 - Filters all traffic and blocks/allows based on ACL
 - Ensures only permitted traffic 
 - 

Proxy servers:
 - Enforces company policies
 - Manages and redirects network traffic

Content Filtering


Common Firewall misconfigs:
 - OVerly permissive ACL
 - Overly prohibitive ACL
 - Failure to apply an implicit deny
 - Improper logging settings

# Hoofstuk 11: Network Security & Design

Zone-based security
    *Definition*
  - Network Security Model
  - Organizes network security in zones
  - Zones a region with specific security requirements 

    *Security Model*
  - Ensures that traffic flows securely between zones
  - Controls access
  - Minimizes risk

ZOnes:
- Private Security Networks
- Private Client 


Demilitarized Zone (DMZ) = Het gedeelte van je netwerk wat bereikbaar is vanaf het internet
Perimiter networks:

Screened subnet

Industrial Embeddeds systems in IoT
  - ICS
  - Supervisory Control & Data Acquisition (SCADA)

## Wireless Networking Standards

| Name     | Band        | Max Speed    |
|----------|-------------|--------------|
| 802.11a  | 5GHz        | 54 Mbps      |
| 802.11b  | 2.4GHz      | 11 Mbps      |
| 802.11g  | 2.4GHz      | 54 Mbps      |
| 802.11n  | 2.5GHz/5GHz | 600 Mbps     |
| 802.11ac | 5GHz        | Several Gbps |
| 802.11ax | 2.5GHz/5GHz | 9.6 Gbps     |


Multiuser MIMO

Bandsteering

Satelite internet  technologies
  - Microwave satellite Broadband
  - Geostationary Orbital satellites 
  - Low earth orbital

Wireless Local Area (WLAN)

BSSID

ESSID

Wireless survey - Checking strenght of intenet

Wireless Distribution System WDS  

Wi-fi protected access 2 (WPA2)

WAN 

Remote access policies
  - Transport Layer Security
  - IPsec
  - Point-to-point protocol
  - Geneting Routing Encapsulation
  - Application


Out of Band Communication Channel (OOB)