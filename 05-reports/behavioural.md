_Summerville Admin Console › Reports › Behavioural_

# Reports: Behavioural Reports

> Six behavioural surfaces on one duration chassis — who logged in, what they did, whether they enrolled, and what they said about it.

## Step-by-Step Workflow

### Step 1: User Report

Shows who is actively logging in, filterable by Membership Type, User Status, and Channel. The Number of Users chart and Active Users counter give you the headline metrics — use Print or Export when this data is going into a board pack or regulatory response.

![Step 1: User Report](img/rp-01a-user-report-default.jpg)

### Step 2: Usage Report

Transaction volume broken out by feature and channel (Online, Mobile, Voice), with an Actions-by-Type Sankey diagram. This is the report that answers what members are actually doing in the platform — useful for pricing reviews and for identifying underutilized features that might need member education.

![Step 2: Usage Report](img/rp-02a-usage-report-default.jpg)

### Step 3: Login Trend

Logins vs. failed-login percentage plotted over time, stamped in Pacific Standard Time. The PST labelling matters when you're reconstructing an incident timeline that crosses a calendar day boundary — a spike in failed logins at 11:55 PM PST is a different event than one at 12:05 AM PST.

![Step 3: Login Trend](img/rp-03a-login-trend-default.jpg)

### Step 4: Enrollment Trend

New enrolments and unenrolments over the selected window. A yellow "No detailed data to show" banner appears on low-activity days — don't skip past quiet windows, because unexpectedly low enrolment on a campaign day is itself a signal worth investigating.

![Step 4: Enrollment Trend](img/rp-04a-enrollment-trend-default.jpg)

### Step 5: Custom Duration

Four duration tabs: Last 7 Days, 30 Days, 90 Days, and Custom. Custom exposes Select Start Date, Select End Date, and Go — use this for any reporting window that doesn't align to a standard chip, such as a fiscal quarter or an exam period.

![Step 5: Custom Duration](img/rp-04d-enrollment-trend-custom.jpg)

### Step 6: Feedback Report

In-app satisfaction scores aggregated by duration window. Paired with Login Trend, this is the earliest available signal for member attrition — a declining satisfaction score alongside a rising failed-login rate is a combination that warrants an immediate product review.

![Step 6: Feedback Report](img/rp-05a-feedback-default.jpg)

## Summary

The six Behavioural Reports share a single duration chassis and together tell the complete story of member engagement: access patterns, feature utilization, enrolment health, and satisfaction. Running them together on a consistent cadence — weekly for operations, quarterly for the board — gives Summerville a reliable baseline against which anomalies become visible.

## Key Use Cases

- Monday morning ops stand-up: run Login Trend, User Report, and Enrollment Trend on Last 7 Days for the week-over-week snapshot.
- Quarterly board reporting package: run each report on Last 90 Days, export, consolidate into the board deck.
- Weekly voice-of-the-customer review: Feedback Report paired with Login Trend — declining satisfaction alongside rising failed logins is an early attrition signal.
