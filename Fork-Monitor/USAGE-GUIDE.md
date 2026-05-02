# AIC Fork Monitor Usage Guide

**Version 1.0** — April 2026
**Managed by**: AIC-Legal-and-Governance

## 1. Introduction

AIC-Fork-Monitor is a fork monitoring system designed specifically for Adaptive Intelligence Circle.

It is a crucial part of the **Governance Framework**, helping to protect licenses, core principles (Third Path Absolute, Zero-Donation, Ethical-from-kernel), and create legal evidence when necessary.

This system **is not intended to prohibit forks**, but to ensure that forks are performed transparently and respect the project's principles.

## 2. Main Purposes

- To record and monitor all public forks of AIC repositories.

- To detect early violations of licenses or core principles.

- To create transparent data and lasting legal evidence.

- Protecting AIC's identity and independence.

## 3. How the system works

- The `monitor-forks.py` script periodically scans all forks via the GitHub API.

- Data is saved to `fork-log.csv` and the `logs/` directory.

- Violating forks are manually recorded in `COMPLIANCE-VIOLATIONS.md`.

- The entire process is public to ensure transparency.

## 4. Usage instructions

### For Contributors/Maintainers
- When forking any AIC repository, please:

- Keep the GPLv3 + OpenMDW-1.0 license intact.

- Do not delete or modify `FORK-AND-COMPLIANCE-POLICY.md`.

- Publicly acknowledge this as an AIC fork in the README.

- Respect Zero-Donation and Third Path Absolute.

### For TSC / Trusted Admin
- Regularly check `fork-log.csv` and `COMPLIANCE-VIOLATIONS.md`.

- Assess the compliance status of major forks.

- Report suspicious forks to the Founder.

### For Founder
- Make the final decision on handling serious violations (public notice, Cease & Desist, DMCA, litigation).

## 5. Levels of Violation

- **Compliant**: Fork fully compliant.

- **Under Review**: Under review.

- **Minor Violation**: Removal of attribution, minor license changes → request for correction within 14 days.

- **Serious Violation**: Removal of policy, changes to core principles, unauthorized commercial use → public notice + legal action.

## 6. Related Policy Links

- [FORK-AND-COMPLIANCE-POLICY.md](./FORK-AND-COMPLIANCE-POLICY.md)

- [ZERO-DONATION-POLICY.md](../ZERO-DONATION-POLICY.md)

- [THIRD-PATH-PRINCIPLES.md](../THIRD-PATH-PRINCIPLES.md)

- [SECURITY-DISCLOSURE-POLICY.md](./SECURITY-DISCLOSURE-POLICY.md)

---
**Commitment**:

We believe that true Open Source must come with responsibility and transparency. The Fork Monitor system is a tool to protect that spirit.

— Nguyen Duc Tri, Founder & Lead Architect
Adaptive Intelligence Circle