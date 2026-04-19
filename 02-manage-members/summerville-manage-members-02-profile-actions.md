_Summerville Admin Console  ›  Manage Members  ›  Profile Actions_

# Manage Members — Profile Actions

> Run the seven safeguard actions on a member profile — Reset Password, Block, Lock, Unenroll, Manage Channels, Sync Contact Details, and Update Info New.

## Summary

Profile Actions are the seven safeguard levers that live above the member profile — Reset Password, Block Member, Lock Member, Unenroll Member, Manage Channels, Sync Contact Details, and Update Info New. Each one opens a modal rather than committing immediately, and each one captures an Admin Comment so the action is defensible on Support History.

The actions are deliberately segmented by intent. Reset is for authentication recovery. Block is the post-enrollment safeguard that stops the member from transacting but keeps the enrollment record. Lock is the fast-acting login freeze for suspected fraud. Unenroll is the full digital-profile removal at account closure. Manage Channels toggles Online / Mobile / Voice at the channel level. Sync and Update Info New reconcile contact details between the core and the digital profile.

## Key Use Cases

A business owner cannot get into online banking before a 9 AM payroll run. The CSR pulls up the member, picks Generate Temporary Password, reads a one-time password to the caller, and logs an admin comment — the member is unblocked in minutes and the audit trail captures why.

Transaction monitoring flags unusual wire activity on a commercial member. The risk analyst presses Lock Member with a comment referencing the alert ID to freeze login in a single click while investigation runs; once cleared, the same page unlocks them and the sequence appears on Support History.

A member has updated their phone and email at the branch but the digital profile still shows the old values. The operator runs Sync Contact Details to pull the refreshed values from the core, or uses Update Info New for a side-by-side Bank Core / nFinia compare so no field the member updated online is accidentally overwritten.

## End-to-End Workflow

### Prerequisites

- Admin login with Manage Members access; the member must be a verified enrollment (pre-enrolled identities live under Pre-Enrolled Block rather than Manage Members).
- Ticket number, call reference, or alert ID to capture in the Admin Comment on every sensitive action — a blank comment is treated as a control failure.
- For dispute or fraud investigations: the disputed transaction date and time window agreed with the member so Transactions and Session Details can be scoped precisely.
- For business-member entitlement review: the specific business the signer administers, so the Business Permissions and Business Limits panels can be loaded against the correct entity.

### Step-by-Step Flow

#### Step 1 — Confirm you have the right person on the Member Profile landing

Clicking the User ID drops the operator into the member profile. Always read the name badge, the status pill (Active / Locked / Blocked), and the Individual ID before acting — a wrong-member action is the most common operational incident in this module.

![Step 1 — Confirm you have the right person on the Member Profile landing](img/mm-03-member-profile.png)

#### Step 2 — Run a Reset Password with the correct delivery channel

Click Reset Password and pick one of three delivery channels — Email reset link, SMS temporary password, or Generate Temporary Password when the member is already on the phone. Add the ticket number in Admin Comment and press Reset Password to commit; the entry lands on Support History immediately.

![Step 2 — Run a Reset Password with the correct delivery channel](img/mm-04-reset-password-modal.png)

#### Step 3 — Use Block Member as the post-enrollment safeguard

Block Member stops a member from completing digital actions while keeping the enrollment record intact — the right choice when the member is still a valid customer but must be stopped from transacting pending a review. The admin comment is mandatory so the next CSR sees why the block was applied.

![Step 3 — Use Block Member as the post-enrollment safeguard](img/mm-05-block-member-modal.png)

#### Step 4 — Use Lock Member as the fast-acting login freeze

Lock Member is the right call during a suspected-fraud conversation — lock first, investigate second. The lock is reversible from Manage Members > Locked Members once the case is cleared, so the blast radius is small and the audit trail is clean.

![Step 4 — Use Lock Member as the fast-acting login freeze](img/mm-06-lock-member-modal.png)

#### Step 5 — Unenroll a member at account closure

Unenroll removes the digital-banking enrollment completely; the member can still bank through the branch and the core, but every saved recipient, alert, and scheduled transfer is gone. Use this when the underlying account is closing or the member is moving FIs.

![Step 5 — Unenroll a member at account closure](img/mm-07-unenroll-modal.png)

#### Step 6 — Toggle channels with Manage Channels

Manage Channels is the quickest way to disable a compromised channel while leaving the rest of the member's access intact. The checkboxes are pre-populated with the current state, so tick Voice off if a voice-banking PIN has been socially engineered, save, and move on.

![Step 6 — Toggle channels with Manage Channels](img/mm-08-manage-channels-modal.png)

#### Step 7 — Sync phone and email from the core

Use Sync Contact Details when a member has updated their phone or email at the branch but the digital profile still shows the old values. The modal also exposes the Enabled-for-voice flag per number, which matters when voice-banking is being provisioned for the first time.

![Step 7 — Sync phone and email from the core](img/mm-10-sync-contact-modal.png)

#### Step 8 — Compare Bank Core and nFinia fields via Update Info New

Update Info New opens a side-by-side compare of Bank Core and nFinia contact fields. Tick only the rows to push to digital so the operator does not accidentally overwrite a field the member updated online.

![Step 8 — Compare Bank Core and nFinia fields via Update Info New](img/mm-09-update-info-modal.png)
