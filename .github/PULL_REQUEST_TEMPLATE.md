# Pull Request Description

## Overview
<!-- Provide a clear, concise summary of the changes made and the business case or issue resolved. -->

## Associated Issue
Closes #<!-- Issue Number -->

---

## Type of Change
- [ ] Bug fix (`fix/*`)
- [ ] New feature (`feat/*`)
- [ ] Security fix (`sec/*`)
- [ ] DevOps/CI/CD configuration (`ops/*`)
- [ ] Documentation update (`docs/*`)

---

## Checklist & Quality Standards

### Security & Compliance
- [ ] **Data Residency**: No data, configurations, or credentials route outside of Australian sovereign borders.
- [ ] **Secret Check**: Verified that no secrets, certificates, or unencrypted private credentials are included in this PR.
- [ ] **Hardening (Essential 8)**: Change aligns with relevant OS/environment hardening controls (e.g., restricted privileges, application validation).
- [ ] **Dependency Audit**: Any new dependencies have been checked for vulnerabilities and verified against our approved vendor list.

### Code Quality & Testing
- [ ] **Cryptographic Signature**: All commits in this PR are cryptographically signed.
- [ ] **Local Verification**: Tested successfully in a simulated or staging sovereign environment.
- [ ] **Clean History**: Commit history has been rebased or is prepared for a clean squash merge.
- [ ] **Documentation**: Updated relevant READMEs, architectural docs, or comments.
