# IQ Crew AU GitHub Configuration & Management (.github)

This repository serves as the central configuration and governance repository for the **IQ Crew AU** GitHub organization. It defines organization-wide defaults, security policies, contribution standards, issue templates, and automated repository settings.

## Organization Design Philosophy

For a sovereign-focused Managed Service Provider, speed must not compromise security. We utilize **Configuration as Code (CasC)** and **DevSecOps** mechanisms to ensure that all repositories under the `IQCrewAU` organization are automated, standardized, and audit-ready from day one.

---

## Recommended Organization Settings

To maintain a secure, compliant, and highly performant organization, the following configurations should be applied at the GitHub Organization settings level:

### 1. Security & Analysis
Navigate to **Organization Settings -> Code security and analysis** and enable:
*   **Dependency Graph**: Enabled (critical for vulnerability tracking).
*   **Dependabot Alerts**: Enabled.
*   **Dependabot Security Updates**: Enabled (automatically creates PRs for vulnerable dependencies).
*   **GitHub Advanced Security**: Enabled (for private repositories where license permits).
*   **CodeQL Code Scanning**: Enabled (with Default configuration for supported languages).
*   **Secret Scanning**: Enabled (includes scanning for partner patterns).
*   **Push Protection**: **Enabled** (prevents developers from pushing secrets to any repository).

### 2. Member Permissions & Repository Defaults
Navigate to **Organization Settings -> Member privileges**:
*   **Base Permissions**: Set to **Read** or **None**. Developers should only have write access via explicit team assignments.
*   **Repository Creation**: Restrict creation of public and private repositories to Organization Administrators to prevent shadow IT and accidental data leaks.
*   **Repository Deletion**: Restricted to Administrators only.
*   **Forking**: Disabled for private repositories containing client configuration, threat models, or proprietary workloads.
*   **Repository visibility changes**: Restricted to Administrators only.

### 3. Repository Defaults & Automation
All new repositories must be instantiated using authorized templates containing baseline configurations.
*   **Default branch name**: `main`.
*   **Required signed commits**: Enabled globally to guarantee audit trails and prevent identity spoofing.

---

## Directory Layout

*   [`/profile/README.md`](file:///Users/justyngreen/Repos/IQ%20Crew/.github/profile/README.md): Displays on the organization's public landing page. Contains the business overview and focus areas.
*   [`/SECURITY.md`](file:///Users/justyngreen/Repos/IQ%20Crew/SECURITY.md): Default vulnerability disclosure policy.
*   [`/CONTRIBUTING.md`](file:///Users/justyngreen/Repos/IQ%20Crew/CONTRIBUTING.md): Git standards, commit signature requirements, and coding guidelines.
*   [`/CODE_OF_CONDUCT.md`](file:///Users/justyngreen/Repos/IQ%20Crew/CODE_OF_CONDUCT.md): Professional and respectful workplace standards.
*   [`/.github/PULL_REQUEST_TEMPLATE.md`](file:///Users/justyngreen/Repos/IQ%20Crew/.github/PULL_REQUEST_TEMPLATE.md): Standardized pull request quality and security checklist.
*   [`/.github/ISSUE_TEMPLATE/`](file:///Users/justyngreen/Repos/IQ%20Crew/.github/ISSUE_TEMPLATE/): Folder containing standardized issue forms.
*   [`/.github/settings.yml`](file:///Users/justyngreen/Repos/IQ%20Crew/.github/settings.yml): Repository Settings-as-Code file.

---

## Repository Settings as Code (`settings.yml`)

We manage repository settings declaratively using a `settings.yml` workflow (compatible with Probot Settings or GitHub Actions). 

### Key Configured Rules:
1.  **Strict Branch Protection**:
    *   No direct pushes to `main`. All changes require an approved Pull Request.
    *   Minimum of 1 approved review from a designated team lead.
    *   Required status checks (e.g., CI, CodeQL, linting) must pass before merging.
    *   Linear history required (no merge commits, only squash or rebase).
2.  **Commit Enforcement**:
    *   All commits must be signed using GPG or SSH keys.
3.  **Collaborator Management**:
    *   Permissions are team-based, not individual-based.
