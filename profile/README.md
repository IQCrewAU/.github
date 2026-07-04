# IQ Crew AU

<!-- Header section with premium badges and style -->
<p align="center">
  <a href="https://github.com/IQCrewAU">
    <img src="https://img.shields.io/badge/Sovereign-Australia-blue.svg?style=for-the-badge&color=002F6C" alt="Sovereign Australia" />
  </a>
  <a href="https://github.com/IQCrewAU">
    <img src="https://img.shields.io/badge/Compliance-ASD_Essential_Eight_L3-gold.svg?style=for-the-badge&color=D4AF37" alt="Essential Eight Level 3 Compliance" />
  </a>
  <a href="https://github.com/IQCrewAU">
    <img src="https://img.shields.io/badge/Focus-Hardened_EUC_%26_AI-black.svg?style=for-the-badge&color=111111" alt="Hardened EUC & AI" />
  </a>
</p>

***

## Executive Overview

**IQ Crew AU** is a boutique Managed Service Provider (MSP) specializing in secured, hardened End User Computing (EUC) and sovereign AI workloads. Based in Australia, we serve government, defense, critical infrastructure, and highly regulated enterprises requiring absolute assurance in data sovereignty, security posture, and workload isolation.

In an era of hyper-escalating state-sponsored cyber threats and complex regulatory landscapes, generic IT management is no longer sufficient. IQ Crew AU designs, deploys, and operates computing environments that are secure by default, resilient by design, and fully sovereign.

---

## Core Pillars & Specializations

```mermaid
graph TD
    classDef default fill:#f9f9f9,stroke:#333,stroke-width:1px;
    classDef primary fill:#e1f5fe,stroke:#0288d1,stroke-width:2px;
    classDef secondary fill:#efebe9,stroke:#5d4037,stroke-width:2px;

    P1(Hardened EUC) --> |Zero Trust Architecture| E1(Secure Virtual Desktops / AVD)
    P1 --> |Automated Patching| E2(Essential 8 Compliance)
    P2(Sovereign AI Workloads) --> |Data Residency| A1(Isolated GPU Compute)
    P2 --> |Privacy Guaranteed| A2(Local & Fine-Tuned LLMs)
    P3(Sovereign Security) --> |Continuous Monitoring| S1(Sovereign SOC Integration)
    P3 --> |Policy as Code| S2(Sovereign Supply Chain Audit)

    class P1,P2,P3 primary;
    class E1,E2,A1,A2,S1,S2 secondary;
```

### 1. Hardened End User Computing (EUC)
We design zero-trust client virtualization and physical endpoint management solutions tailored to the strictest classification levels.
*   **Hardened Desktops**: Custom operating system builds (Windows, macOS, Linux) optimized for security, with complete driver auditing, strict app control policies, and aggressive hardening profiles.
*   **Virtual Desktop Infrastructures (VDI)**: High-performance, low-latency, and hardened environments using Azure Virtual Desktop (AVD), Windows 365, or specialized on-premise private clouds.
*   **Zero-Trust Endpoint Management**: Continuous verification, micro-segmentation at the client level, and integration with passwordless, phish-resistant authentication schemes.

### 2. Sovereign AI Workloads
Integrating artificial intelligence into business processes requires absolute control over intellectual property and models.
*   **Private & Isolated LLMs**: Deployment of open-weights and custom models inside your secure boundaries, ensuring training data and prompts never leave your designated sovereign environment.
*   **Hardened AI Pipelines**: End-to-end security for AI systems, from vector databases and retrieval-augmented generation (RAG) datasets to API endpoints.
*   **Sovereign GPU Orchestration**: Automated deployment and scaling of secure GPU instances hosted exclusively within Australian sovereign data centers.

### 3. Sovereign Compliance & Governance
We ensure workloads comply with Australian government frameworks and sovereign data laws.
*   **ASD Essential Eight**: Hardening of IT environments to Level 3 maturity, implementing strict application control, patch management, restricted admin privileges, and user application hardening.
*   **IRAP Readiness**: Aligning architectures and evidence structures with the Information Security Manual (ISM) to streamline assessment and certification by IRAP assessors.
*   **Data Residency & Sovereignty**: Assurances that data, metadata, transit routes, and support personnel reside strictly within Australia.

---

## The Sovereign Advantage

Unlike generalist MSPs, our operational model is optimized for sovereign risk management:

| Operational Dimension | Standard MSP | IQ Crew AU |
| :--- | :--- | :--- |
| **Data Residency** | Global transit & storage allowed | Strictly restricted to Australian territory |
| **Support Staff** | Offshore / Follow-the-sun model | Australian citizens with security clearances |
| **System Hardening** | Basic template-based security | Continuous policy-as-code hardening (Essential 8 L3) |
| **AI Data Processing** | Multi-tenant public cloud APIs | Single-tenant private environments with isolated data |
| **Supply Chain Validation** | Standard vendor procurement | Software Bill of Materials (SBOM) & vendor risk auditing |

---

## Contact & Collaboration

IQ Crew AU operates on a trust-first foundation. For project engagements, architectural consultations, or vulnerability notifications:

*   **Secure Communications**: We recommend using PGP-encrypted email for sensitive inquiries.
*   **PGP Fingerprint**: `F3C9 816D 002B A1CE 9E27 B884 892C 012B AAAA BBBB`
*   **Inquiries**: secure-contact@iqcrew.com.au
