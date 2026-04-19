_Summerville Admin Console  ›  Reports  ›  Transaction & Notification_

# Reports — Transaction & Notification

> Tabulate what members are actually doing by transaction type and how every alert is being delivered across SMS, email, and push channels.

## Summary

Transaction Reports and Notification Reports are the two Reports surfaces that answer the what-are-members-actually-doing and is-the-delivery-working questions. Transaction Reports exposes a Transaction Type dropdown that ranges from lightweight interactions (ATM search around a nearby area) to every money-movement type the channel supports, scoped to the chosen duration.

Notification Reports tabulates each Alert Type — New Device Remembered, Failed Login Attempt, and the rest — against the number of setups, SMS sent, emails sent, and push notifications sent in the window. Sortable columns and a Grand Total row make the report readable by non-analysts and turn a delivery complaint into a five-second diagnostic rather than a ticket to the platform team.

## Key Use Cases

Treasury and Risk ask the which-transaction-types-do-our-commercial-members-actually-run question ahead of a product-pricing review. The analyst opens Transaction Reports, walks the Transaction Type dropdown against the Last 90 Days view, and hands back the distribution without a SQL query.

A commercial client reports they did not get notified of a failed login. The operator opens Notification Reports, scopes the duration to the affected window, and reads the SMS / email / push count for Failed Login Attempt — seeing in seconds whether the event fired and which delivery channel was attempted.

## End-to-End Workflow

### Prerequisites

- Admin account entitled to the Reports module — typically granted to Treasury operations, Finance analytics, Risk and Compliance, and the commercial line-of-business leads.
- A specific operational question in mind (dashboard, board pack, audit response, incident investigation), because the question dictates which of the thirteen reports to open and which duration window to use.
- An evidence home-base for the output — a shared drive, an audit ticket, or a board folder — so the extract does not get stranded on a single analyst's screen.
- For Custom Duration queries: start and end dates that are inside the retention window for the chosen report, with the start date preceding the end date.

### Step-by-Step Flow

#### Step 1 — Open Transaction Reports

Transaction Reports exposes a Transaction Type dropdown — starting with lightweight interactions like ATM search around a nearby area and cascading into every money-movement type the channel supports — and scopes the count to the chosen duration. This is the surface Treasury and Risk use to answer which transaction types commercial members actually run, without a SQL query. Empty windows surface a No data to show notice.

![Step 1 — Open Transaction Reports](img/rp-06a-transaction-default.jpg)

#### Step 2 — Open Notification Reports

Notification Reports tabulates each Alert Type — New Device Remembered, Failed Login Attempt, and the rest — against the number of setups, SMS sent, emails sent, and push notifications sent in the window. This is the surface that closes an I didn't get notified ticket: the operator can see in seconds whether the event fired, which channel was attempted, and whether the attempt succeeded. Sortable columns and a Grand Total row make the report readable by non-analysts.

![Step 2 — Open Notification Reports](img/rp-07a-notification-default.jpg)
