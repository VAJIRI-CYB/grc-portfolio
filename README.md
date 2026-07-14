# GRC Portfolio — End-to-End ISMS Build & Internal Audit

**Victor Ajiri** | Canada | [linkedin.com/in/victor-a-0b668862](https://linkedin.com/in/victor-a-0b668862)
*Security Operations Analyst (6+ yrs) transitioning into Governance, Risk & Compliance | CySA+ • Security+ • ISC² CC | MSc Information Systems Security Management*

---

## What this is

A complete, self-directed GRC practicum: I designed, documented, and internally audited a full **Information Security Management System (ISMS)** for a fictional company — **MapleTech Inc.**, a 200-person Canadian B2B SaaS handling customer PII in AWS — following **ISO/IEC 27001:2022**, **ISO 27005**, and **PIPEDA** requirements.

> ⚠️ **MapleTech Inc. is entirely fictional.** All scenarios, findings, and data are simulated for demonstration. No artifact here derives from any current or former employer.

Every document interlocks the way a real ISMS does: risks in the register map to controls in the Statement of Applicability, controls are governed by the policies, and the capstone internal audit tests those same policies — producing findings and corrective actions that feed back into the register.

## Why I built it

Six years in SOC and security operations taught me to *operate* the controls — SIEM monitoring, vulnerability management, access reviews, incident response. This practicum builds the governance layer on top: assessing risk, writing the policies, designing the control framework, and auditing it. Operating controls and governing them are different skills; I wanted proof of both.

---

## The artifacts (in ISMS lifecycle order)

| # | Phase | Artifact | Folder | What it demonstrates |
|---|-------|----------|--------|---------------------|
| 1 | Foundations | Incident review: SOC ticket vs. GRC write-up | `01-grc-foundations/` | Translating technical incidents into control-failure and root-cause language |
| 2 | Risk | 15-risk enterprise risk register + heat map | `02-risk-register/` | Defined L×I criteria, treatment plans, named risk owners, formal risk acceptance |
| 3 | Risk | STRIDE threat model — login & payment flow | `03-threat-model/` | Trust boundaries, threat-to-control gap analysis feeding the risk register |
| 4 | Context | Asset inventory (CIS Controls 1–2) + framework selection memo | `04-asset-inventory/` | Data classification, criticality rating, SOC 2-first framework strategy rationale |
| 5 | ISMS core | ISMS scope statement + 25-control Statement of Applicability | `05-soa-and-scope/` | Per-control justification, implementation status, evidence expectations, defensible exclusions |
| 6 | Controls | IT General Controls matrix (12 controls) + sample High finding | `06-itgc-matrix/` | Test procedures, evidence requirements, formal finding structure |
| 7 | Controls | Vulnerability Management Policy + completed risk-acceptance form | `07-vuln-mgmt-policy/` | SLA-based remediation, KEV/EPSS-informed prioritization, exception governance |
| 8 | Governance | Policy suite: InfoSec Policy, Access Control Policy & Standard, AUP + Business Impact Analysis | `08-policy-suite-bia/` | Policy vs. standard hierarchy, enforceable language, RTO/RPO with business justification |
| 9 | Third parties | Vendor risk assessment: Tier-1 payroll SaaS + 20-question questionnaire | `09-vendor-risk/` | SOC 2 report evaluation, findings with contractual mitigations, conditional approval |
| 10 | Privacy | PIPEDA data map (9 flows) + breach assessment memo (RROSH analysis) | `10-privacy-pipeda/` | Canadian privacy law application, OPC reporting decision, remediation plan |
| 11 | Assurance | **Capstone: internal audit report** — access control vs. ISO 27001 A.5.15–A.5.18 | `11-internal-audit/` | Full audit lifecycle: scope, methodology, major nonconformity, corrective action tracker |

## Decisions & lessons per phase

Each folder contains a short `NOTES.md` — the judgment calls behind the artifact (e.g., *why control A.7.4 was excluded from the SoA*, *why the access-review finding was rated a major nonconformity*, *why MapleTech should pursue SOC 2 before ISO certification*). The documents show what I built; the notes show how I think.

## Grounding in real experience

The scenarios draw on patterns from six years of real security operations (fully genericized): the risk register reflects threats I've actually triaged, the ITGC access controls mirror provisioning and access-review processes I've administered, and the audit evidence standards come from writing investigation records that had to withstand scrutiny.

## Roadmap

- [ ] ISO 27001 Lead Implementer *(planned)*
- [ ] Expand SoA to full 93-control coverage
- [ ] Management review meeting pack (Clause 9.3)
- [ ] SOC 2 readiness gap assessment for MapleTech

---

**Open to GRC Analyst / IT Risk / Compliance Analyst roles (Canada, remote-friendly).** Happy to walk through any artifact — the internal audit report is the best place to start.
