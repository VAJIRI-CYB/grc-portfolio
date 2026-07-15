
# Notes — SOC Ticket vs. GRC Write-Up

**Judgment calls:**

- Simulated a credential-phishing incident deliberately: it's the most common real-world
  incident type, and it fails across three control families at once (authentication,
  awareness, monitoring) — perfect for showing control-failure analysis.
  
- In the GRC version, I traced the root cause past the user ("clicked a link") to the
  governance gap: an MFA rollout exception that nobody had risk-accepted. Blaming users
  is a dead end; finding the unowned exception is actionable.
  
- Ended the GRC version with metrics (MFA coverage %, training completion %) because a
  corrective action without a monitoring metric is just a promise.

**What I'd do differently:** 

Add a cost dimension ( even a rough estimate of incident handling hours would strengthen the business-impact framing.)
