_Summerville Admin Console  ›  Manage Business  ›  Business Users_

# Manage Business — Business Users & Role Diagnostics

> Diagnose what a specific commercial user can and cannot do — the role's applied permissions tree and its dollar / frequency limits.

## Summary

Business Users is the diagnostic surface for any commercial ticket that starts with X cannot do Y. It lists every employee of the business who can log in to digital banking with their assigned role, and opening a single user exposes the effective entitlements the user has inherited — the Role Permissions modal with the full feature tree and the Role Limits modal with the dollar and frequency caps.

The permission tree is structured exactly how the customer-facing site renders navigation, which makes it easy to trace what the end user will and will not see on their own dashboard. Nine times out of ten a missing-feature escalation is either an un-ticked checkbox on Role Permissions or an approval sitting in the work queue — both of which are visible from this single user profile.

## Key Use Cases

A client calls saying their controller, mapped to Business Admin, cannot release wires. The operator opens the user detail, expands Role Permissions > Manage Transfers and Payments, and confirms whether the wire-release leaf is ticked — then cross-checks Role Limits to see whether the wire ceiling is zeroed.

A payment rejected on limit. The operator compares the user's Role Limits modal against the Business Limits from the Permissions & Limits sub-guide to identify whether the binding constraint was the role ceiling or the entity ceiling, which is the difference between a role tweak and a credit-memo conversation.

## End-to-End Workflow

### Prerequisites

- Business booked on the core banking system with a Business ID issued — the admin console matches businesses by that ID on an exact-search basis.
- At least one Permission Template and one Role Template active in the central catalogue, so a newly onboarded business inherits a production-ready default on day one.
- Signed treasury-services agreement, commercial pricing schedule, and approved credit memo lined up before any entitlement, limit, or role change is made.
- Documented dual-control policy agreed with Risk and Audit so the Approval Settings thresholds can be calibrated to policy rather than set by feel.

### Step-by-Step Flow

#### Step 1 — Open a Business User detail

Business Users lists every employee of the company who can log in to digital banking, along with their assigned role. Opening an individual user — for example, a controller mapped to Business Admin — shows the effective entitlements the user has inherited from that role, which is the first place to look when a client reports a missing capability.

![Step 1 — Open a Business User detail](img/mb-19-business-user-detail.png)

#### Step 2 — Inspect the role's applied permissions

From the user detail the operator can drill into the Role Permissions modal, which displays every feature flag the user's role currently carries — Access/View Bill Pay, Scheduled Transfers, Recipients, Wires, ACH, and the full Manage Transfers and Payments tree. Nine times out of ten a missing feature is either an un-ticked checkbox at this level or an approval sitting in the queue.

![Step 2 — Inspect the role's applied permissions](img/mb-20-role-permissions-modal.png)

#### Step 3 — Expand the permission tree

Expanding the modal reveals the full hierarchy beneath Manage Transfers and Payments — ACH origination sub-features, wire release, scheduled transfer management, external transfer visibility. The tree is structured exactly how the customer-facing site renders navigation, which makes it easy to trace what the end user will and will not see on their own dashboard.

![Step 3 — Expand the permission tree](img/mb-21-role-permissions-expanded.png)

#### Step 4 — Inspect the role's applied limits

Still from the user detail, the Role Limits modal shows the dollar ceiling on each entitled flow — Request ACH collections, Run payroll template, Make domestic wire transfers — in the exact units the transaction runtime will enforce. Compare against the Business Limits from step 9 to confirm the role is nested correctly inside the entity ceiling.

![Step 4 — Inspect the role's applied limits](img/mb-22-role-limits-modal.png)
