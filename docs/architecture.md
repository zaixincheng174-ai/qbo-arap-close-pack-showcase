# Architecture

## High-level workflow

Source exports:
- AR/AP
- General Ledger
- Trial Balance

Workflow:
1. Upload and validation
2. Field mapping
3. Canonical source model
4. Review rule engine
5. Traceable findings
6. Excel close pack

## Main components

### 1. Source ingestion

The workflow starts with accounting exports: AR/AP for subledger detail, General Ledger for transaction-level activity, and Trial Balance for account-level balances.

### 2. Validation and mapping

Each file type requires validation and field mapping. The system needs to understand source columns such as account, date, customer/vendor, amount, debit, credit, memo, balance, and source row identifier.

### 3. Canonical source model

After mapping, records are normalized into a canonical representation so review checks can operate consistently across export formats.

### 4. Review rule engine

The review layer checks for issues such as uncategorized activity, suspense activity, clearing account issues, missing metadata, AR/AP tie-out issues, unusual variances, and items requiring client clarification.

### 5. Traceability

Each generated finding should preserve a link back to source file, source row, source account, source amount, and related AR/AP, GL, or TB record where applicable.

### 6. Excel output

The output is a downloadable Excel close pack designed for reviewer handoff.

Expected workbook sections:
- Cover / Review Summary
- Exception List
- AR/AP Review
- GL/TB Reconciliation
- Variance Bridge
- Ask Client List
- Source Trace / Evidence Notes
