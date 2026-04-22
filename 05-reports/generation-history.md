_Summerville Admin Console › Reports › Generation & History_

# Reports: Generation & History (ACH, E-Notice, SRT)

> Asynchronous extract jobs and the historical archives for ACH batches, electronic notices, and service request tickets.

## Step-by-Step Workflow

### Step 1: Generate New Report

Select a Report Type from the dropdown — Transactions-All, Statistics-Feature-Usage, and audit variants are available. Report generation is asynchronous: after you submit, the job moves to Scheduled while it processes, then to Generated when it's ready for download.

![Step 1: Generate New Report](img/rp-08-generate-new-report.jpg)

### Step 2: View Scheduled Reports

Recurring and queued extract jobs waiting to run. An empty state shows "No scheduled reports to show" — if you're expecting a downstream file and it hasn't arrived, check here first to confirm the job is queued and hasn't been accidentally removed.

![Step 2: View Scheduled Reports](img/rp-09-view-scheduled.jpg)

### Step 3: View Generated Reports

The historical record of completed extracts: Report Name, Channel, Status, Date Generated, Start, End, Size, and Action. Sortable and filterable across four duration tabs — use this when an examiner or operations team asks for a specific export from a past window.

![Step 3: View Generated Reports](img/rp-10a-generated-default.jpg)

### Step 4: View ACH Reports

Every ACH origination batch produced by the digital channel, scoped by duration. An empty window showing "No ACH reports" on a business day is itself a signal — if your commercial clients should have originated ACH that day and the archive is empty, that's worth investigating before end of day.

![Step 4: View ACH Reports](img/rp-11a-ach-default.jpg)

### Step 5: View E-Notice Reports

Electronic notices delivered through the digital channel: statements, NSF notices, Reg-E and Reg-DD disclosures. Pair with Notification Reports when diagnosing whether a member received both their notice and the alert about it.

![Step 5: View E-Notice Reports](img/rp-12a-enotice-default.jpg)

### Step 6: View SRT Reports

Service Request Tickets raised through the digital channel, near-real time. This is the operational analogue of your CRM case list for digital-channel requests — use it when you need to see what members are requesting through self-service without waiting for a CRM export.

![Step 6: View SRT Reports](img/rp-13a-srt-default.jpg)

## Summary

Generation creates the extract jobs; Scheduled shows you what's queued; Generated is the downloadable history. ACH, E-Notice, and SRT are three specialized archives on the same duration chassis — each covering a distinct regulatory and operational record type. The absence of expected records in any of these archives is as significant as the presence of them.

## Key Use Cases

- Examiner requests Transactions-All for a three-week window: View Generated, sort by Date Generated, filter by Report Name, export the matching file.
- Commercial client reports an ACH file didn't originate on a given day: View ACH Reports, scope to that date, look for the absence of the expected batch.
- Monthly Statistics-Feature-Usage extract for the product team: Generate New Report, monitor Scheduled until it moves to Generated, download from the Generated tab.
