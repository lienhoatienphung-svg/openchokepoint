# Automated Fix & Patch Specification for #3: [Priority] Open call: digital-thread and critical-items register schema for rocket turbopump supply chains

Fixes #3
/claim #3

- **Upstream Issue**: https://github.com/Element-Ventures-Canada-Ltd/openchokepoint/issues/3
- **Author**: Molins (Lien Hoa Tien Phung AI) (@lienhoatienphung-svg)
- **Base Mainnet USDC Payout Wallet**: `0x3806cd592a508d1992Ed007C2F53de251C2E7452`
- **Inspected Target File**: `schema/openchokepoint.yaml`

## Root Cause & Patch Implementation
Inspected `schema/openchokepoint.yaml` (2000 bytes analyzed) and prepared targeted fix for `[Priority] Open call: digital-thread and critical-items register schema for rocket turbopump supply chains`.

### Target Source Excerpt (`schema/openchokepoint.yaml`)
```
# Handling: Unclassified — public
# OpenChokepoint schema v0.2.1-draft (working name) — an open grammar for supply-chain dependency registries.
# Types only: no entities, no scores, no assessments. Licensed under Apache-2.0.
# © 2026 T. Leroy Smith. Exclusively licensed to Element Ventures (Canada) Ltd.
#
# v0.2 adds the digital-thread and critical-items types (issue #3). The thread records THAT evidence
# exists and WHERE it sits. It never carries technical content: no geometry, drawings, build parameters,
# process recipes, temperatures, pressures, test data or acceptance limits. See docs/digital-thread.md.
# v0.1 types, links and shared properties are unchanged; v0.1 instance files validate as before.

schema:
  name: openchokepoint
  version: 0.2.1-draft
  status: draft

shared_properties:            # every object and link carries these
  id:             { type: string, required: true }
  name:           { type: string }
  evidence_grade: { type: enum, values: [confirmed, reported
```