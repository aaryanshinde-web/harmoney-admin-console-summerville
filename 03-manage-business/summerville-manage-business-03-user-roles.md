_Summerville Admin Console  ›  Manage Business  ›  User Roles_

# Manage Business — User Roles

> Shape the per-role permissions, dollar limits, and frequency stack that govern segregation of duties inside a commercial relationship.

## Summary

User Roles is the lever for enforcing segregation of duties inside a commercial business. Every role defined on the business appears as a card — View-only, Basic Role, Business Admin, and any client-specific roles — and opening a role exposes Role Permissions (which capabilities the role carries) and Role Limits (the dollar and frequency caps on each capability, bounded by the entity-level Business Limits).

Roles should be seeded from the central Role Templates catalogue via the Select Template Role(s) modal rather than built from scratch — the template carries pre-approved permissions and limits straight from Summerville's master policy, which cuts configuration time and keeps every business consistent. Role Information at the top of the panel captures the role name and a one-line description that will be read six months later by an examiner reconciling the transaction log against the documented dual-control policy.

## Key Use Cases

The client's controller should be able to build and submit payroll files but never release them. The administrator creates a Payroll role using the Payroll template, confirms ACH permissions are enabled while wire-release and user-management permissions are withheld, and caps the role's Max Daily and Max Monthly to the anticipated payroll envelope.

A commercial AP clerk needs to originate vendor ACH only. The administrator seeds a role from the Basic Role template, trims it to only the ACH-origination sub-features, stacks Max Per Transaction (fat-finger defence), Max Daily (velocity), and Max Monthly (slow-drift) limits, and writes a Role Information description that makes the segregation explicit.

## End-to-End Workflow

### Prerequisites

- Business booked on the core banking system with a Business ID issued — the admin console matches businesses by that ID on an exact-search basis.
- At least one Permission Template and one Role Template active in the central catalogue, so a newly onboarded business inherits a production-ready default on day one.
- Signed treasury-services agreement, commercial pricing schedule, and approved credit memo lined up before any entitlement, limit, or role change is made.
- Documented dual-control policy agreed with Risk and Audit so the Approval Settings thresholds can be calibrated to policy rather than set by feel.

### Step-by-Step Flow

#### Step 1 — Review the User Roles matrix

User Roles surfaces every role defined on the business as a card — View-only, Basic Role, Business Admin, and any client-specific roles. Roles are the lever for enforcing segregation of duties inside the company: one role originates, another approves, a third is strictly view-only for auditors and advisors.

![Step 1 — Review the User Roles matrix](img/mb-10-user-roles-panel.png)

#### Step 2 — Tailor Role Permissions

Inside a role, Role Permissions presents the same dual-pane Available / Included control, but scoped to that one role rather than the whole business. Enable the commercial sub-features the role actually needs — view transfers, initiate ACH, release wires, manage recipients — and leave the rest on the Available side to honour least privilege.

![Step 2 — Tailor Role Permissions](img/mb-11-role-permissions-edit.png)

#### Step 3 — Set per-role amount limits

Role Limits lets the operator cap each feature inside the role with a dollar ceiling — typically Max Per Transaction for line-level controls, Max Daily for velocity, and Max Monthly for the audit trail. Whatever is set here is bounded by the Business Limits configured earlier, so a controller's role cannot exceed the entity-level envelope.

![Step 3 — Set per-role amount limits](img/mb-12-role-limits-amounts.png)

#### Step 4 — Choose the limit frequency

The amount inputs expose a frequency dropdown — Max Per Transaction, Max Daily, Max Monthly — and the operator can stack all three to build a layered control. Per-Transaction defends against fat-finger errors, Max Daily governs business-as-usual velocity, and Max Monthly catches slow-drift patterns that single-day limits miss.

![Step 4 — Choose the limit frequency](img/mb-13-role-limits-frequency.png)

#### Step 5 — Capture Role Information

On the Role Information panel, enter a descriptive role name and a one-line description that explains the role's business intent — e.g. Payroll — Handles Payroll or AP Clerk — originates vendor ACH, no wire release. Treat the description as audit-grade documentation, because it is what an examiner reads six months later when reconciling the transaction log.

![Step 5 — Capture Role Information](img/mb-14-role-information.png)

#### Step 6 — Seed the role from a template

Rather than build a role from scratch, use the Select Template Role(s) modal to inherit a vetted starting point — Payroll, Business Admin, Basic Role, View-only — and then trim. The template carries pre-approved permissions and limits straight from Summerville's central Role Templates catalogue, which cuts configuration time and keeps every business consistent with master policy.

![Step 6 — Seed the role from a template](img/mb-15-select-template-role.png)
