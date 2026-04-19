_Summerville Admin Console  ›  Manage Content  ›  Reference Data_

# Manage Content — Rates, Static Content & File Exchange

> Publish dashboard rate tiles, manage member-identifier tokenisation, maintain fixed in-app copy blocks, and run secure bank-to-member document drops.

## Summary

Rates, Static Content & File Exchange groups four Manage Content sub-surfaces that publish reference content to the member experience. Rates stages the deposit, loan, and mortgage rate tiles that render on the member-facing dashboard. Tokenize Individual Id manages how member identifiers are tokenised as they move between the console, the mobile and online channels, and downstream fraud systems.

Static Content is where Marketing and Compliance co-own the fixed in-app copy blocks — help text, footer copy, enrolment prompts, module-level explainer text — so microcopy is reviewed and versioned in one place rather than scattered across engineering tickets. File Exchange is the secure bank-to-member document-drop workspace for KYC refresh packets, tax forms, and large wire confirmations — the channel Summerville controls end to end rather than losing custody over email.

## Key Use Cases

Treasury publishes a new paper rate sheet and needs the digital dashboard to match. The content operator opens Rates, updates the tiles, and the member-facing dashboard re-renders on the next load without an engineering release.

A commercial relationship manager needs to send a set of year-end trust forms and an annual loan review packet to a customer. The operator opens File Exchange, creates an outbound drop, and hands the secure link to the customer — the drop is audited and gated to the authenticated session rather than sitting in an inbox.

Compliance reviews all in-app help text at quarter end and updates the enrolment prompts that render inside the member experience. The operator opens Static Content, replaces the outdated copy, and the new microcopy is live on the next member session.

## End-to-End Workflow

### Prerequisites

- Manage Content role assigned to the operator via Manage Administrators (separate roles for Marketing, Compliance, and Content Operations where the bank has chosen to split duties).
- Approved marketing creative (1000x1296 banner image), approved legal document (PDF for Terms and Conditions), or approved broadcast copy for Notifications, reviewed and signed off outside the console.
- For scheduled content: a confirmed effective date or send timestamp in Pacific Standard Time, aligned with the regulatory, campaign, or operations calendar.
- For audience targeting: content-segmentation Groups already provisioned via Add Group so the operator can scope a banner or notification to the intended audience.

### Step-by-Step Flow

#### Step 1 — Open Rates to manage the public rate tiles

From Manage Content, click Rates to land on the rate publisher. This is the surface where the deposit, loan, and mortgage rate tiles that render on the member-facing dashboard are staged and published, and it is where the content operator synchronises the digital rate display with the paper rate sheet published by Treasury.

![Step 1 — Open Rates to manage the public rate tiles](img/mc-03-rates.jpg)

#### Step 2 — Open Tokenize Individual Id for identity-tokenisation configuration

From Manage Content, click Tokenize Individual Id to land on the tokenisation controls. This surface manages how member identifiers are tokenised when they travel between the console, the mobile and online channels, and downstream fraud systems — a control that matters both for PCI posture and for preventing identifier leakage into third-party analytics.

![Step 2 — Open Tokenize Individual Id for identity-tokenisation configuration](img/mc-04-tokenize-individual-id.jpg)

#### Step 3 — Open Static Content to maintain fixed in-app copy

From Manage Content, click Static Content to maintain the fixed copy blocks that render inside the member experience — help text, footer copy, enrolment prompts, module-level explainer text. This is the surface Marketing and Compliance co-own so that every piece of in-app microcopy is reviewed and versioned in one place rather than scattered across engineering tickets.

![Step 3 — Open Static Content to maintain fixed in-app copy](img/mc-05-static-content.jpg)

#### Step 4 — Open File Exchange for secure bank-to-member document transfer

From Manage Content, click File Exchange to land on the secure-drop workspace. This is the channel Summerville uses to send sensitive documents to a commercial customer — KYC refresh packets, tax forms, large wire confirmations — inside an authenticated session the credit union controls, rather than over email where Summerville loses custody the moment the message leaves its perimeter.

![Step 4 — Open File Exchange for secure bank-to-member document transfer](img/mc-06-file-exchange.jpg)
