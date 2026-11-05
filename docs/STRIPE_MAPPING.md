# Stripe Mapping Rules

## Identity

Each sellable offer receives one stable internal SKU. Stripe product and price IDs are mappings, not the canonical identity.

Recommended SKU pattern:

`MAIM-{FAMILY}-{OFFER}-{VERSION}`

Examples:

- `MAIM-BOOK-ABC1-001`
- `MAIM-COHORT-FOUNDATIONS-001`
- `MAIM-ACADEMY-CAMPUS-MONTHLY-001`
- `MAIM-SPARK-BPT-001`

## Price rules

- Store currency and amount in the catalog only after founder approval.
- Do not overwrite historical prices accepted by customers.
- Create a new Stripe Price for a changed amount, interval, currency, or tax behavior.
- Record test and live IDs separately.
- Recurring offers must state interval, trial behavior, cancellation rules, and bounded entitlements.
- Physical offers must state inventory, shipping region, taxes, returns, and fulfillment owner.

## Release evidence

Before `VERIFIED_LIVE`, evidence must cover:

1. production checkout;
2. successful payment;
3. signature-verified webhook;
4. durable order persistence;
5. Resend acceptance and inbox receipt;
6. correct entitlement or fulfillment;
7. customer return and support path;
8. safe duplicate retry;
9. refund and entitlement behavior.

No credentials or customer records belong in this repository.
