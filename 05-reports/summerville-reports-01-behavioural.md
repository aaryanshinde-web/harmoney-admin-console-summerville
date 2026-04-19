_Summerville Admin Console  ›  Reports  ›  Behavioural_

# Reports — Behavioural Reports

> Measure logins, active users, enrolments, usage mix, and member-submitted feedback across Last 7 / 30 / 90 Day and Custom Duration windows.

## Summary

Behavioural Reports are the six Reports surfaces that measure how the commercial digital channel is actually being used — User Report, Usage Report, Login Trend, Enrollment Trend, the shared Custom Duration picker, and the Feedback Report. Together they answer the Treasury P&L question of who is logging in, what they are doing, whether they are signing up, and what they are telling the credit union about the experience.

Every behavioural report shares the four-tab duration selector — Last 7 Days, Last 30 Days, Last 90 Days, Custom Duration — and Custom Duration is the only tab that changes the surface by exposing Select Start Date and Select End Date pickers alongside a Go button. The picker is identical across every report in the module, so the analyst learns it once and reuses it everywhere.

## Key Use Cases

The Treasury operations lead starts every week with a five-minute review of Login Trend, User Report, and Enrollment Trend on the Last 7 Days view — looking for three signals: did logins hold week-over-week, is the failed-login percentage within normal range, and did new enrolments keep pace with the commercial onboarding pipeline.

Ahead of the quarterly board meeting, the head of Commercial Digital opens each behavioural report on the Last 90 Days window, prints the charts, and consolidates them into the digital-channel section of the board pack.

The customer-experience team pairs the Feedback Report with Login Trend on a weekly VOC review — which is the cheapest early-warning system Summerville has against commercial-book attrition.

## End-to-End Workflow

### Prerequisites

- Admin account entitled to the Reports module — typically granted to Treasury operations, Finance analytics, Risk and Compliance, and the commercial line-of-business leads.
- A specific operational question in mind (dashboard, board pack, audit response, incident investigation), because the question dictates which of the thirteen reports to open and which duration window to use.
- An evidence home-base for the output — a shared drive, an audit ticket, or a board folder — so the extract does not get stranded on a single analyst's screen.
- For Custom Duration queries: start and end dates that are inside the retention window for the chosen report, with the start date preceding the end date.

### Step-by-Step Flow

#### Step 1 — Open the User Report

User Report is the first entry in the Reports navigator and answers the Treasury P&L question of who is actually logging in. The page combines a Membership Type, User Status, and Channel filter with a Number of Users chart and a Total Number of Active Users counter broken down by channel. A Print and an Export button in the top-right turn the view into an evidence artefact for the board pack or the incident file.

![Step 1 — Open the User Report](img/rp-01a-user-report-default.jpg)

#### Step 2 — Open the Usage Report

Usage Report pivots the same chassis from users to transactions, showing a Number of Transactions line chart, a Total Number of Transactions counter, and an Actions-by-Type Sankey that decomposes each transaction into its feature (Balance, Bill Pay Login, Bulk Fund Transfer, Cheque Deposited, Member Account History) and channel (Online, Mobile, Voice). For a commercial credit union, this is the single best surface to evidence which digital features the book is actually consuming.

![Step 2 — Open the Usage Report](img/rp-02a-usage-report-default.jpg)

#### Step 3 — Open Login Trend

Login Trend charts the number of logins against the failed-login percentage, so the security and the experience teams read the same surface and agree on whether any spike is adoption or attack. The page is explicitly labelled Pacific Standard Time because login events are logged server-side, which matters when an incident timeline crosses a day boundary. Four duration tabs — 7, 30, 90, Custom — scope the same chart without leaving the page.

![Step 3 — Open Login Trend](img/rp-03a-login-trend-default.jpg)

#### Step 4 — Open Enrollment Trend

Enrollment Trend charts new enrolments and unenrolments over the selected window, which is the cleanest leading indicator of commercial channel growth the digital team owns. A bright yellow No detailed data to show banner appears when the window is quiet, which is a deliberate nudge that low enrolment days should be noticed rather than glossed over.

![Step 4 — Open Enrollment Trend](img/rp-04a-enrollment-trend-default.jpg)

#### Step 5 — Use the Custom Duration picker

Every behavioural and transactional report shares the four-tab duration selector — Last 7 Days, Last 30 Days, Last 90 Days, Custom Duration — and Custom Duration is the only tab that changes the surface by exposing Select Start Date and Select End Date pickers alongside a Go button. The date picker is identical across every report in the module, so learn it once and reuse it everywhere for examiner, incident, or bespoke windows.

![Step 5 — Use the Custom Duration picker](img/rp-04d-enrollment-trend-custom.jpg)

#### Step 6 — Open the Feedback Report

Feedback Report consolidates the in-app satisfaction signal members submit, rolled up over the chosen window. Quiet days render a soft No feedback data to show notice, and live days render the captured sentiment alongside the volume — exactly the surface the customer-experience lead needs for a Monday VOC review. Pairing this report with Login Trend is the cheapest early-warning system Summerville has against commercial-book attrition.

![Step 6 — Open the Feedback Report](img/rp-05a-feedback-default.jpg)
