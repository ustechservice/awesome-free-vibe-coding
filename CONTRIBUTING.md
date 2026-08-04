# Contributing

This repo survives on verification discipline. PRs that follow the rules get merged fast; PRs that don't get closed with a link here.

## The Rules

1. **Receipts required.** Every limit/price claim must link to the official pricing page or docs. Screenshot of the pricing page attached to the PR is strongly encouraged.
2. **Announcement posts are not sources.** Launch blogs, press releases, and news articles are where stale data comes from (see: CodeWhisperer, Cohere). Pricing/docs pages only.
3. **Permanent free ≠ trial.** Trials, expiring credits, and promos must be labeled as such. Never present a one-time credit as a recurring limit.
4. **Honest accounting.** Report documented recurring limits. No theoretical rate-limit-ceiling math, no "550+ tools" inflation. The README's counts must match `tools.json`.
5. **Set the date.** Every added/updated row gets `last_verified` = the date you checked the primary source.
6. **Scope: vibe coding.** AI-assisted development tools, their fuel (APIs/models), their deploy targets, and the minimal business stack a shipped app needs. General AI apps, writing tools, and infra long-tail belong in the linked directories, not here.
7. **Displacement rule (curated sections).** Business Stack and Subscription Killers are capped. To add a tool, argue which incumbent it displaces and why.
8. **Deaths are contributions.** A well-sourced Graveyard PR (tool/tier discontinued, with date and source) is as valuable as a new entry.
9. **Don't abuse free tiers.** No entries that depend on ToS violations (key pooling, proxy rotation, multi-accounting). We list what providers actually offer.

## Adding a tool

1. Add the entry to `tools.json` following the schema (see file header comment).
2. Add the row to the appropriate README section with badges.
3. Include primary-source link + verification date.

## Updating / flagging stale data

Open an issue with the `stale` label, or better: PR the correction with the new receipt. If a tool died, move it to `GRAVEYARD.md` — don't just delete it.
