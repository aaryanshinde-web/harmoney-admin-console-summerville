_Summerville Admin Console › Manage Content › Reference Data_

# Manage Content: Rates, Static Content & File Exchange

> Four surfaces for publishing reference content to members — rate tiles, identifier tokenisation, fixed in-app copy, and secure file delivery.

## Step-by-Step Workflow

### Step 1: Rates

Deposit, loan, and mortgage rate tiles that render on the member-facing dashboard. Stage the new rates here and publish to synchronize with Treasury's paper rate sheet — the dashboard re-renders on the member's next load, so there's no delay between publishing and visibility.

![Step 1: Rates](img/mc-03-rates.jpg)

### Step 2: Tokenize Individual Id

Controls how member identifiers are tokenised between the console, digital channels, and fraud systems. This configuration matters for PCI posture and for preventing analytics leakage across integration boundaries — changes here should be reviewed with your compliance and security teams before being made.

![Step 2: Tokenize Individual Id](img/mc-04-tokenize-individual-id.jpg)

### Step 3: Static Content

Fixed in-app copy that appears across the member experience: help text, footer content, enrolment prompts, and feature explainers. Marketing and Compliance co-own this section and can update it here directly, bypassing the engineering ticket queue for routine copy changes.

![Step 3: Static Content](img/mc-05-static-content.jpg)

### Step 4: File Exchange

A secure, session-authenticated workspace for delivering files to specific members — KYC packets, tax forms, wire confirmations, and similar documents. Files are delivered inside an authenticated session, so Summerville maintains custody and the delivery is auditable.

![Step 4: File Exchange](img/mc-06-file-exchange.jpg)

## Summary

Four distinct content surfaces, each serving a different operational function: Rates keeps member-facing pricing current, Tokenize Individual Id governs compliance-sensitive identifier handling, Static Content lets non-engineering teams manage in-app copy, and File Exchange provides a secure and auditable channel for document delivery to individual members.

## Key Use Cases

- Treasury publishes a new rate sheet: update Rates in the console, the dashboard tiles re-render on next member load with no code change required.
- Year-end trust documents need to go to a specific client: File Exchange drop inside an authenticated session, delivery is logged and auditable.
- Quarterly compliance copy review: update Static Content directly, changes go live at the member's next session without an engineering release.
