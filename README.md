# MAIM Commerce Catalog

Canonical offer, SKU, Stripe mapping, fulfillment, and release-readiness register for the MAIM ecosystem.

## Purpose

This repository answers four operational questions:

1. What can MAIM sell?
2. What must be built before each offer is sellable?
3. How does each offer map to Stripe, fulfillment, access, and legal terms?
4. What evidence proves the offer works in production?

It tracks commercial records. It does not replace curriculum authority, brand authority, the shared media catalogue, Stripe, Airtable, or production evidence.

## Authority map

- [Major-AI-OS](https://github.com/MajorDream444/Major-AI-OS): MAIM philosophy, doctrine, customer journey, ecosystem meaning.
- [MAIMACADEMY](https://github.com/MajorDream444/MAIMACADEMY): Academy curriculum, application behavior, learner experience, fulfillment implementation.
- [MAIM-Academy---brand](https://github.com/MajorDream444/MAIM-Academy---brand): visual and verbal application.
- **This repository:** offers, SKUs, prices, Stripe mappings, entitlements, dependencies, readiness, and release evidence.

## Start here

- [Offer register](catalog/offers.csv)
- [Offer schema](schemas/offer.schema.json)
- [Status model](docs/STATUS_MODEL.md)
- [Stripe mapping rules](docs/STRIPE_MAPPING.md)

## Non-negotiable boundary

A placeholder, approved idea, completed asset, merged branch, Stripe object, successful test, and verified live offer are different states. No offer is marked `VERIFIED_LIVE` until checkout, payment, webhook, persistence, confirmation, fulfillment, access, support, retry, and refund behavior are evidenced in the intended production environment.

## Stack

Owned commerce uses Vercel, Stripe, Airtable, and Resend. Shopify, Gumroad, and Kit are retired.

Never commit secrets, customer data, payment details, private learner records, or personal email identities.
