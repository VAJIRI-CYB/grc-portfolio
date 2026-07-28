# Notes — Asset Inventory & Framework Selection

**Judgment calls:**
- Included SaaS and cloud resources as first-class assets, not just hardware — for a
  200-person SaaS company, the crown jewels live in AWS, Okta, and Salesforce, not in
  a server closet.
  
- Every asset got an OWNER and a DATA CLASSIFICATION, because every downstream
  artifact (risk register, SoA, BIA, audit scope) queries those two fields.
  
- Framework memo recommends SOC 2 Type II FIRST, CIS Controls as the internal build
  roadmap, ISO 27001 as the 12–18 month follow-on. Rationale: enterprise procurement
  demands SOC 2 — it unblocks revenue; ISO adds international credibility once the
  evidence discipline exists. Framework sequencing is a business decision.
  
- Deliberately excluded one asset (A-23, marketing website) from ISMS scope with an
  explicit justification — an inventory that includes everything is really an
  inventory that has never been scoped.

**What I'd do differently:** 
Add a data-flow column linking each asset to the privacy data map (folder 10) — the two inventories should reference each other.
