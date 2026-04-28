# Data Lineage and Traceability

## Goal

The core goal is not just to flag exceptions. The goal is to make every finding reviewable.

A reviewer should be able to answer:
- Which source file created this finding?
- Which row or record is involved?
- Which account, customer, vendor, or balance is affected?
- Is the finding tied to AR/AP, GL, TB, or multiple sources?
- What should the reviewer or client do next?

## Source reference model

Each finding should carry source metadata:
- finding_id
- source_system
- source_file
- source_file_type
- source_row_index
- source_account
- source_name
- source_date
- source_amount
- related_gl_reference
- related_tb_reference
- related_ar_ap_reference
- review_category
- suggested_action

## Example traceability path

Finding: AR balance does not tie to GL control account

Finding row → AR/AP source rows → GL control account movement → Trial Balance ending balance → Reviewer action / Ask Client item.

## Why this matters

Accounting reviewers do not only need an alert. They need evidence. A finding without traceability is hard to trust, hard to review, and hard to sign off.
