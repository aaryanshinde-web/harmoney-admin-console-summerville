_Summerville Admin Console  ›  Manage Members  ›  Devices & Login_

# Manage Members — Devices & Login

> Pull the device ledger, drill into a device fingerprint, walk successful-login history, and download the per-session transaction log for Reg-E investigations.

## Summary

Devices & Login is the forensic surface on the member profile — the panel that a fraud or Reg-E investigator opens first on a session-hijack claim. Access Devices is the grid of every browser and mobile device the member has signed in from, with Remembered flags showing which ones the member has trusted.

Login Details is the companion surface for successful-login events, with IP, user-agent, and a Session link per row. Session Information opens a modal that lists every transaction that ran inside one login — authentication, balance check, Bill Pay Login Enhanced, Zelle Login — and exposes a Download button that saves the full session as evidence for a Reg-E investigation.

## Key Use Cases

A member claims a wire was initiated from a device they do not recognise. The investigator opens Access Devices, identifies the unfamiliar device, clicks View Information, and copies the Device ID into the fraud case so it can be correlated with other alerts on the same fingerprint.

Regulation E requires documented evidence of the exact session a disputed transfer ran in. The operator opens Login Details, scopes the date chip to the disputed day, opens Session Information on the matching row, and downloads the full session to the case file — which is the evidence format the examiner expects.

## End-to-End Workflow

### Prerequisites

- Admin login with Manage Members access; the member must be a verified enrollment (pre-enrolled identities live under Pre-Enrolled Block rather than Manage Members).
- Ticket number, call reference, or alert ID to capture in the Admin Comment on every sensitive action — a blank comment is treated as a control failure.
- For dispute or fraud investigations: the disputed transaction date and time window agreed with the member so Transactions and Session Details can be scoped precisely.
- For business-member entitlement review: the specific business the signer administers, so the Business Permissions and Business Limits panels can be loaded against the correct entity.

### Step-by-Step Flow

#### Step 1 — Pull the device ledger under Devices and Login

Access Devices is a grid of every browser and mobile device the member has signed in from, with Remembered flags showing which ones are trusted. This is the first page to open on a session-hijack claim.

![Step 1 — Pull the device ledger under Devices and Login](img/mm-19-access-devices.png)

#### Step 2 — Drill into a single device fingerprint

View Information on any row opens the full device fingerprint — Device ID, Type, OS, OS version, first-seen. Copy the Device ID into the fraud case so the investigator can correlate it with other alerts.

![Step 2 — Drill into a single device fingerprint](img/mm-20-device-information-modal.png)

#### Step 3 — Switch to Login Details for the successful-login ledger

Login Details is the successful-login ledger with IP, user-agent, and a Session link per row. Use the date-range chips to scope quickly, then click Session Information on the row under investigation.

![Step 3 — Switch to Login Details for the successful-login ledger](img/mm-21-login-details.png)

#### Step 4 — Download the per-session transaction log

Session Details lists every transaction that ran inside one login — authentication, balance check, Bill Pay Login Enhanced, Zelle Login, and so on. Download saves the full session as evidence, which is what a Reg-E investigation requires.

![Step 4 — Download the per-session transaction log](img/mm-22-session-details-modal.png)
