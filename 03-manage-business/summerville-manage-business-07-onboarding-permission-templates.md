_Summerville Admin Console  ›  Manage Business  ›  Onboarding_

# Manage Business — Onboarding & Permission Templates

> Add a new commercial relationship via exact Business ID lookup, and maintain the central Permission Templates catalogue that every new business inherits.

## Summary

Onboarding & Permission Templates governs how a new commercial relationship lands on the digital channel. Add a New Business accepts an exact Business ID and pulls the legal-entity record from the core into digital banking; the Matching Results panel tells the operator when an entity has already been onboarded, which prevents the most common onboarding error — provisioning the same entity twice and splitting its audit trail across two profiles.

Permission Templates is the central library of entitlement bundles — Business Template 1, Test Template, and any approved additions — that every newly onboarded business inherits. The dual-pane editor used inside a single Business Profile applies here too, only bank-wide. Deleting a template is effectively a policy retirement, so the Delete Template confirmation modal exists to force the change-advisory conversation.

## Key Use Cases

A mid-sized LLC running ACH payroll is booked by the commercial loan officer. The onboarding specialist keys the Business ID, the core record is pulled into digital banking, and the specialist assigns Business Template 1 so the client has a working ACH, Wires, and Bill Pay footprint on day one.

The product team adds a new treasury-management feature and wants every future commercial onboarding to inherit it. The administrator opens Permission Templates, edits Business Template 1 to include the new feature, and pairs the change with a release note so operations knows new clients will receive it automatically.

## End-to-End Workflow

### Prerequisites

- Business booked on the core banking system with a Business ID issued — the admin console matches businesses by that ID on an exact-search basis.
- At least one Permission Template and one Role Template active in the central catalogue, so a newly onboarded business inherits a production-ready default on day one.
- Signed treasury-services agreement, commercial pricing schedule, and approved credit memo lined up before any entitlement, limit, or role change is made.
- Documented dual-control policy agreed with Risk and Audit so the Approval Settings thresholds can be calibrated to policy rather than set by feel.

### Step-by-Step Flow

#### Step 1 — Add a New Business

Add a New Business is the onboarding entry point: the page accepts an exact Business ID and, on finding a match in core, pulls the legal-entity record into digital banking. If the business has already been onboarded, the Matching Results panel tells the operator so, which prevents the most common onboarding error — provisioning the same entity twice and splitting its audit trail across two profiles.

![Step 1 — Add a New Business](img/mb-27-add-new-business.png)

#### Step 2 — Open the Permission Templates catalogue

Permission Templates is where Summerville maintains its central library of entitlement bundles — Business Template 1, Test Template, and any additional templates approved by the credit union. Every newly onboarded business inherits one of these bundles, which is how the platform guarantees a client never lands in production with a half-provisioned feature set.

![Step 2 — Open the Permission Templates catalogue](img/mb-28-permission-templates-list.png)

#### Step 3 — Inspect a permission template

Opening a template surfaces the full list of features bundled inside it — View Scheduled Transfer History, View Scheduled Transfers, View List of Recipients, External Scheduled Transfers, Access/View Bill Pay, and the rest. The feature set is the default capability any business inherits when this template is assigned on onboarding, making the template the single source of truth for Summerville's commercial product catalogue.

![Step 3 — Inspect a permission template](img/mb-29-permission-template-details.png)

#### Step 4 — Edit a permission template

Clicking Edit template opens the dual-pane editor — Available Features on the left, Included in template on the right — identical to the per-business editor but applied credit-union-wide. Changes here ripple into every future onboarding that picks this template, so pair every template change with a release note to the operations team.

![Step 4 — Edit a permission template](img/mb-30-permission-template-edit.png)

#### Step 5 — Delete a permission template

Permission templates can be removed from the catalogue via the Delete Template confirmation modal, but only once the operator has confirmed that no active business depends on the bundle. A deletion is effectively a policy retirement, so document the decision in the change-advisory record before clicking Delete, and ensure an alternative template is in place for any onboarding workflow that referenced the old one.

![Step 5 — Delete a permission template](img/mb-31-delete-template-confirm.png)
