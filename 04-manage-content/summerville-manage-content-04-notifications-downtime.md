_Summerville Admin Console  ›  Manage Content  ›  Notifications_

# Manage Content — Notifications & System Downtime

> Compose and schedule Push / SMS / E-mail broadcasts, and draft the planned-outage advisory that runs ahead of a core-banking conversion or wire-cutoff change.

## Summary

Notifications & System Downtime are the two Manage Content surfaces Summerville uses to talk to its members about the platform. Notifications is the outbound-broadcast register for Push, SMS, and E-mail — used by Marketing for reminder campaigns and by Treasury Operations for payment-window advisories. Title has a 50-word limit and Notification Text a 300-word limit; Schedule toggles Immediate versus One time, On with a PST timestamp picker.

System Downtime Notification is deliberately separated from the general Notifications register because planned-outage advisories have a different approval path and a different severity tone than marketing broadcasts. It is the surface Treasury Operations uses to draft the advisory that runs ahead of a core conversion, a wire-cut change, or a mobile-app release window.

## Key Use Cases

Marketing wants to push an enrolment reminder to inactive members at a specific hour on a specific day. The operator opens Notifications, sets Schedule to One time, On, picks the PST timestamp, and leaves Push, SMS, and E-mail all checked — the right default for commercial members who may live across more than one delivery channel.

The core-banking team has scheduled a Saturday-evening conversion window during which wire and ACH cut-offs will be unavailable. Treasury Operations opens System Downtime Notification, drafts the advisory, and schedules it to publish 72 hours before the window so commercial customers can plan their payment batches.

## End-to-End Workflow

### Prerequisites

- Manage Content role assigned to the operator via Manage Administrators (separate roles for Marketing, Compliance, and Content Operations where the bank has chosen to split duties).
- Approved marketing creative (1000x1296 banner image), approved legal document (PDF for Terms and Conditions), or approved broadcast copy for Notifications, reviewed and signed off outside the console.
- For scheduled content: a confirmed effective date or send timestamp in Pacific Standard Time, aligned with the regulatory, campaign, or operations calendar.
- For audience targeting: content-segmentation Groups already provisioned via Add Group so the operator can scope a banner or notification to the intended audience.

### Step-by-Step Flow

#### Step 1 — Open Notifications to manage outbound broadcasts

From Manage Content, click Notifications to land on the outbound-broadcast register. This is the surface where push, SMS, and e-mail broadcasts are drafted, scheduled, and published — the same place Marketing uses for reminder campaigns and the same place Treasury Operations uses for payment-window advisories, which is exactly why its governance matters.

![Step 1 — Open Notifications to manage outbound broadcasts](img/mc-11-notifications.jpg)

#### Step 2 — Open Add Notification and capture the broadcast payload

Click Add Notification to open the form. Capture Title (50 word limit) and Notification Text (300 word limit), leave Schedule on Immediate for a send-now broadcast, and pick the Delivery Channel mix from Push Notification, SMS, and E-mail — in practice you want all three checked for treasury advisories and only Push plus E-mail for marketing reminders.

![Step 2 — Open Add Notification and capture the broadcast payload](img/mc-12-notifications-add.jpg)

#### Step 3 — Toggle Schedule to One time, On and set the send timestamp

Toggle Schedule from Immediate to One time, On — the form reveals a PST timestamp picker. This is the correct pattern for any broadcast that must land at a specific moment, such as a reminder that goes out at 10 AM PST on the Monday before a payroll cut-off, or a Treasury advisory that drops exactly 24 hours before a wire-cut window change.

![Step 3 — Toggle Schedule to One time, On and set the send timestamp](img/mc-13-notifications-scheduled.jpg)

#### Step 4 — Open System Downtime Notification to draft a planned-outage advisory

From Manage Content, click System Downtime Notification to draft the advisory that runs ahead of a planned outage — a core conversion, a wire-cut change, a mobile-app release window. This surface is deliberately separated from the general Notifications register because planned-outage advisories have a different approval path and a different severity tone than marketing broadcasts.

![Step 4 — Open System Downtime Notification to draft a planned-outage advisory](img/mc-14-system-downtime.jpg)
