# Security Policy

## Coordinated Vulnerability Disclosure (CVD)

As a security-first MSP focused on hardened End User Computing (EUC) and sovereign AI workloads, IQ Crew AU is committed to resolving security vulnerabilities quickly and responsibly. 

We appreciate the assistance of security researchers who audit our systems and code. This policy outlines how to report vulnerabilities and our commitment to resolving them.

---

## Supported Versions

Only the latest release/state of our repositories is actively supported. Security updates will be applied to main branches and backported to long-term support (LTS) releases if explicitly defined.

| Version | Supported | Notes |
| :--- | :--- | :--- |
| Latest Main | :white_check_mark: Yes | Primary focus for all security fixes. |
| Active Releases | :white_check_mark: Yes | Backporting occurs based on severity. |
| Legacy Versions | :x: No | Users are urged to upgrade to active versions. |

---

## Reporting a Vulnerability

**DO NOT open a public GitHub issue for security-related bugs.**

If you discover a vulnerability, please report it securely through one of the following methods:

### Method 1: Encrypted Email (Preferred)
Encrypt your report using PGP and send it to: **secure-contact@iqcrew.com.au**

*   **PGP Fingerprint**: `F3C9 816D 002B A1CE 9E27 B884 892C 012B AAAA BBBB`
*   Please include:
    *   Description of the vulnerability and its potential impact.
    *   Step-by-step instructions to reproduce (proof of concept).
    *   Details of any affected environments or systems.

### Method 2: GitHub Private Vulnerability Reporting
For repositories where Private Vulnerability Reporting is enabled, use the **Security** tab to report the issue directly to the maintainers.

---

## Our Commitment

Upon receiving a valid report, the IQ Crew AU security team will:
1.  Acknowledge receipt of the report within **24 hours**.
2.  Provide a preliminary triage assessment within **72 hours**.
3.  Coordinate a timeline for remediation.
4.  Apply fixes via our automated CI/CD pipeline and release updates to affected environments.

---

## Sovereign and Hardened Data Handling
*   **Data Isolation**: All reports are handled on isolated, sovereign Australian servers.
*   **Access Control**: Access to vulnerability reports is strictly restricted to cleared, local security operations personnel.
*   **Zero Public Disclosure**: To safeguard our critical infrastructure and government clients, we do not permit public disclosure of vulnerabilities until all affected systems have been remediated.
