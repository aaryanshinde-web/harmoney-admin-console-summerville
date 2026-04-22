_Summerville Admin Console › Manage Content › Notifications_

# Manage Content: Notifications & System Downtime

> Two broadcast surfaces: Notifications for member-facing messaging across Push, SMS, and Email, and System Downtime for pre-outage advisories with their own approval path.

## Step-by-Step Workflow

### Step 1: Notifications

The outbound broadcast register showing all Push, SMS, and Email messages. Used by Marketing for member reminders and by Treasury Ops for payment-window advisories — the channel scope and scheduling options make this flexible enough for both use cases.

![Step 1: Notifications](img/mc-11-notifications.jpg)

### Step 2: Add Notification

Title field accepts up to 50 words; Notification Text up to 300 words. Select the Delivery Channels — Push, SMS, Email, or any combination. Set Schedule to Immediate for send-now broadcasts when a time-sensitive operational message needs to go out without delay.

![Step 2: Add Notification](img/mc-12-notifications-add.jpg)

### Step 3: Schedule - One time, On

Toggle Schedule to One time, On to expose the PST timestamp picker. This is the right pattern for reminders or advisories that need to land at a precise moment — a payment window reminder at 10 AM PST Monday, for example, should be scheduled here rather than sent immediately.

![Step 3: Schedule - One time, On](img/mc-13-notifications-scheduled.jpg)

### Step 4: System Downtime Notification

A dedicated broadcast type for planned outages: core conversions, wire-cut windows, and mobile release events. It's intentionally separated from general Notifications because system downtime advisories carry different tone requirements and typically need a separate approval before going out to members.

![Step 4: System Downtime Notification](img/mc-14-system-downtime.jpg)

## Summary

Notifications handles routine member-facing messaging across all three digital channels with flexible scheduling. System Downtime is a distinct surface for outage advisories, separated to enforce a different review and approval process appropriate for operationally sensitive communications. Using the wrong surface for system downtime messages bypasses the approval controls that exist for a compliance reason.

## Key Use Cases

- Enrolment reminder that needs to land at 10 AM PST Monday: set Schedule to One time, On, select Push and Email, pick the exact timestamp.
- Saturday core conversion window: create a System Downtime notification, draft it at least 72 hours ahead to allow time for the separate approval process before it goes out.
