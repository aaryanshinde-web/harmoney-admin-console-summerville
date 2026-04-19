_Summerville Admin Console  ›  Reports  ›  Generation & History_

# Reports — Generation & History (ACH, E-Notice, SRT)

> Stand up point-in-time extract jobs, govern the scheduled queue, and retrieve the historical ACH, E-Notice, and SRT report archives an examiner expects.

## Summary

Generation & History is the operational micro-workflow Reports offers for point-in-time extracts and historical archives. Generate New Report launches an asynchronous extract job (Transactions-All, Statistics-Feature-Usage, and audit-file variants), View Scheduled Reports lists the recurring and queued jobs the team has stood up, and View Generated Reports is the historical record with Report Name, Channel, Status, Date Generated, Start and End Date, and Size — sortable and filterable per column.

View ACH Reports, View E-Notice Reports, and View SRT Reports are the three specialised history surfaces for cash-management, electronic-notice, and service-request-ticket archives respectively. Each follows the same duration-scoped table shape, and each renders a soft no-data-to-show notice on empty windows — which matters because, for a commercial credit union, the absence of an ACH batch on a business day is itself the signal.

## Key Use Cases

An examiner asks for every Transactions-All file produced over a three-week window. The analyst opens View Generated Reports, sorts by Date Generated, filters by Report Name, and exports the matching rows — which is the audit artefact the examiner will pick up.

A business reports that an ACH file did not originate. The analyst opens View ACH Reports, scopes the duration to the affected window, and looks for the absence — pairing that with Notification Reports and Transaction Reports narrows the root cause to either the origination engine or the notification engine without paging the platform team.

The monthly data-warehouse feed needs a new Statistics-Feature-Usage extract. The operator opens Generate New Report, picks the type, submits, and then confirms the job on View Scheduled Reports and later on View Generated Reports when it completes.

## End-to-End Workflow

### Prerequisites

- Admin account entitled to the Reports module — typically granted to Treasury operations, Finance analytics, Risk and Compliance, and the commercial line-of-business leads.
- A specific operational question in mind (dashboard, board pack, audit response, incident investigation), because the question dictates which of the thirteen reports to open and which duration window to use.
- An evidence home-base for the output — a shared drive, an audit ticket, or a board folder — so the extract does not get stranded on a single analyst's screen.
- For Custom Duration queries: start and end dates that are inside the retention window for the chosen report, with the start date preceding the end date.

### Step-by-Step Flow

#### Step 1 — Generate a new report

Generate New Report opens a single Report Type dropdown that launches a point-in-time extract job — the common ones in Summerville's portfolio are Transactions-All, Statistics-Feature-Usage, and the audit-file variants. Use this surface for examiner requests, for the monthly data-warehouse feed, or for any extract that will not fit into a live dashboard. Generation is asynchronous: once a type is submitted, the run shows up on View Scheduled Reports and then on View Generated Reports when it completes.

![Step 1 — Generate a new report](img/rp-08-generate-new-report.jpg)

#### Step 2 — View Scheduled Reports

Scheduled Reports lists the recurring and queued extract jobs the team has stood up — a soft No scheduled reports to show notice renders when the queue is empty. For a commercial credit union, this is the page operations checks first whenever a downstream team complains that a file didn't arrive, because a missing schedule here is always the root cause before delivery-side issues are examined.

![Step 2 — View Scheduled Reports](img/rp-09-view-scheduled.jpg)

#### Step 3 — View Generated Reports

Generated Reports is the historical record of every extract the module has produced — Report Name, Channel, Status, Date Generated, Report Start Date, Report End Date, Size, and an Action column. The list is sortable on every column and filterable via Search-within-Results, which is how an auditor asks for the Transactions-All files produced between two dates without leaving the console. The four-tab duration selector scopes the list itself.

![Step 3 — View Generated Reports](img/rp-10a-generated-default.jpg)

#### Step 4 — View ACH Reports

ACH Reports is where the cash-management and NACHA-audit surfaces live — every ACH origination batch the channel has produced, scoped by the duration tabs. Empty windows render a No ACH reports to show notice, which matters because the absence of ACH batches on a business day is itself the signal — either the business users didn't initiate, or the origination path is broken. This is the first page to open during any ACH origination incident.

![Step 4 — View ACH Reports](img/rp-11a-ach-default.jpg)

#### Step 5 — View E-Notice Reports

E-Notice Reports tabulates the electronic notices the channel has dispatched — account statements, insufficient-funds notices, and any Reg-E or Reg-DD communications that moved via the digital channel. A soft No E-Notice reports to show notice guards against misreading an empty window, which is important because commercial clients generally consume these notices via e-mail or in-app delivery rather than paper. Combine with Notification Reports to diagnose delivery complaints.

![Step 5 — View E-Notice Reports](img/rp-12a-enotice-default.jpg)

#### Step 6 — View SRT Reports

SRT Reports — Service Request Ticket reports — lists the member-originated service requests that have flowed through the digital channel over the chosen window. For a commercial book, this is the operational analogue of the CRM case list: it tells the operator what business members are asking Summerville to fix, in near-real time, without waiting for the CRM extract. Like the other history surfaces, empty windows render a soft No SRT reports to show notice.

![Step 6 — View SRT Reports](img/rp-13a-srt-default.jpg)
