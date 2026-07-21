# Notes — STRIDE Threat Model

**Judgment calls:**
- Modelled the login + payment flow because it crosses the most trust boundaries and
  concentrates the highest-value data ; scope discipline matters more than coverage.
- Ran STRIDE per component rather than per flow; it surfaces repudiation and info
  disclosure threats that attack-path thinking (MITRE ATT&CK habit) tends to skip.
- The most severe findings were governance failures in technical costume: 
  An admin console with no owner for verifying its exposure, a shared full-scope API key with
  no key management standard. Each gap traced to a missing policy or ownership line.
- Fed every accepted gap into the risk register ; a threat model that doesn't update
  the register is a drawing, not a control.

**What I'd do differently:** 
Score the threats (even simple H/M/L) inside the model itself so prioritization survives the handoff to the register.
