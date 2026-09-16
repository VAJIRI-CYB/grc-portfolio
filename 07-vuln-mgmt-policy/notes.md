
# Notes — Vulnerability Management Policy & Risk Acceptance

**Judgment calls:**
- SLAs are risk-informed rather than CVSS-only. Prioritization combines CVSS base
  score, exploitability signals (CISA KEV listing, EPSS score), and asset criticality
  from the inventory. A 9.8 on an isolated lab box is not a 7.5 on the payment API,
  and any policy that treats them identically will burn remediation capacity in the
  wrong place.
- KEV-listed vulnerabilities inherit Critical SLA regardless of CVSS score. Confirmed
  in-the-wild exploitation is a stronger signal than any theoretical severity rating.
- Separated internet-facing from internal SLAs. Same vulnerability, different exposure,
  different urgency ; a single flat SLA is either too slow for the perimeter or
  unrealistic for internal estate.
- The exception process is the heart of the policy: named approver (Head of Security
  up to 90 days, CTO for renewal), mandatory compensating controls, and a HARD expiry.
  Immortal "temporary" exceptions are how vulnerability programs rot.
- Wrote the policy tool-agnostic. "Nessus" appears nowhere in the policy text so it
  survives a scanner change; tooling belongs in standards and procedures.
- Built the risk acceptance form around a legacy server with a vendor-dependent patch
  timeline — deliberately the most mundane scenario possible, because every real
  security team has that server and program maturity is visible in how it's governed.
- The acceptance form shows the residual score math explicitly (inherent L3 x I4 = 12
  reduced to L2 x I3 = 6, within the ≤6 appetite) rather than asserting "it's fine."
  Named five specific compensating controls; vague "we're monitoring it" is not a
  compensating control.
- Added early-termination triggers to the exception (KEV listing, EPSS rise above 0.5,
  migration completing early). This converts an accepted risk into a monitored risk.

**What I'd do differently:** add a metrics appendix with historical trend data rather
than just targets ; SLA compliance at a point in time says less than SLA compliance
trending over six months. Also define a false-positive determination workflow; the
policy references it as a valid SLA closure path without specifying who adjudicates.
