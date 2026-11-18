# Portfolio publishing standards

[← Profile](README.md) · [Project register](PROJECTS.md)

This repository documents public-facing work. It should look like an engineering portfolio, not a collection of generated marketing claims.

## Evidence over decoration

For any project we publish, include:

1. **Problem and audience** — one clear paragraph.
2. **My exact role** — solo, team, university, client or research.
3. **Architecture and stack** — what is actually used, not every technology I've heard of.
4. **Working features** — evidenced by source, a demo or a reproducible test.
5. **Limitations** — simulated actions, missing integrations, security and accessibility gaps.
6. **Run and test instructions** — for public source repositories.
7. **Next milestone** — one concrete, measurable improvement.

Distinguish a prepared concept from a functioning prototype, an interface from its backend, a hosted demo from a production system, and a reported payment from a confirmed customer outcome.

## What not to do

- No animated activity generators, inflated skill bars, vanity metrics or generic motivational banners.
- No fake contribution streaks, testimonials, partnerships, app-store releases or deployment claims.
- No empty repos created just to make the account appear larger.
- No public release of client work or shared projects without permission.
- No screenshots with real customer, patient, student or contact information.
- No keys, credentials, copied private configuration or secrets in source/history.
- No claiming ownership of external-company assets.

## Repository hygiene

Public source projects should have an informative README, appropriate licence (only when chosen), .gitignore, meaningful commits, and a documented test/build path. Before publishing a private repository, audit its files **and history**, credentials, ownership and dependencies. Adding a .gitignore later does not remove secrets already committed.

Use short, purposeful commits and review the diff before merging. Not every project needs a public repo: documentation can be public while implementation stays private.

## Portfolio priorities

1. Preserve the concise [profile README](README.md).
2. Keep [PROJECTS.md](PROJECTS.md) comprehensive but factual.
3. Write technical case studies for a few strong projects with screenshots, diagrams and validated behaviour.
4. Publish reproducible code only after access, privacy and quality review.
5. Revisit the register when a stage changes; don't silently promote concepts to products.

The bar is simple: **could another developer distinguish what exists, understand how it works and tell what remains unfinished?**
