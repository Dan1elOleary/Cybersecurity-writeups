TryHackMe Grep — OSINT & Web Reconnaissance Lab


Overview

This repository documents my notes and methodology for the TryHackMe Grep room, an OSINT and reconnaissance-based challenge from TryHackMe’s Red Teaming path.

The lab focuses on using publicly available information, web application enumeration, source-code review, and basic exploitation techniques to identify sensitive data and gain access to a vulnerable web application.

The purpose of this repository is to demonstrate my understanding of reconnaissance workflows, OSINT techniques, and secure handling of sensitive findings during a web application assessment.

Lab Objective

The objective of the lab was to assess a newly developed blogging platform created by a fictional company and identify weaknesses that could be discovered through open-source intelligence and web reconnaissance.

The main goals included:

Discovering exposed or leaked application information
Identifying sensitive data in publicly available sources
Finding an API key used for user registration
Registering and accessing the application
Locating user and administrative information
Using OSINT techniques to identify related services
Understanding how poor secret management can lead to account compromise
Skills Practiced
OSINT Research

This lab required searching publicly available sources for information related to the target application and organization.

Skills practiced included:

Searching for public references to the target company
Reviewing exposed documentation or repositories
Looking for leaked credentials, API keys, or configuration details
Identifying related domains, hostnames, and services
Web Application Reconnaissance

The lab involved reviewing the web application for exposed routes, hidden pages, and useful client-side information.

Skills practiced included:

Inspecting page source
Reviewing JavaScript files
Checking common web paths
Looking for exposed API endpoints
Identifying registration and authentication workflows
Source Code Review

The challenge emphasized reviewing publicly available or exposed code for sensitive information.

Skills practiced included:

Searching source files for secrets
Reviewing comments and configuration files
Identifying hardcoded API keys
Understanding how leaked development artifacts can impact security
Command-Line Searching

The room title, Grep, highlights the importance of searching through files efficiently.

Commands and techniques used included:

grep -Rni "api" .
grep -Rni "key" .
grep -Rni "token" .
grep -Rni "admin" .
grep -Rni "email" .
grep -Rni "password" .
grep -Rni "leak" .
Tools Used
Web browser
Browser Developer Tools
Linux command line
grep
curl
wget
Directory enumeration tools
Public search engines
GitHub search
/etc/hosts file modification for hostname testing
Methodology
1. Initial Web Application Review

The first step was to access the deployed lab machine and review the visible web application.

This included checking:

Home page content
Login and registration pages
Page source
JavaScript files
Cookies and local storage
Visible links and routes

The goal was to identify how the application worked and whether any useful information was exposed to unauthenticated users.

2. Directory and Endpoint Enumeration

After reviewing the visible application, directory enumeration was used to identify hidden routes and API endpoints.

Example enumeration targets included:

/login
/register
/admin
/api
/assets
/js
/config
/docs
/robots.txt
/sitemap.xml

This step helped identify areas of the application that were not directly linked from the main page.

3. Public Source Investigation

Because this was an OSINT-focused room, public sources were reviewed for information related to the fictional company and application.

This included searching for:

Company name
Application name
API key references
Registration logic
Admin user information
Password leak references
Related hostnames

The purpose of this step was to identify sensitive information that may have been accidentally published outside of the application itself.

4. Sensitive Data Discovery

During the lab, sensitive data was discovered through reconnaissance and source review.

Examples of sensitive data types included:

API keys
User information
Admin email address
Related service hostnames
Password leak information

For security and ethical reasons, this public writeup does not include real challenge answers, flags, passwords, or API keys.

5. Registration and Authentication Testing

Once the registration mechanism was understood, the discovered API key was used to register an account on the application.

After registering, authenticated areas of the application were reviewed for additional information.

This step demonstrated how leaked API keys can allow unauthorized users to access restricted functionality.

6. Hostname Discovery

The lab also required identifying a related hostname used for checking whether an email was involved in a possible password leak.

This reinforced the importance of reviewing public references, source code, and configuration data for related infrastructure.

In a real-world assessment, exposed hostnames can expand the attack surface and reveal additional services that may need to be secured.

7. Credential Exposure Analysis

After identifying the admin email, the related password leak checking service was used to investigate whether credentials had been exposed.

This part of the lab demonstrated how reused or leaked credentials can lead to unauthorized access, especially when combined with OSINT findings.

Key Takeaways
Exposed Secrets Are High Risk

Hardcoded API keys, credentials, and tokens should never be committed to public repositories or exposed in client-side files.

Even a single leaked API key can allow attackers to register accounts, access restricted functionality, or pivot deeper into an application.

OSINT Can Reveal Critical Information

Attackers do not always need advanced exploitation techniques. Public search engines, GitHub repositories, documentation, comments, and exposed files can provide enough information to compromise an application.

Client-Side Code Should Not Contain Secrets

JavaScript files, frontend configuration files, and browser-accessible assets should be treated as public. Secrets stored in client-side code can be discovered by anyone.

Reconnaissance Should Be Methodical

A structured recon process helps avoid missing important details. Reviewing source code, endpoints, public references, and related infrastructure provides a stronger understanding of the target.

Credential Reuse Increases Risk

If an admin account uses a password that appears in a leak or reused credential list, attackers may be able to gain access without exploiting a technical vulnerability.

Defensive Recommendations

To reduce the risks demonstrated in this lab, organizations should:

Remove secrets from public repositories
Rotate exposed API keys and credentials immediately
Store secrets in secure vaults or environment variables
Avoid placing sensitive data in frontend code
Enforce strong authentication controls
Implement multi-factor authentication for admin accounts
Monitor public repositories for leaked secrets
Review application logs for suspicious registration or login activity
Restrict sensitive API endpoints
Conduct regular OSINT reviews against company assets
What This Lab Demonstrates

This lab demonstrates practical experience with:

OSINT methodology
Web application reconnaissance
Sensitive data discovery
Source-code review
API key exposure risks
Authentication workflow testing
Credential exposure analysis
Secure documentation practices
Professional Summary

The TryHackMe Grep room helped reinforce how reconnaissance and OSINT can expose serious security weaknesses in web applications.

This lab was valuable because it showed that attackers often succeed by finding overlooked information rather than exploiting complex vulnerabilities. Publicly exposed source code, leaked secrets, weak credential practices, and related infrastructure can all contribute to application compromise.

By documenting this lab, I am demonstrating my ability to approach a target methodically, identify exposed information, understand the security impact, and communicate findings in a professional way.

Disclaimer

This repository is for educational and professional development purposes only.

No real flags, passwords, API keys, or challenge answers are included in this writeup. The content is intended to document methodology and lessons learned while respecting TryHackMe’s challenge integrity.
