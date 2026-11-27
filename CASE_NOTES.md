# Engineering case notes

[Profile](README.md) · [Portfolio](PROJECTS.md) · [Capabilities](CONTRIBUTIONS.md)

These notes describe documented contributions and design boundaries, not independently audited production architectures.

## 01 — Autom8r: connecting acquisition to delivery

**Problem:** small businesses need coherent customer journeys rather than disconnected websites and AI tools.

**Contribution:** founder-led service design, website and assistant experiences, lead research, outreach, quotation and follow-up workflow design.

**System model:** website or enquiry → qualification → human-reviewed response or quote → follow-up → delivery records.

**Engineering considerations:** business-specific knowledge, escalation, validation, duplicate submissions and clear handoffs. Integration and delivery maturity varies by client.

**Evidence:** [public agency site](https://autom8r.uk). Client implementations remain private.

## 02 — KeepSide: trusted information and family support

**Problem:** people affected by dementia and their families need accessible, familiar information and support with daily routines.

**Contribution:** product journeys, interactive demonstration, family memories, voice assistant direction, permission-aware access, research rationale and safeguarding design.

**Design model:** authorised family information → accessible retrieval → familiar reassurance or routine guidance → human support where appropriate.

**Engineering considerations:** source grounding, consent, access separation, accessibility, escalation and data minimisation. Clinical efficacy, security assurance and production readiness are not established.

**Evidence:** [public product site](https://keepside.uk).

## 03 — Agent H: AI calling control surface

**Problem:** make agent configuration and call initiation understandable to an operator.

**Contribution:** React/TypeScript frontend prototype, contact selection, agent settings, call preparation and webhook request path.

**Boundary:** a request acknowledgement is not evidence of a completed call. Telephony/backend operation is separate; some frontend actions are simulations. Private source is not published here.

## 04 — JARVIS OS: human-supervised AI operations

**Problem:** specialist AI tasks need organisation, persistent context and review boundaries.

**Contribution:** configured role workspaces, task ownership, records, context separation and approvals.

**Design model:** request → specialist workspace → proposed output → human review → recorded outcome.

**Boundary:** coordinated assistant roles are not equivalent to autonomous employees; external actions depend on available integrations and permissions.

## 05 — Business operations console

**Problem:** disconnected records make quoting, jobs and stock harder to coordinate.

**Contribution:** browser-local demonstration spanning customers, enquiries, jobs, inventory, quotes, invoices and tasks.

**Boundary:** local persistence demonstrates interaction and workflow design, not secure multi-user storage. Production would require authentication, server-side authorisation, database constraints, audit trails and backups.

## 06 — Growth and creative intelligence

**Problem:** research, content decisions and distribution are often fragmented.

**Contribution:** creator discovery and scoring concepts, campaign research workflows, content queues and approval architecture across Vaultara, GrowthOS and historical agency experiments.

**Boundary:** planned platform integrations and analytics are not claimed as released features. Campaign results and client data remain private.

## What I would demonstrate in a technical review

- Explain the user problem and the chosen data or interaction model.
- Identify implemented, simulated and planned components.
- Walk through failure cases, permissions and integration boundaries.
- Discuss testing and production requirements without claiming they have already been met.

[Back to profile](README.md)
