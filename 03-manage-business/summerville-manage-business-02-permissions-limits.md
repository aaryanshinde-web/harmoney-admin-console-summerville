_Summerville Admin Console  ›  Manage Business  ›  Permissions & Limits_

# Manage Business — Permissions & Limits

> Edit the entity-level feature catalogue (Business Permissions) and the aggregate velocity envelope (Business Limits) that cap the commercial relationship.

## Summary

Business Permissions is the catalogue of every feature the business has been entitled to — ACH origination, domestic wires, bill pay, scheduled transfers, recipient management. Business Limits is the aggregate ceiling that caps the entire legal entity — Max Per Transaction, Max Daily, and Max Monthly on every money-movement feature the business can consume.

The two surfaces are designed to be read together: Business Permissions answers the what (which capabilities can this business use), and Business Limits answers the how much (what velocity envelope applies to those capabilities). Both are edited via the dual-pane Available / Included editor (for features) or a three-input limit row (for dollars). Every change propagates to every user inside the business on the next login and is bounded by the signed treasury-services agreement.

## Key Use Cases

A long-standing client has grown into international suppliers and now needs domestic wires. The relationship manager moves Make domestic wire transfers from Available to Included on Business Permissions, then raises the Max Per Transaction and Max Daily wire ceilings in Business Limits in line with the approved credit memo.

A business is onboarded with ACH-only permissions at the request of the treasury officer, while Wires remain on the Available side of the editor until the dual-control policy for high-value outbound payments is in place — which is what the dual-pane design is there to enforce.

## End-to-End Workflow

### Prerequisites

- Business booked on the core banking system with a Business ID issued — the admin console matches businesses by that ID on an exact-search basis.
- At least one Permission Template and one Role Template active in the central catalogue, so a newly onboarded business inherits a production-ready default on day one.
- Signed treasury-services agreement, commercial pricing schedule, and approved credit memo lined up before any entitlement, limit, or role change is made.
- Documented dual-control policy agreed with Risk and Audit so the Approval Settings thresholds can be calibrated to policy rather than set by feel.

### Step-by-Step Flow

#### Step 1 — Open Business Permissions

Business Permissions is the catalogue of every feature the business has been entitled to — ACH origination, domestic wires, bill pay, scheduled transfers, recipient management. This page shows the live, as-of-now list of features the business and its users may consume, and it is the correct place to start when a client asks why a feature is missing from their dashboard.

![Step 1 — Open Business Permissions](img/mb-06-business-permissions-view.png)

#### Step 2 — Edit Business Permissions

Click Edit and the page splits into two panes — Available Features on the left, Included in template on the right. Move features across the panes to match the pricing schedule the client has signed, then save; the change propagates to every role within the business and is picked up on the user's next login.

![Step 2 — Edit Business Permissions](img/mb-07-business-permissions-edit.png)

#### Step 3 — Open Business Limits

Business Limits is the ceiling for the entire legal entity — the aggregate cap that no user in the business can exceed, regardless of their role. Every money-movement feature the business has entitled shows up here, and this page is the reference point before any role-level limit downstream is tuned.

![Step 3 — Open Business Limits](img/mb-08-business-limits-view.png)

#### Step 4 — Edit the business-level amount caps

Click Edit and each feature exposes three inputs — Max Per Transaction, Max Daily, and Max Monthly — which together define the velocity envelope Summerville is willing to support for this business. Set these against the approved credit memo and the BSA/AML profile on file, because this is the hard cap the transaction layer enforces on every ACH or wire originating from the entity.

![Step 4 — Edit the business-level amount caps](img/mb-09-business-limits-edit.png)
