# TryHackMe: Red Team Engagements

## Overview

This writeup summarizes my learning from TryHackMe's Red Team Engagements training. The course focused on the planning, documentation, structure, and rules required to conduct authorized red team operations in a professional and controlled manner.

The purpose of this writeup is to document the engagement planning concepts practiced, the documentation types reviewed, and how red team planning supports safe, legal, and effective security testing.

## Skills Practiced

* Understanding the purpose of red team engagements
* Reviewing rules of engagement documentation
* Learning how a Concept of Operations document is structured
* Understanding resource planning for red team operations
* Identifying engagement scope and limitations
* Understanding timelines, objectives, and client expectations
* Recognizing the importance of authorization and communication
* Connecting offensive security planning to defensive improvement
* Documenting engagement details in a professional format

## Key Concepts Learned

### Red Team Engagements

A red team engagement is an authorized security assessment designed to emulate real-world adversary behavior. The goal is to test an organization's people, processes, and technology against realistic attack scenarios.

Unlike a basic vulnerability scan or standard penetration test, a red team engagement often focuses on objectives, stealth, detection capability, and the organization's ability to respond to live threats.

### Rules of Engagement

Rules of Engagement, also known as ROE, define what is allowed and not allowed during a security assessment.

The ROE helps protect both the client and the red team by clearly defining the scope, boundaries, testing windows, approved techniques, communication procedures, and escalation paths.

Important ROE details may include:

* Authorized targets
* Out-of-scope systems
* Approved testing dates and times
* Allowed attack methods
* Prohibited techniques
* Emergency contacts
* Reporting expectations
* Deconfliction procedures
* Legal authorization

### Concept of Operations

A Concept of Operations, also known as CONOPS, provides a high-level overview of how an engagement will be conducted.

The CONOPS is usually written in a semi-technical style so both technical and non-technical stakeholders can understand the plan.

A CONOPS may include:

* Client name
* Service provider
* Engagement timeframe
* General objectives
* Planned phases
* Training objectives
* High-level tools and techniques
* Threat group emulation, if applicable

### Resource Planning

A resource plan outlines the personnel, dates, tools, infrastructure, and other resources needed to complete the engagement.

Unlike the CONOPS, the resource plan is usually more structured and direct. It may use bullet points, tables, or clearly separated sections.

A resource plan may include:

* Red cell lead
* Assistant cell lead
* Operators
* Engagement dates
* Reconnaissance dates
* Initial access dates
* Post-exploitation dates
* Cloud resource requirements
* Hardware requirements
* Budget details
* Miscellaneous requirements

### Engagement Scope

Scope defines what systems, users, networks, applications, or environments are authorized for testing.

A clearly defined scope helps prevent accidental impact to systems that were not approved for testing.

Examples of scope considerations include:

* IP ranges
* Domains
* Applications
* Physical locations
* User groups
* Cloud environments
* Third-party systems
* Excluded assets

### Threat Emulation

Threat emulation involves modeling an engagement after a real-world adversary or threat group. This helps organizations test their defenses against tactics, techniques, and procedures that are relevant to their industry or risk profile.

Threat emulation may include:

* Reconnaissance
* Initial access
* Credential access
* Lateral movement
* Persistence
* Command and control
* Exfiltration simulation
* Detection testing

### Communication and Deconfliction

Communication is critical during a red team engagement. The red team, blue team, white cell, and client stakeholders need clear communication channels and escalation procedures.

Deconfliction helps ensure that authorized red team activity is not mistaken for an actual malicious attack without proper escalation.

## Defensive Takeaways

* Red team engagements should always have clear authorization.
* Rules of engagement must define scope, limits, and approved techniques.
* Testing should be planned to reduce unnecessary business disruption.
* Communication paths should be established before the engagement begins.
* Documentation helps both the red team and client understand expectations.
* Red team activity should support defensive improvement, not just exploitation.
* Lessons learned should be used to improve detection, response, and security controls.

## Real-World Relevance

This training is relevant to cybersecurity roles that involve penetration testing, security operations, risk management, governance, and incident response.

Understanding red team engagement planning is useful even for defensive roles because it explains how offensive security teams structure assessments and how organizations can prepare for realistic adversary simulations.

These concepts are important for roles involving:

* Penetration testing
* Red team operations
* SOC analysis
* Security engineering
* Incident response
* Governance, risk, and compliance
* Vulnerability management
* Security consulting

## Reflection

This training helped me understand that red team work is not only about technical exploitation. A successful engagement also depends on planning, documentation, communication, scope control, authorization, and professional reporting.

The biggest takeaway is that red team operations must be structured and controlled. Proper planning documents such as the ROE, CONOPS, and resource plan help ensure that testing is legal, safe, measurable, and aligned with the client's objectives.

## Disclaimer

This writeup is for educational and portfolio purposes only. It does not include private flags, paid challenge answers, or restricted lab solutions. The focus is on skills learned, security concepts, and professional documentation.
