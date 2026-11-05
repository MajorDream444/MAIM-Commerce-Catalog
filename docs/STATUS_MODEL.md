# Offer Status Model

Use one primary `release_status` per catalog row.

| Status | Meaning |
|---|---|
| CONCEPT | Captured idea; no founder approval implied |
| FOUNDER_SELECTED | Founder wants it developed |
| APPROVED | Scope and commercial policy approved |
| ASSET_BUILD | Content, design, or physical asset in production |
| IMPLEMENTED | Required code or operational workflow exists |
| TESTED | Controlled test passed; environment must be named in evidence |
| DEPLOYED | Deployed, but full customer path is not yet verified |
| VERIFIED_LIVE | Production customer path verified end to end |
| ON_HOLD | Work intentionally paused; reason required |
| RETIRED | No longer offered; replacement or archive note required |

## Required rule

Never infer a later state from an earlier one:

- merged is not deployed;
- deployed is not tested;
- tested in Preview is not verified in Production;
- a Stripe product is not a functioning checkout;
- an email provider acceptance ID is not inbox delivery;
- an Airtable schema is not persisted order evidence.

Every state change should include an evidence URL and updated date.
