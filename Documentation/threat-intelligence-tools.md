# Threat Intelligence Tools

[1. Urlscan.io](#urlscanio)
[2. Abuse.ch](#abusech)
[3. Phishtool](#phishtool)
[4. Cisco Talos](#cisco-talos)


Threat Intelligence is the analysis of data and information using tools and techniques to generate meaningful patterns on how to mitigate against potential risks associated with existing or emerging threats targeting organisations, industries, sectors or governments.

To mitigate against risks, we can start by trying to answer a few simple questions:

1. Who's attacking you?
2. What's their motivation?
3. What are their capabilities?
4. What artefacts and indicators of compromise should you look out for?

There exist different types of threat intel:
- Strategic Intel
- Technical Intel
- Tactical Intel
- Operational Intel

## Urlscan.io

[Urlscan.io](https://urlscan.io/) is a free service developed to assist in scanning and analysing websites. It is used to automate the process of browsing and crawling through websites to record activities and interactions.

When a URL is submitted, the information recorded includes the domains and IP addresses contacted, resources requested from the domains, a snapshot of the web page, technologies utilised and other metadata about the website.

## Abuse.ch

Abuse.ch is a research project hosted by the Institue for Cybersecurity and Engineering at the Bern University of Applied Sciences in Switzerland. It was developed to identify and track malware and botnets through several operational platforms developed under the project. These platforms are:

_IOC: Indicator Of Compromise_

- [Malware Bazaar](https://bazaar.abuse.ch/):  A resource for sharing malware samples.
- [Feodo Tracker](https://feodotracker.abuse.ch/):  A resource used to track botnet command and control (C2) infrastructure linked with Emotet, Dridex and TrickBot.
- [SSL Blacklist](https://sslbl.abuse.ch/):  A resource for collecting and providing a blocklist for malicious SSL certificates and JA3/JA3s fingerprints.
- [URL Haus](https://urlhaus.abuse.ch/):  A resource for sharing malware distribution sites.
- [Threat Fox](https://threatfox.abuse.ch/):  A resource for sharing indicators of compromise (IOCs).
  
## Phishtool
[PhishTool](https://phistool.com) seeks to elevate the perception of phishing as a severe form of attack and provide a responsive means of email security. Through email analysis, security analysts can uncover email IOCs, prevent breaches and provide forensic reports that could be used in phishing containment and training engagements.

PhishTool has two accessible versions: Community and Enterprise. We shall mainly focus on the Community version and the core features in this task. Sign up for an account via this link to use the tool.

The core features include:

- **Perform email analysis:** PhishTool retrieves metadata from phishing emails and provides analysts with the relevant explanations and capabilities to follow the email’s actions, attachments, and URLs to triage the situation.
- **Heuristic intelligence:** OSINT is baked into the tool to provide analysts with the intelligence needed to stay ahead of persistent attacks and understand what TTPs were used to evade security controls and allow the adversary to social engineer a target.
- **Classification and reporting:** Phishing email classifications are conducted to allow analysts to take action quickly. Additionally, reports can be generated to provide a forensic record that can be shared.

## Cisco Talos

[Cisco Talos](https://talosintelligence.com/) encompasses six key teams:

- **Threat Intelligence & Interdiction:** Quick correlation and tracking of threats provide a means to turn simple IOCs into context-rich intel.
Detection Research: Vulnerability and malware analysis is performed to create rules and content for threat detection.
- **Engineering & Development:** Provides the maintenance support for the inspection engines and keeps them up-to-date to identify and triage emerging threats.
Vulnerability Research & Discovery: Working with service and software vendors to develop repeatable means of identifying and reporting security vulnerabilities.
- **Communities:** Maintains the image of the team and the open-source solutions.
- **Global Outreach:** Disseminates intelligence to customers and the security community through publications.