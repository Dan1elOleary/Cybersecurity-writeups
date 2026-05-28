# TryHackMe: AI Security

## Overview

This writeup summarizes my learning from TryHackMe's AI Security training. The course focused on common risks found in AI-enabled systems, including prompt injection, jailbreaking, sensitive information disclosure, insecure retrieval, unsafe logging, AI supply chain risks, and excessive permissions.

The purpose of this writeup is to document the security concepts practiced, the defensive controls learned, and how these topics apply to real-world cybersecurity environments.

## Skills Practiced

* Identifying AI security vulnerabilities
* Understanding OWASP LLM Top 10 concepts
* Testing retrieval boundaries in AI assistants
* Recognizing sensitive information disclosure risks
* Reviewing secure logging and redaction practices
* Understanding prompt injection and jailbreaking risks
* Documenting remediation steps for AI security issues
* Thinking from both attacker and defender perspectives

## Key Concepts Learned

### Prompt Injection

Prompt injection occurs when user-controlled input influences an AI system to ignore its intended instructions, reveal restricted information, or perform actions outside of its approved purpose.

This is especially risky when AI systems process untrusted input from emails, documents, websites, tickets, or user-submitted prompts.

### Jailbreaking

Jailbreaking attempts to manipulate the model directly into bypassing its safety rules or intended behavior. Unlike prompt injection, which often abuses how external data is mixed into the model context, jailbreaking targets the model's responses more directly.

### Sensitive Information Disclosure

AI systems can expose confidential data if they are connected to internal documents, logs, tickets, databases, or knowledge bases without proper access control.

Examples of sensitive information that should be protected include:

* Credentials
* API keys
* Internal documents
* Customer data
* Employee records
* Security incident reports
* Infrastructure details

### Retrieval-Augmented Generation Security

Retrieval-Augmented Generation, also known as RAG, allows an AI system to retrieve information from external knowledge sources before generating an answer.

A major security risk occurs when retrieval systems do not enforce proper document-level permissions. If access control is missing, a user may be able to retrieve documents they should not have permission to view.

### Secure Logging

Logs are useful for auditing and troubleshooting, but they can become a security risk if they store sensitive data.

AI system logs should avoid storing:

* Raw prompts containing sensitive information
* Retrieved confidential context
* Credentials
* Tokens
* API keys
* Personal information
* Restricted internal data

Secure logging should use redaction, minimization, and restricted access.

### AI Supply Chain Risk

AI applications often rely on third-party models, datasets, packages, plugins, and repositories. If one of these components is compromised, it may affect every application that depends on it.

Supply chain security requires validating trusted sources, reviewing dependencies, monitoring changes, and limiting what external components can influence.

## Defensive Recommendations

* Enforce document-level access control before retrieval.
* Use role-based access control or attribute-based access control.
* Apply tenant and user-level filtering in RAG systems.
* Redact sensitive information from logs.
* Avoid storing raw prompts or retrieved confidential context.
* Use least privilege for AI tools, agents, and integrations.
* Validate third-party models, packages, datasets, and plugins.
* Monitor AI systems for abnormal behavior or unexpected output.
* Sanitize model output before rendering it in applications.
* Treat all external content as untrusted input.

## Real-World Relevance

This training helped me understand how AI systems can introduce new security risks when they are connected to internal knowledge bases, automation tools, or sensitive business data.

These concepts are important for roles involving:

* SOC analysis
* Security operations
* IT support
* Cloud security
* Governance, risk, and compliance
* Application security
* AI security auditing

## Reflection

Completing this training strengthened my understanding of how traditional security principles apply to AI systems. Concepts such as least privilege, access control, secure logging, input validation, and monitoring are still critical when working with AI-enabled tools.

The biggest takeaway is that AI security is not only about the model itself. It also depends on the surrounding systems, including retrieval pipelines, logs, permissions, integrations, and supply chain components.

## Disclaimer

This writeup is for educational and portfolio purposes only. It does not include private flags, paid challenge answers, or restricted lab solutions. The focus is on skills learned, security concepts, and defensive takeaways.
