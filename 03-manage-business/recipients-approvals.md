# recipients-approvals

_Summerville Admin Console › Manage Business › Recipients & Approvals_

## Manage Business: Recipients & Approval Settings

> The payee master list and the dual-control thresholds — together these are the first line of defense against BEC and payment fraud.

### Step-by-Step Workflow

#### Step 1: Business Recipients

The master list of external bank contacts authorized for ACH and wire payments, each tagged by recipient type and verification status. Treat this list as the business's authorized payee register — anything unverified or stale here is a fraud risk.

![Step 1: Business Recipients](../.gitbook/assets/mb-16-business-recipients.png)

#### Step 2: Recipient Detail

Click any row to see the full record: name, bank, masked routing and account numbers, recipient type, and verification status. Confirm all fields against the supporting documentation on file before marking a recipient as Verified — this step is the KYC checkpoint for outbound payment rails.

![Step 2: Recipient Detail](../.gitbook/assets/mb-17-recipient-detail.png)

#### Step 3: Approval Settings

Defines how many approvals each payment flow requires before release. Low-value ACH typically needs one; high-value ACH, wires, and ACH collections should require two or more — this is the dual-control configuration that your BSA/AML program depends on for business payments.

![Step 3: Approval Settings](../.gitbook/assets/mb-18-approval-settings.png)

### Summary

Recipients is the authorized payee register — it controls who the business can pay and validates the bank details on file. Approval Settings is the dual-control framework — it controls how many people must sign off before any payment goes out. Together these two surfaces represent the primary operational controls against business email compromise and unauthorized payment initiation for commercial members.

### Key Use Cases

* Phishing attempt reported on a business account: audit the recipient list for unrecognized payees, remove stale entries, and raise high-value ACH and wire approval counts to two or more.
* Quarterly KYC review on commercial relationships: verify each recipient row against supporting documentation, confirm verified status is current before the next payment cycle.
