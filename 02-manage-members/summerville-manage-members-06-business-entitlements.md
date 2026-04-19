_Summerville Admin Console  ›  Manage Members  ›  Business Entitlements_

# Manage Members — Business Entitlements

> For commercial members: review the Business Permissions feature tree and the Business Limits count / dollar caps per business the member administers.

## Summary

Business Entitlements is the commercial-only pill on the member profile. It has two sub-panels — Business Permissions and Business Limits — that together describe exactly what the member can do on each business they administer, indexed by the Select business dropdown at the top of the panel.

Business Permissions is a searchable feature tree of every capability granted on the selected business; Business Limits is the count and dollar ceiling per flow (ACH collection, payroll template, wire, and so on). When a commercial signer pushes back on a declined transfer, this is the two-screen surface that shows whether the limit was daily, per-transaction, or per-month, and whether the missing capability is an un-ticked permission or an approval queue.

## Key Use Cases

Internal audit needs to confirm that a business signer still has only the payment-approval permissions their board authorised. The auditor opens Business Permissions, picks the business, and uses the search bar at the top of the feature tree to jump to the specific authorisations — the entitlement snapshot lines up with what the examiner expects to see.

A controller reports that a declined payroll transfer was inside their documented authority. The operator opens Business Limits, picks the business, and reads the Max Per Transaction / Max Daily / Max Monthly row for Run payroll template to identify whether the binding constraint was daily or monthly velocity.

## End-to-End Workflow

### Prerequisites

- Admin login with Manage Members access; the member must be a verified enrollment (pre-enrolled identities live under Pre-Enrolled Block rather than Manage Members).
- Ticket number, call reference, or alert ID to capture in the Admin Comment on every sensitive action — a blank comment is treated as a control failure.
- For dispute or fraud investigations: the disputed transaction date and time window agreed with the member so Transactions and Session Details can be scoped precisely.
- For business-member entitlement review: the specific business the signer administers, so the Business Permissions and Business Limits panels can be loaded against the correct entity.

### Step-by-Step Flow

#### Step 1 — Expand the Business Entitlements dropdown

The fourth pill is the one commercial members care about. Business Entitlements has two sub-panels — Business Permissions and Business Limits — that together describe exactly what the member can do on each business they administer.

![Step 1 — Expand the Business Entitlements dropdown](img/mm-23-business-entitlements-dropdown.png)

#### Step 2 — Review the feature tree on Business Permissions

Pick a business from the Select business dropdown to load the feature tree. Each leaf is a capability — View Transfer Information, Access/View Bill Pay, View Scheduled Transfer History — and the search bar at the top of the tree lets the operator jump straight to a feature when confirming a specific authorisation.

![Step 2 — Review the feature tree on Business Permissions](img/mm-24-business-permissions.png)

#### Step 3 — Confirm money-movement caps on Business Limits

Business Limits is the count and dollar caps per flow — ACH collection, payroll template, wire, and so on. When a business member pushes back on a declined transfer, this is the page that shows whether the limit was daily, per-transaction, or per-month.

![Step 3 — Confirm money-movement caps on Business Limits](img/mm-25-business-limits.png)
