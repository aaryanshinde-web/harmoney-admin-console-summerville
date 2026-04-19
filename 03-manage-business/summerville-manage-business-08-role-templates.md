_Summerville Admin Console  ›  Manage Business  ›  Role Templates_

# Manage Business — Role Templates

> Maintain the central catalogue of pre-built roles (Business Admin, Basic Role, Payroll, View-only) that every business can inherit to seed its own user roles.

## Summary

Role Templates is the role-level counterpart to Permission Templates: a library of pre-built roles — Business Admin, Basic Role, Payroll, View-only — that any commercial business can inherit to seed its own user roles quickly. The lock icon next to Business Admin and View-only indicates a system-default role that cannot be removed, which guarantees that every commercial workspace always has an administrator and an auditor path.

Creating a template role uses a two-step form: Role Information captures the name and one-line description, and the second step assembles the feature set via the now-familiar dual-pane editor. Because a template role feeds every downstream business that picks it, every edit is a policy change that should be paired with a ticket, a reviewer, and a retrospective check against the signed service agreements.

## Key Use Cases

Summerville standardises a Payroll role for every commercial client that runs an ACH payroll template. The operator creates a Template Role called Payroll with a clear description, assembles the permissions via the dual-pane editor, and every future onboarding seeded from this template carries the identical payroll-originator shape.

A policy review decides that the View-only template should no longer expose the scheduled-transfer history. The operator edits the View-only Template Role's permissions, pairs the change with a retrospective check against existing clients, and the new capability set is applied on every business that picks View-only going forward.

## End-to-End Workflow

### Prerequisites

- Business booked on the core banking system with a Business ID issued — the admin console matches businesses by that ID on an exact-search basis.
- At least one Permission Template and one Role Template active in the central catalogue, so a newly onboarded business inherits a production-ready default on day one.
- Signed treasury-services agreement, commercial pricing schedule, and approved credit memo lined up before any entitlement, limit, or role change is made.
- Documented dual-control policy agreed with Risk and Audit so the Approval Settings thresholds can be calibrated to policy rather than set by feel.

### Step-by-Step Flow

#### Step 1 — Open the Template Roles catalogue

Template Roles is the role-level counterpart to Permission Templates: a library of pre-built roles — Business Admin, Basic Role, Payroll, View-only — that any business can inherit to seed its own user roles quickly. The lock icon next to Business Admin and View-only indicates a system-default role that cannot be removed, guaranteeing every commercial workspace always has an administrator and an auditor path.

![Step 1 — Open the Template Roles catalogue](img/mb-32-template-roles-list.png)

#### Step 2 — Create a new Template Role

Create New Template Role opens a two-step form: in step 1, Role Information captures the role name and a one-line description of what the role is for, and step 2 lets the operator assemble the feature set. Keep the role name in plain English, because every business administrator who later inherits this template will see the name in their own User Roles panel.

![Step 2 — Create a new Template Role](img/mb-33-create-template-role.png)

#### Step 3 — Review a Template Role's permissions

Once a template role exists, the Template Role Permissions page lists every feature currently granted — Access/View Bill Pay, View Scheduled Transfer History, View List of Recipients, View Recipient, View Scheduled Transfer Details, View External Transfers. Use this read-only surface as the definitive statement of what a business inheriting this role will get on day one.

![Step 3 — Review a Template Role's permissions](img/mb-34-template-role-permissions.png)

#### Step 4 — Edit a Template Role's feature set

Edit template role opens the now-familiar dual-pane Available / Included editor, scoped to the template role being tuned. Because this feeds every downstream business that picks the role, treat the change as a policy change: pair it with a ticket, a reviewer, and a retrospective check against the business's signed service agreement.

![Step 4 — Edit a Template Role's feature set](img/mb-35-template-role-permissions-edit.png)
