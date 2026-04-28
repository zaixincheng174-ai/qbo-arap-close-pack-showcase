# QBO / AR-AP Close Pack Showcase

A public showcase for an Excel-native pre-close review workflow that turns AR/AP, General Ledger, and Trial Balance exports into traceable, reviewer-ready Excel close workpapers.

> This repository is a sanitized portfolio showcase. It does not contain real client data, private firm documents, internal audit notes, commercial strategy files, credentials, or the full private product source code.

## One-line pitch

An accounting workflow automation project that ingests AR/AP, GL, and TB exports, runs traceable pre-close review checks, and produces a downloadable Excel close pack for reviewer handoff.

## Problem

Small bookkeeping and accounting teams often perform monthly close review through exported accounting reports and manually maintained Excel workbooks. This creates recurring friction:

- AR/AP balances need to tie back to the GL and Trial Balance.
- Exceptions must be reviewed before close.
- Client questions need to be collected into a clear Ask Client list.
- Reviewers need source-level traceability, not just a dashboard.
- Final output must fit the existing Excel-native workflow.

## Solution

The project is designed as an Excel-native close-pack output layer:

AR/AP exports + General Ledger + Trial Balance → validation and field mapping → traceable review checks → exceptions, reconciliation, variance, Ask Client → downloadable Excel close pack.

## Core capabilities

- Import AR/AP, General Ledger, and Trial Balance exports.
- Validate and map source fields.
- Run deterministic review checks for close-readiness.
- Trace findings back to source rows and source files.
- Generate reviewer-facing exception, reconciliation, variance, and client-question outputs.
- Produce a downloadable Excel workbook designed for review, signoff, and handoff.

## Why AR/AP + GL/TB matters

AR/AP files show subledger-level detail. GL and TB files show the accounting system view. A useful close-pack workflow should connect both.

- AR/AP records explain customer/vendor-level balances.
- GL records show transaction-level accounting movement.
- TB records support account-level balance checks.
- A reviewer needs the ability to trace a finding back to the source file and row.

## Intended users

- Small bookkeeping firms
- Small accounting firms
- QBO/Xero-heavy teams
- Monthly close reviewers
- Staff preparing client follow-up lists
- Firms that still rely heavily on Excel workpapers

## Public showcase contents

- `docs/architecture.md` — system architecture
- `docs/data-lineage.md` — traceability model
- `docs/review-checks.md` — supported check categories
- `docs/demo-script.md` — 5-minute demo walkthrough
- `docs/privacy-and-risk.md` — public-release safety notes
- `samples/README.md` — synthetic sample data plan
- `screenshots/README.md` — screenshot checklist
- `excel-output/README.md` — Excel output description
- `diagrams/workflow.md` — workflow diagram

## What is not included

This public repository does not include real client data, private accounting firm data, credentials, internal audit files, commercial strategy documents, full proprietary implementation details, or non-synthetic workbooks.

## Status

Portfolio showcase. The private implementation has working flows for AR/AP + GL/TB review and downloadable Excel output. This public repo is intentionally scoped to explain the workflow, architecture, and review logic without exposing sensitive or commercial internals.

## Resume positioning

This project supports fintech, bank technology, accounting automation, B2B SaaS, and full-stack software roles.

<!-- SHOWCASE_PROOF_START -->
## Demo Evidence Status

This repository is a sanitized public showcase for a private working implementation. The next public proof layer is screenshots and a short demo built from synthetic data.

Current proof files:

- [Architecture](docs/architecture.md)
- [Data lineage and traceability](docs/data-lineage.md)
- [Review checks](docs/review-checks.md)
- [5-minute demo script](docs/demo-script.md)
- [Showcase proof plan](docs/showcase-proof-plan.md)
- [Screenshot checklist](screenshots/README.md)
- [Excel output evidence plan](excel-output/README.md)

Public boundary: no real client data, private firm data, credentials, internal audit files, commercial strategy files, or full private implementation source code are included.
<!-- SHOWCASE_PROOF_END -->
