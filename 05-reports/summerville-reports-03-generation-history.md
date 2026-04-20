_Summerville Admin Console  ›  Reports  ›  Generation & History_

# Reports — Generation & History (ACH, E-Notice, SRT)

> Point-in-time extract jobs and the historical ACH, E-Notice, and SRT archives.

## Step-by-Step Workflow

### Step 1 — Generate New Report

Report Type dropdown — Transactions-All, Statistics-Feature-Usage, audit variants. Asynchronous: run shows up on Scheduled, then Generated.

![Step 1 — Generate New Report](img/rp-08-generate-new-report.jpg)

### Step 2 — View Scheduled Reports

Recurring and queued extract jobs. Empty state renders No scheduled reports to show. First page to check when a downstream file is missing.

![Step 2 — View Scheduled Reports](img/rp-09-view-scheduled.jpg)

### Step 3 — View Generated Reports

Historical record — Report Name, Channel, Status, Date Generated, Start / End, Size, Action. Sortable, filterable, four-tab duration.

![Step 3 — View Generated Reports](img/rp-10a-generated-default.jpg)

### Step 4 — View ACH Reports

Every ACH origination batch the channel produced. Empty windows render No ACH reports — absence on a business day is itself the signal.

![Step 4 — View ACH Reports](img/rp-11a-ach-default.jpg)

### Step 5 — View E-Notice Reports

Electronic notices — statements, NSF, Reg-E / Reg-DD via digital channel. Pair with Notification Reports for delivery diagnostics.

![Step 5 — View E-Notice Reports](img/rp-12a-enotice-default.jpg)

### Step 6 — View SRT Reports

Service Request Tickets raised through digital channel. Operational analogue of the CRM case list, near-real time.

![Step 6 — View SRT Reports](img/rp-13a-srt-default.jpg)

## Summary

Generation stands up extract jobs; Scheduled queues them; Generated is the history. ACH / E-Notice / SRT are three specialised archives, same duration chassis.

## Key Use Cases

- Examiner asks for Transactions-All over three weeks → View Generated, sort Date Generated, filter Report Name, export.
- "ACH file didn't originate" ticket → View ACH Reports, scope window, look for the absence.
- Monthly Statistics-Feature-Usage → Generate New Report, watch Scheduled, pick up from Generated when done.
