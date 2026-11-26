# Framing Creativity Lab — Audit Documentation

**Document ID:** FCL-AUD-INDEX-001  
**Version:** 1.0  
**Status:** Initial audit collection index

This collection stores audit instructions, dated findings, and the resulting remediation/validation history. 
It is a record series, not a policy and not a substitute for the Lab's governance documents.

## Audit records

| Audit ID | Date | Scope | Baseline | Overall result | Record |
|---|---|---|---|---|---|
| `FCL-DOC-AUDIT-2026-001` | 25 Nov 2026 | Twelve foundational documentation files | `e026bdc5cc4a78dd80570f8c93d50008711de262` | 3.7/5; conditionally ready; 11 findings | [Open audit record](FCL-DOC-AUDIT-2026-001/00-AUDIT-RECORD.md) |

## Validation reports

| Audit ID | Date | Inspected commit | Result | Report |
|---|---|---|---|---|
| `FCL-DOC-AUDIT-2026-001` | 26 Nov 2026 | `b0a71f618cde4b75459b1094f80a30eec5a71543` | Not ready — remediation remains open | [Post-remediation validation](FCL-DOC-AUDIT-2026-001/06-POST-REMEDIATION-VALIDATION-2026-11-26.md) |

## Collection structure

Each audit folder should contain, as applicable:

1. Audit record and scope metadata.
2. Prompt or protocol version used.
3. Immutable report for the inspected commit.
4. Remediation register with evidence and status.
5. A new post-remediation validation report and its prompt, if used.

## Naming convention

Use `FCL-[SCOPE]-AUDIT-YYYY-NNN` for audit instances and stable document IDs for reusable prompts, registers, and protocols. 
Keep historical records; create a new audit instance for a new inspection rather than overwriting an earlier report.

## Publication and confidentiality

Only publish material cleared under the Publication Policy. Never place private project material, source code, credentials, prompts,
assets, client data, private architecture, or restricted metadata in this collection. Public visibility does not grant reuse rights.
