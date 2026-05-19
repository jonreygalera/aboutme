# 2026: StatsFlow — Freelancer Disbursement Platform

## StatsFlow

**Role:** Lead Developer  
**Tech Stack:** Laravel, Filament, PHP, MySQL, Redis, Docker, Finance

### The Challenge

Managing freelancer disbursements was a disjointed process. The business was running two legacy systems: **Prody** (which tracked production statistics) and **Flai** (which handled payouts). While **Flai** was functional but not modern, almost all operational and calculation errors stemmed from **Prody**. Because these systems were disconnected, statistics data had to be manually extracted from **Prody**, cross-referenced, and calculated inside massive, fragile spreadsheets before being passed to **Flai** for disbursement.

This approach introduced significant risks:
* **Manual Errors:** One broken spreadsheet formula or corrupted import from Prody could lead to incorrect payout calculations.
* **Audit Gaps:** Spreadsheet cells lacked approval histories, change tracking, or immutable audit trails.

The goal was to eliminate this fragmentation and consolidate **Prody** and **Flai** into a secure, modern source of truth—automating calculations and payouts end-to-end.

### The Build

Designed and engineered **StatsFlow**, a modern financial orchestration engine built with Laravel and Filament that seamlessly combined the stats tracking and disbursement pipelines.

Key implementation details:
* **Legacy Data Migration:** Migrated large volumes of historical stats and payout records from the legacy Prody and Flai systems into the unified StatsFlow database schema, preserving years of history.
* **Automated Production Rules:** Created a flexible calculation engine that translates complex production metrics into concrete earnings, eliminating manual data entry.
* **Multi-Stage Approval Hierarchies:** Built a structured, role-based workflow allowing managers, finance teams, and directors to audit and sign off on payouts with full audit logging.
* **Flai Integration:** Integrated directly with the legacy Flai payout system, bridging the stats and disbursement pipelines.
* **Queue-Driven Scaling:** Leveraged Laravel Queues and Redis to handle concurrent calculations and disbursement requests asynchronously, keeping the Filament dashboard fast and responsive.

### The Outcome

The launch of StatsFlow successfully eliminated spreadsheet dependency for freelancer payouts:
1. **Zero Math Errors:** All calculations are handled programmatically by tested rule engines.
2. **Reduced Turnaround:** Payout times dropped from several days of manual work to instant automated processing.
3. **Institutional Security:** Every payout is recorded, approved, and tracked with a clear audit trail.
