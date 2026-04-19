_Summerville Admin Console  ›  Manage Members  ›  Accounts & Activity_

# Manage Members — Accounts & Activity

> Walk the member's financial surface area — Accounts, Alerts, Transactions, Activity log, and All Recipients — during a dispute, fraud claim, or entitlement question.

## Summary

Accounts & Activity is the financial-surface-area view on the member profile. Six sub-panels — Accounts, Alerts, Transactions, Feature Enrollment, Scheduled Transfers, and All Recipients — give the operator a complete picture of the member's money-movement footprint from a single authenticated session.

The surface is built for dispute and fraud investigation. Transactions carries Last 7 / 30 / 90 / Custom duration chips and an Activity log dropdown that narrows the ledger to a specific event like Balance check, Zelle Login, or a Bill Pay flow. All Recipients exposes the saved payee master list scoped by Membership, and each recipient opens a verification drawer that shows every receiving account and its verified / unverified status.

## Key Use Cases

A member disputes a bill-pay transfer. The CSR expands Transactions, filters Last 30 Days, narrows Activity log to Bill Pay Login Enhanced, and exports the matching row for the Reg-E investigation file — which is what the examiner will ask for later.

A member complains they never received an alert on a large wire. The operator opens Alerts to see the blackout window and the channels the member enabled, then drops into the Sent Alerts ledger underneath to show the exact delivery per channel at the disputed timestamp.

A commercial signer questions why a payment has not cleared to the receiving FI. The operator opens All Recipients, filters by Membership to scope to the business, opens the recipient detail drawer, and shows each receiving account's verified / unverified status — the fastest way to explain the rail the payment took.

## End-to-End Workflow

### Prerequisites

- Admin login with Manage Members access; the member must be a verified enrollment (pre-enrolled identities live under Pre-Enrolled Block rather than Manage Members).
- Ticket number, call reference, or alert ID to capture in the Admin Comment on every sensitive action — a blank comment is treated as a control failure.
- For dispute or fraud investigations: the disputed transaction date and time window agreed with the member so Transactions and Session Details can be scoped precisely.
- For business-member entitlement review: the specific business the signer administers, so the Business Permissions and Business Limits panels can be loaded against the correct entity.

### Step-by-Step Flow

#### Step 1 — Open Accounts and Activity for the financial surface area

Accounts and Activity is the financial-surface-area view. Six sub-panels — Accounts, Alerts, Transactions, Feature Enrollment, Scheduled Transfers, and All Recipients — give the operator a complete picture of the member's money-movement footprint.

![Step 1 — Open Accounts and Activity for the financial surface area](img/mm-13-accounts-activity-dropdown.png)

#### Step 2 — Review alert configuration and delivery

Alerts shows the blackout window, the channels the member has enabled, and every configured alert with its trigger. The Sent Alerts ledger underneath is gold during an I never got notified call — it shows the exact delivery per channel with timestamps.

![Step 2 — Review alert configuration and delivery](img/mm-14-alerts-notifications.png)

#### Step 3 — Pull transaction history with the timeframe chips

Transactions shows the member's activity across accounts with quick Last 7 / 30 / 90 Days buttons and a Custom Duration picker. The rooted-device toggle is worth knowing — it filters to sessions where the device reported jailbreak or root, which is what the operator wants when triaging a fraud claim.

![Step 3 — Pull transaction history with the timeframe chips](img/mm-15-transactions.png)

#### Step 4 — Slice the ledger by Activity log type

The Activity log dropdown is the widest enum in the module — it lets the operator narrow the ledger to a specific action like Balance check, Zelle Login, or a Bill Pay flow. Combine it with a tight date range when confirming a single disputed event.

![Step 4 — Slice the ledger by Activity log type](img/mm-16-activity-log-dropdown.png)

#### Step 5 — Inspect saved recipients on All Recipients

All Recipients is the list of every payee the member has saved across rails — internal, ACH, wire, bill pay. The Membership filter scopes the list to a specific business the member administers, which is how the operator proves out a commercial entitlement question.

![Step 5 — Inspect saved recipients on All Recipients](img/mm-17-all-recipients.png)

#### Step 6 — Open a recipient for verification details

Click a recipient name to open a verification drawer. It shows each receiving account and its verified / unverified status — the fastest way to explain why a payment has not cleared to the receiving FI yet.

![Step 6 — Open a recipient for verification details](img/mm-18-recipient-detail-modal.png)
