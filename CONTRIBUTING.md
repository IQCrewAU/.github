# Contributing to IQ Crew AU Projects

Thank you for contributing to IQ Crew AU. To maintain our high standards of security, sovereign compliance, and engineering speed, we enforce strict controls over codebase additions.

---

## Coding and Security Guidelines

Before making any changes, ensure you align with our core standards:

1.  **Security by Design**: Never hardcode API keys, certificates, passwords, or personal identifying information (PII). All configurations must pull secrets from secure key vaults (e.g., Azure Key Vault, HashiCorp Vault) or GitHub secrets.
2.  **Sovereign Data Boundaries**: Ensure that code, logs, and external resource dependencies (such as public AI model APIs or non-sovereign CDNs) do not route or leak data outside Australia.
3.  **ASD Essential Eight Controls**: Software configuration must conform to application control and user hardening specifications. Ensure no unsigned binaries are executed.

---

## Commit & Branching Standards

### 1. Mandatory Commit Signing
All commits must be cryptographically signed (GPG, SSH, or S/MIME). Commits without valid signatures will be automatically rejected by branch protection rules.

To configure signing:
```bash
git config --global user.signingkey <YOUR_KEY_ID>
git config --global commit.gpgsign true
```

### 2. Branch Naming Conventions
Always create a branch for your work. Do not push directly to `main`. Use the following prefixes:
*   `feat/` - New features or capabilities (e.g., `feat/hardened-avd-image`)
*   `fix/` - Bug fixes and stability improvements (e.g., `fix/gpu-allocation-timeout`)
*   `sec/` - Security patches, updates, and threat mitigations (e.g., `sec/remediate-cve-xyz`)
*   `ops/` - Infrastructure, CI/CD pipelines, and tool configurations (e.g., `ops/update-terraform-provider`)
*   `docs/` - Documentation-only updates (e.g., `docs/add-architecture-diagrams`)

### 3. Commit Messages
We follow the Conventional Commits specification. Messages should be structured as:
```text
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```
Example:
```text
feat(avd): add automated local policy hardening rules for ASD E8 L3 compliance
```

---

## Pull Request Workflow

1.  **Create your Branch**: Derive your branch from the latest `main` branch.
2.  **Run Pre-Commit Hooks**: Ensure local linting, testing, and secret scanning checks (such as `trufflehog` or `gitleaks`) pass.
3.  **Open a Pull Request**: Use the provided PR Template. Connect your PR to a corresponding GitHub issue.
4.  **Security Scan & Status Checks**: All automated tests, vulnerability scanners (CodeQL, Dependabot), and formatters must pass.
5.  **Code Review**: At least one approved review from an administrator or designated team leader is required.
6.  **Merge**: Once approved, select **Squash and Merge** to maintain a clean, linear commit history on `main`.
