# Notes — ISMS Scope Statement & Statement of Applicability

**Judgment calls:**

- Scoped the ISMS around the customer platform and its supporting corporate IT
  services; excluded the marketing website (public content only, separately hosted)
  and physical security of employee home offices (addressed via endpoint controls)
  with written justification for each. Scope creep is how ISMS implementations drown.
  
- Wrote the scope statement to cite Clauses 4.1, 4.2, and 4.3 explicitly, because
  auditors verify scope against the clauses it satisfies. Naming the clauses signals
  the document was built for the standard, not around it.
  
- Declared shared-responsibility explicitly for AWS, M365, Okta, Stripe, and PayCo.
  Modern ISMS scopes touch cloud providers, and undeclared interfaces are where
  scope disputes happen during audit.
  
- Used honest statuses on the SoA: 25 controls broken down as Implemented / Partial
  / Planned / Not applicable. Pretending everything is Implemented is how Stage 2
  audits go badly — the SoA is a management tool first and an audit artifact second.
  
- The EVIDENCE column was the most valuable discipline. "We do access reviews" is a
  sentence; "quarterly signed attestations per system owner" is a control. Every
  applicable row names what an auditor should ask to see.
  
- Excluded exactly one control (A.7.4 physical monitoring) and spent real effort on
  the justification tied to accepted risk R-15. An SoA with zero exclusions usually
  signals nobody examined anything; an exclusion without defense fails the audit.
  
- Cross-referenced every applicable row back to the risk register, policy suite, or
  a specific incident review. Interlocking artifacts is how a real ISMS behaves;
  isolated documents is how portfolios read as templates.

**What I'd do differently:** 

Expand from 25 controls toward full 93-control coverage (on the roadmap) and add a column linking each control to its governing policy 
The SoA and the policy suite should reference each other by document ID, not by memory.
