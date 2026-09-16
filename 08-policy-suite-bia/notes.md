
# Notes — Policy Suite & Business Impact Analysis

**Judgment calls:**
- Enforced the document hierarchy strictly: policies state WHY and WHAT and name no
  tools; standards carry the enforceable specifics. The Access Control document is
  deliberately split into Part A (policy) and Part B (standard) in one file to make
  the separation visible.
- The Information Security Policy is owned and approved by the CTO, not the security
  team. ISO 27001 Clause 5.2 puts the policy with top management, and that placement
  is what gives every subordinate document its authority.
- Followed current password guidance: length (14+) plus breached-password screening,
  and explicitly NO forced periodic rotation absent suspected compromise.
- Wrote the Acceptable Use Policy to be readable rather than exhaustive. It's the only
  policy most staff will ever open. Included an explicit no-retaliation clause for
  self-reported mistakes — people who fear blame report late, and late reporting is
  what turns incidents into breaches.
- Added a public-AI-tools rule to the AUP. Most policy templates predate this risk
  entirely, and it's now a common real-world data-leakage path.
- Access review cadence is driven by asset criticality rather than a flat schedule.
  Flat cadences either over-burden reviewers or under-protect crown jewels.
- BIA scored impact at 4h / 24h / 72h / 1 week rather than as a single number, because
  impact is rarely linear. The RTO is set where impact crosses from tolerable to
  unacceptable ; a defensible derivation rather than a guess.
- Let the BIA surface a real gap rather than tidying it away: the support ticketing
  vendor has no contractually committed RTO, so the 24-hour objective isn't guaranteed
  by anyone. That gap feeds the risk register and the next vendor reassessment.

**What I'd do differently:** write the Data Classification Standard that both the
InfoSec Policy and the AUP reference ; it's cited as a supporting document but not
yet drafted. Also add a procedure-level document for access provisioning to
demonstrate the full policy → standard → procedure chain rather than just the top
two layers.
