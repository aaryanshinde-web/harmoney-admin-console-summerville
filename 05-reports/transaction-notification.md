_Summerville Admin Console › Reports › Transaction & Notification_

# Reports: Transaction & Notification

> What members are doing financially and whether their alerts are reaching them — two questions that close most operational support tickets without SQL.

## Step-by-Step Workflow

### Step 1: Transaction Reports

A Transaction Type dropdown that spans from lightweight interactions like ATM search all the way through every money-movement flow. Scope it to a duration window and you have a complete picture of transaction activity for that period — useful for pricing reviews, dispute pattern analysis, and volume reporting.

![Step 1: Transaction Reports](img/rp-06a-transaction-default.jpg)

### Step 2: Notification Reports

Each Alert Type shown against setup count, SMS delivery count, email delivery count, and push delivery count, with sortable columns and a Grand Total row. This is where you go when a member says they didn't receive an alert — scope the window, find the alert type, and read the delivery counts to see whether the issue is channel-specific or broader.

![Step 2: Notification Reports](img/rp-07a-notification-default.jpg)

## Summary

Transaction Reports and Notification Reports answer the two most common operational questions without requiring a database query: what did members do, and did they get notified about it. Transaction Reports covers the full payment activity spectrum by type and window. Notification Reports covers alert delivery by channel, making it the first stop for any "I didn't receive my alert" complaint.

## Key Use Cases

- Pricing review for a new fee structure: walk the Transaction Type dropdown on Last 90 Days, export the distribution, hand it to the product and finance teams.
- Member files a complaint about a missed fraud alert: Notification Reports, scope to the relevant window, read the Failed Login Attempt row to check whether the alert was sent and to which channels.
