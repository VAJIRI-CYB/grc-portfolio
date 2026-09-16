# Notes — IT General Controls Matrix & Sample Finding

**Judgment calls:**
- Covered all four classic ITGC domains (access, change, program development,
  operations) even though access and change dominate at a SaaS company. Auditors
  expect the full frame, and gaps in program development are where fast-moving
  engineering orgs actually lose control.
- Every test procedure specifies a METHOD and a SAMPLE SIZE. "Review the process" is
  not a test. Included the four testing methods (inquiry, observation, inspection,
  reperformance) in a legend tab so the strength hierarchy is explicit ; inquiry alone
  is never sufficient evidence.
- Used reperformance deliberately on the highest-risk controls (AC-04 privileged
  access, CM-03 dev/prod segregation): attempting the prohibited action is the only
  test that proves the control actually blocks rather than merely being configured.
- Balanced the matrix across preventive, detective, and corrective types rather than
  loading up on preventive. A portfolio with no corrective controls has no answer for
  what happens after something gets through.
- The sample finding names a PRIVILEGED account in the consequence section. Severity
  is argued with facts, not adjectives — this is what makes it High rather than
  Medium.
- Included a management response and a corrective action tracker. Findings without
  responses are opinions; findings without owned actions and dates are documents
  rather than control improvements.
- Split remediation into immediate (disable the three identified accounts, 24 hours)
  versus systemic (automation, 90 days). Good corrective action plans distinguish
  stopping the bleeding from curing the cause.

**What I'd do differently:** add separate columns for control frequency versus TEST
frequency, conflating them is a common matrix error I caught late. Also map each
control to its governing policy by document ID so the matrix and the policy suite
reference each other explicitly.
