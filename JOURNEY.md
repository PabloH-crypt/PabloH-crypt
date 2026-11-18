# Engineering notes

[← haych](README.md) · [Work](PROJECTS.md)

I work on products at the point where **interfaces, AI, business processes and user behaviour** meet. These are some design principles I return to across prototypes and client work.

## 01 / A request is not an outcome

A frontend can successfully POST to a service and still have no evidence that the underlying job finished.

For any asynchronous workflow, I want to distinguish the stages:

```text
draft → submitting → accepted → running → succeeded
                                   └──→ failed
```

The exact contract depends on the backend. In a calling interface, a `200 OK` from a webhook should not be labelled “call completed.” Completion requires an authoritative event, status check or equivalent evidence.

**What I look for:** request IDs, explicit pending states, retry/error behaviour and an auditable source of truth.

## 02 / Local persistence is not a backend

Browser storage is useful for a fast, interactive operations demonstration. It is not a shared database and is not a security boundary.

A production transition needs to address authentication, authorisation, ownership checks, validation, auditability, backups and data retention—not just replace `localStorage` with an API call.

**What I look for:** entity boundaries, permission checks on the server, predictable empty/error states and a repeatable test path.

## 03 / An AI assistant needs constraints

An interface with multiple specialist roles can organise work, but the roles themselves do not guarantee autonomous execution or correct answers.

Useful systems need explicit context boundaries, source provenance, clear tool permissions, human approval for consequential actions and verification of output.

**What I look for:** what the assistant may read, what it may change, who approves a change, and how a mistake is detected.

## 04 / Accessibility changes the architecture

For a product built around sensitive or familiar information, accessibility isn't just visual polish.

The design has to account for cognitive load, understandable language, predictable navigation, consent, appropriate role access and the possibility that information is outdated or incorrect.

A fictional-data demonstration can test interaction ideas. It cannot establish real-world or clinical effectiveness.

## 05 / Distribution belongs in product thinking

A feature is only useful if someone understands it, discovers it and returns to it.

My experience in influencer research and creative strategy changes how I scope technical products: audience fit, the first impression, short-form explanation, onboarding, call-to-action and follow-up all shape the system.

That doesn't mean every product needs a content machine. It means **adoption is a design constraint**.

---

These are patterns and lessons from my work, not claims that every prototype already implements them at production quality.

[Browse the anonymised case studies](PROJECTS.md).
