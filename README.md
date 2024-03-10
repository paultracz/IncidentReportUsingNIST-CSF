# IncidentReportUsingNIST-CSF
An security incident report done for a fictional multimedia company as a part of the Google Cybersecurity Certificate

# Table of contents
1. [Activity Overview](#activity-overview)
2. [Scenario](#scenario)
3. [Incident Report Analysis](#incident-report-analysis)

# Activity Overview
Create an incident report using the knowledge you’ve gained about networks throughout this course to analyze a network incident. You will analyze the situation using the National Institute of Standards and Technology's Cybersecurity Framework (NIST CSF). This is an activity in the [Google Cybersecurity Professional Certificate](https://www.coursera.org/google-certificates/cybersecurity-certificate). The goal is to create a quality cybersecurity incident report and by applying the CSF, you will demonstrate a proactive approach to security, improving communication and transparency with stakeholders, and improve security practices within your organization.

# Scenario
You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DDoS attack, which compromised the internal network for two hours until it was resolved.

During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 

The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 

● To address this security event, the network security team implemented: 

● A new firewall rule to limit the rate of incoming ICMP packets

● Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets

● Network monitoring software to detect abnormal traffic patterns

● An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics

# Incident Report Analysis

| Function | Description |
|--------------------|---------------|
| Summary | The organization experienced a two hour disruption of critical network services due to a DDoS attack involving a flood of ICMP packets. Through the investigation of the cybersecurity team, it was discovered that the attack exploited an unconfigured firewall that allowed a threat actor to overwhelm the network. The incident management team promptly responded by blocking incoming ICMP packets, temporarily taking non-critical services offline, and restoring critical services. This led to the implementation of new firewall rules and network monitoring systems that will mitigate future incidents. The impact of the attack included business disruption, potential revenue loss, and reputational damage due to service downtime. |
| Identify   | The organization experienced a distributed denial-of-service (DDoS) attack, more specifically an ICMP flood attack. The network was flooded with ICMP packets that caused it to become congested. As a result, internal users were unable to access network resources, affecting productivity and operations within the organization. | 
| Protect  | The network security team implemented a new firewall rule to limit the rate of incoming ICMP packets and an IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics.  |
| Detect | To detect any similar and new network attacks in the future, the team implemented network monitoring software to detect abnormal traffic patterns, as well as source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets.  | 
| Respond  |For future related security events, the team will immediately isolate affected devices or systems from the network to prevent any spread of the incident. They will deploy firewall rules to prevent the malicious attack from continuing. The team will also use an IDS/IPS system that will actively monitor and block malicious traffic. Then, the team will collect and analyze the network traffic logs, system logs, and security event data to identify any indicators of compromise (IOC’s) and determine the scope of the incident. Lastly they should update any relevant incident response playbooks to improve future procedures. |
| Recover | To recover from a DDoS attack by ICMP flooding, access to the network services must be restored to normal functioning states. In the future, external ICMP flood attacks can be blocked at the firewall. Then, all non-critical network services should be stopped to reduce internal network traffic. Next, critical network services should be restored first. Finally, once the flood of ICMP packets have timed out, all non-critical network systems and services can be brought back online. |
