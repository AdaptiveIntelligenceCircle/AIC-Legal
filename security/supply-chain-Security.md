# Supply-Chain Security Considerations

**Adaptive Intelligence Circle Foundation (AIC)**  
**Version:** 0.1 (Draft)  
**Last updated:** October 2026  
**Status:** Pre-Covenant guidance

---

## 1. Purpose

This document records AIC’s current approach to software supply-chain risk.  

AIC develops open-source protocol and infrastructure components. We aim to keep the attack surface visible, the build and dependency process understandable, and the introduction of untrusted code difficult by default.

This is guidance and current practice, not a certification or guarantee of supply-chain integrity.

---

## 2. Guiding Principles

- Prefer minimal, auditable dependencies.
- Prefer well-known, actively maintained libraries over obscure or abandoned ones.
- Treat any new dependency as a potential trust decision that should be reviewable.
- Keep build and release processes as simple and reproducible as practical.
- Align with the spirit of Ethical-from-kernel: critical paths should not silently depend on opaque external components.

---

## 3. Current Practices (as of October 2026)

### 3.1 Dependency Management

- New dependencies should be justified in the corresponding pull request or design note.
- Prefer language ecosystems and package sources that support verification (checksums, signed releases, lockfiles).
- Periodic review of high-impact dependencies is encouraged, especially those touching authorization, cryptography, networking, or agent execution.

### 3.2 Build & Release

- Aim for reproducible or at least inspectable builds where the technology stack allows.
- Release artifacts should be associated with clear commit hashes and, when practical, signatures or attestations.
- Avoid complex multi-stage pipelines that obscure the origin of binaries.

### 3.3 Third-Party Code & Contributions

- External contributions are welcome under the project’s contribution guidelines.
- Changes that affect security-sensitive areas (authorization, refusal logic, human-gating, cryptographic primitives, supply-chain tooling itself) require elevated review.
- Binary or opaque blobs are strongly discouraged unless there is a documented, exceptional justification.

### 3.4 Secrets & Credentials

- No long-lived secrets should appear in public repositories.
- Any operational credentials are managed outside the public source tree and follow least-privilege principles.

---

## 4. Alignment with External Frameworks

AIC monitors relevant international and regional developments, including:

- Concepts from NIST SP 800-161 (Cybersecurity Supply Chain Risk Management)
- Emerging requirements under the EU Cyber Resilience Act (CRA) and related guidance
- Common open-source supply-chain practices (lockfiles, SBOMs where useful, provenance)

AIC does not claim formal compliance with any specific regulation at this stage. As a small, non-profit-oriented project, we focus on practical, proportionate measures rather than heavyweight certification.

---

## 5. Limitations & Under-claim

- AIC cannot guarantee that every transitive dependency is free of vulnerabilities.
- Contributors and downstream users remain responsible for their own risk assessment when deploying or extending AIC components.
- This document will evolve as Parallel TestNet and core components mature.

---

## 6. Reporting Supply-Chain Issues

Suspected malicious or high-risk supply-chain problems (compromised packages, suspicious commits, build-system anomalies) should be reported through the same private channel used for vulnerability disclosure (see Vulnerability-Disclosure.md).

---

*Adaptive Intelligence Circle Foundation*  

*Transparency over opacity. Minimal trust surface. Human oversight on critical paths.*