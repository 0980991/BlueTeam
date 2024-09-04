# Cyber Defense Frameworks

- [Cyber Defense Frameworks](#cyber-defense-frameworks)
  - [Pyramid of Pain](#pyramid-of-pain)
  - [Cyber Kill Chain](#cyber-kill-chain)
  - [Unified Kill **Chain**](#unified-kill-chain)
## Pyramid of Pain
The pyramid of pain is a framework which describes the impact an indicator of compromise may have on the adversary when denied by a Blue Team.

There are 6 indicators.
![Alt](img/blog-pyramid-pain-01.jpg)

**1. Hash values**

SHA1, MD5, or other similar hashes that correspond to specific suspicious or malicious files. Hash values are often used to provide unique references to specific samples of malware or to files involved in an intrusion.

**2. IP addresses**

As the name suggests, but also includes netblocks.

**3. Domain names**

A domain name itself, or sub domains.

**4a. Network Artifacts**

Adversaries’ network activities that are observable. Typical examples include URI patterns, C2 information embedded in network protocols, distinctive HTTP User-Agent, or SMTP Mailer values, etc.

**4b. Host Artifacts**

Observables caused by adversary activities on one or more of your hosts, such as registry keys or values known to be created by specific pieces of malware, files, or directories.

**5. Tools**

Software used by attackers to accomplish their mission. This includes utilities designed to create malicious documents for spear phishing, backdoors used to establish C2 or password crackers, or other host-based utilities

**6. Tactics, Techniques and Procedures (TTPs)**

How the adversary goes about accomplishing their mission, from reconnaissance all the way through data exfiltration and at every step in between.

*src: [What is the pyramid of pain?](https://www.attackiq.com/glossary/pyramid-of-pain/)*

## Cyber Kill Chain
The Cyber Kill Chain framework is designed for identification and prevention of the network intrusions. The framework defines the steps used by adversaries or malicious actors in cyberspace. To succeed, an adversary needs to go through all phases of the Kill Chain.

There are generally 7 steps in the Cyber Kill Chain:
![alt text](img/cyber-kill-chain.png)

**1. Reconnaissance**

Reconnaissance is discovering and collecting information on the system and the victim. The reconnaissance phase is the planning phase for the adversaries *e.g. OSINT*

combines malware and exploit into a deliverable payload. 

**2. Weaponization**

This is the process of combining malware and an exploit into a deliverable payload using the information found during the reconaissance phase *e.g. creating a malicious MS Word macro*

**3. Delivery**

Te method for transmitting the payload or the malware. For the malware to reach the machine of a victim, the adversary must deliver the malware to the victim. This is often done remotely using (spear)phishing but in some cases require physical delivery *e.g. distributing malicious USB sticks*. 


**4. Exploitation**



**5. Installation**

**6. Command & Control**

**7. Actions on Objectives**


## Unified Kill **Chain**