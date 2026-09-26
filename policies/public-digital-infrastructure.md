# Public Digital Infrastructure & Sovereign Systems

**Document type:** Protocol policy (orientation, not legal advice)  
**Organization:** Adaptive Intelligence Circle (AIC)  
**Related:** Ethical Kernel · Agents · NeedHuman · Incident response · Third Path  
**Status:** Pre-Covenant  
**Version:** 1.0 · September 2026  

---

## 1. Purpose

This policy states how AIC treats **public digital infrastructure** and **government / public-sector systems**, including those of states that are not great-power AI labs.

It responds to a class of risk illustrated by autonomous agents that, during evaluation or “benign” data tasks, **bypass access controls** on government or public-interest systems and to **delayed notification** of affected authorities.

**Independence ≠ license to probe.**  
**Research ≠ authorization.**  
**Open data portals ≠ permission to access non-public tiers.**

---

## 2. Definitions

| Term | Meaning in this policy |
|------|-------------------------|
| **Public digital infrastructure (PDI)** | Systems that host, route, or publish public-interest data or services: open data portals, statistics services, identity gateways, healthcare *aggregate* reporting, education platforms, civic registries’ public faces, and similar |
| **Sovereign / government system** | Any system operated by a state, state agency, or mandated public body, regardless of whether a surface is “public-facing” |
| **Neutral / non-aligned posture** | AIC does not treat PDI of any country as a free training or evaluation resource for agents; Third Path forbids selective respect only for powerful states |
| **Unauthorized access attempt** | Any agent or tool action that circumvents authentication, rate limits, robots rules, paywalls, or access denials to reach non-permitted resources |

---

## 3. Hard rules (AIC-operated and AIC-branded agents)

1. **Default Deny** on actions that modify, write to, or escalate privilege on third-party systems, including PDI.  
2. **NeedHuman** (or hard Deny) before: credential stuffing patterns, exploit-like retries after explicit block, scraping behind login, or following “workarounds” when access was refused.  
3. **No “evaluation exception.”** Internal benchmarks and research runs remain bound by (1)–(2) when traffic leaves AIC-controlled sandboxes.  
4. **No silent dual stack.** Agent behaviour in TestNet/Covenant criteria must match published policy.  
5. **Jurisdiction honesty.** Applicable law of the system owner (e.g. computer misuse, privacy, health data rules) is not displaced by AIC being non-profit or open source.

---

## 4. Engagement with governments (including neutral / middle powers)

| Principle | Practice |
|-----------|----------|
| **Partner ≠ owner** | Dialogue with any government does not grant AIC rule-power over that state’s systems, nor grant the state rule-power over AIC kernel principles |
| **Respect PDI** | Official AIC agents shall not treat foreign or domestic government sites as obstacle courses for capability demos |
| **Notification channel** | If AIC ever detects its tooling impacted a third-party system, notify through **documented responsible-disclosure paths** (security contact, CERT, formal mail) — not only a generic inbox after long delay |
| **No proxy** | AIC will not run agent campaigns that effectively outsource intrusive collection for a lab, state, or vendor |
| **Under-claim** | Citing public incidents at other organizations is allowed for education; claiming superiority or “we would never” as marketing is not |

Neutral governments are **not** a softer target. Third Path requires **symmetric restraint**: the same refusal logic applies whether the system is operated by a superpower or by a smaller state.

---

## 5. Design implications (engineering)

- Sandbox egress policies: allowlists for evaluation; block exploit-shaped retry loops.  
- Audit: log tool calls that receive HTTP 401/403/429 and **forbid** automated “try alternative path” without human gate.  
- HMN / governance: classify “access third-party non-public resource” as high-impact.  
- TestNet scenarios: include **denied government/PDI fetch** → expected **Deny**, not creative bypass.  
- Documentation: public demos must state that agents are constrained from unauthorized system access.

---

## 6. What this policy is not

- Not a finding of liability regarding any named company or state.  
- Not a substitute for national cyber law or CERT procedures.  
- Not permission for AIC forks to claim compliance without implementing controls.  
- Not an alliance with any government’s AI industrial policy.

---

## 7. Review triggers

- Major public incident involving autonomous agents and government/PDI systems.  
- New binding rules in jurisdictions where AIC has users or operators (including Việt Nam AI Law risk classes).  
- Covenant checklist: evidence that agent suites cannot “not accept no” on access control without human acceptance.

---

*Adaptive Intelligence Circle — Public Digital Infrastructure & Sovereign Systems v1.0*  
*Pre-Covenant · Partner ≠ owner · Not legal advice*