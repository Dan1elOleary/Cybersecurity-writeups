# TryHackMe: SOC Level 1 Learning Path

## Overview

This writeup summarizes my learning from TryHackMe's SOC Level 1 learning path. The training focuses on the foundational skills needed to work as a Security Operations Center analyst, including blue team operations, alert triage, log analysis, endpoint monitoring, incident response, and threat detection.

The purpose of this writeup is to document the security concepts practiced, the analyst skills being developed, and how these topics apply to real-world SOC and IT security environments.

## Skills Practiced

* Understanding the role of a SOC analyst
* Reviewing security alerts and suspicious activity
* Learning blue team defensive operations
* Identifying human and system attack vectors
* Understanding common network and web attacks
* Practicing log review and event analysis concepts
* Learning endpoint monitoring fundamentals
* Understanding SIEM usage for security investigations
* Documenting findings for escalation or remediation
* Thinking from a defensive security and incident response perspective

## Key Concepts Learned

### Security Operations Center

A Security Operations Center, also known as a SOC, is a centralized team responsible for monitoring, detecting, investigating, and responding to cybersecurity threats.

SOC analysts review alerts, analyze logs, investigate suspicious behavior, and help protect an organization from security incidents.

### Blue Team Operations

Blue team operations focus on defending systems, networks, applications, and users from cyber threats.

This includes monitoring security tools, reviewing alerts, identifying suspicious activity, responding to incidents, and improving defensive controls.

### Alert Triage

Alert triage is the process of reviewing security alerts to determine whether they are false positives, low-risk events, or potential security incidents.

A SOC analyst must consider the source of the alert, affected asset, user activity, severity, and supporting evidence before deciding the next step.

### Log Analysis

Logs provide important evidence during a security investigation. They can show user activity, authentication attempts, network connections, system changes, and application behavior.

Common logs that may be reviewed include:

* Windows event logs
* Authentication logs
* Firewall logs
* Web server logs
* Endpoint detection logs
* SIEM alerts
* Network traffic logs

### Endpoint Monitoring

Endpoint monitoring focuses on identifying suspicious activity on devices such as workstations, laptops, and servers.

Examples of suspicious endpoint activity include:

* Unusual process execution
* Malware detections
* Suspicious PowerShell activity
* Unauthorized software installation
* Unexpected network connections
* Abnormal login behavior
* Changes to security settings

### Network and Web Attacks

SOC analysts need to understand common attack techniques used against networks and web applications.

Examples include:

* Phishing
* Brute-force attacks
* Credential theft
* Malware infections
* Web application attacks
* Command injection
* SQL injection
* Unauthorized access attempts
* Lateral movement

### Incident Response

Incident response is the process of identifying, containing, investigating, and remediating a security incident.

A basic incident response workflow may include:

* Detection
* Triage
* Containment
* Investigation
* Remediation
* Recovery
* Documentation
* Lessons learned

### SIEM Concepts

A Security Information and Event Management system, also known as a SIEM, collects and analyzes logs from multiple sources.

SIEM tools help analysts identify suspicious activity, correlate events, prioritize alerts, and investigate possible incidents.

## Defensive Recommendations

* Monitor authentication logs for suspicious login activity.
* Review endpoint alerts for malware, suspicious scripts, and abnormal behavior.
* Use SIEM correlation rules to identify patterns across multiple systems.
* Prioritize alerts based on severity, asset importance, and business impact.
* Document investigation steps clearly for escalation.
* Apply least privilege to user accounts and administrative access.
* Keep systems patched and updated.
* Use endpoint detection and response tools to monitor device activity.
* Train users to recognize phishing and social engineering attacks.
* Review incident response procedures regularly.

## Real-World Relevance

This training is directly relevant to entry-level SOC analyst, IT support, and cybersecurity support roles. Many SOC responsibilities involve reviewing alerts, checking logs, documenting findings, escalating incidents, and supporting remediation efforts.

The concepts learned in this path also connect to managed service provider environments, where technicians may assist with endpoint alerts, Microsoft 365 security events, suspicious login activity, malware detections, and user account issues.

These concepts are important for roles involving:

* SOC analysis
* Security operations
* IT support
* Managed services
* Endpoint security
* Incident response
* Vulnerability management
* Identity and access monitoring

## Reflection

Working through the SOC Level 1 learning path is helping me better understand how security teams detect and respond to threats in real-world environments. It reinforces the importance of careful alert review, clear documentation, log analysis, and structured investigation methods.

The biggest takeaway is that SOC analysis is not only about using tools. It also requires understanding attacker behavior, knowing what normal activity looks like, asking the right questions, and documenting findings clearly so the correct response can be taken.

## Disclaimer

This writeup is for educational and portfolio purposes only. It does not include private flags, paid challenge answers, or restricted lab solutions. The focus is on skills learned, security concepts, and defensive takeaways.
