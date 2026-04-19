_Summerville Admin Console  ›  Manage Administrators_

# Manage Administrators

> Provision admin console operators, scope their role-based access, and review the audit footprint every privileged action leaves behind.

## Summary

Manage Administrators is the internal-governance module of the Summerville Admin Console — the place where Summerville Credit Union maintains the roster of people who themselves operate the digital-banking platform. Where Manage Members defines who banks with Summerville and Manage Business defines how those commercial entities are structured, Manage Administrators defines who at Summerville is allowed to log in to the console itself, what they can see and do once they are in, and what footprint they leave behind when they act on a member's account.

The module is deliberately small and auditable. The left-hand navigator exposes two surfaces: Manage Admin Users for provisioning and role assignment, and Admin Activity for the corresponding audit trail. This mirrors how a credit union's Information Security Officer actually thinks about privileged access — one screen for who-has-what-rights, one screen for what-did-they-do-with-those-rights — and keeps the concerns separated so they can be governed by different owners and reviewed on different cadences. The combination of role-based provisioning plus an immutable date-filtered activity log is what lets the CISO demonstrate to FFIEC and NCUA examiners that privileged access is scoped, justified, and reviewable.

## Key Use Cases

When Treasury Operations hires a new analyst who needs console access to approve ACH batches and release wires, the ISO opens Manage Admin Users, clicks Add New Admin User, captures Title, Email, Mobile, and User ID, and assigns a Role scoped to Treasury-Ops approvals only. The Role assignment is the governance boundary — it ensures the new analyst can see only the surfaces they need, and the audit trail in Admin Activity starts capturing their footprint from the moment they first log in.

Each quarter the ISO attests that every administrator on the platform still has a legitimate business need for the access they hold. The ISO opens Manage Admin Users, searches the roster by Name or User ID, and walks each record against HR's active-employee list and the business unit's sign-off — anyone who has moved teams or left the credit union is removed, and the Admin Activity log provides corroborating evidence of recent use for the accounts that remain.

When an examiner or internal audit requests a log of administrator actions over a specific window — a common ask during a BSA or cybersecurity exam — the ISO opens Admin Activity, fills in Start Date and End Date for the window in question, and runs the search. The date-bounded result is the auditable extract: reproducible on demand, scoped precisely to the examiner's window, and eliminates the manual database query many institutions still rely on for this evidence.

When Risk or the SOC flags a suspicious configuration change — a role reassignment, a member record edit, a rates update — the incident responder uses Admin Activity to pin the change to a specific administrator and a specific timestamp. Pairing that attribution with the Role in Manage Admin Users closes the forensics loop, tells the incident team whether the action was within scope for that Role, and feeds the formal incident write-up filed with the regulator.

## End-to-End Workflow

### Prerequisites

- A console login with ISO or administrator-of-administrators role (provisioning Admin Users requires elevated privilege).
- An access-matrix signed off by the requesting business unit that maps Roles to the surfaces each Role is permitted to reach.
- For Admin Activity extracts: the review window's Start Date and End Date agreed with the requester (examiner, internal audit, or incident team).
- For recertification walks: HR's current active-employee list for the cycle being reviewed.

### Step-by-Step Flow

#### Step 1 — Open Manage Admin Users

From the left-hand navigator under Manage Administrators, click Manage Admin Users to land on the roster page. The default view offers a User ID radio option, a search input, and a Search button — this is the primary lookup pattern for an administrator you already know by ID, and it is the fastest way to recertify a single named account during a quarterly review.

![Step 1 — Open Manage Admin Users](img/ma-01-admin-users-landing.jpg)

#### Step 2 — Switch the radio to Name for fuzzy lookup

If you do not have the User ID to hand, toggle the radio from User ID to Name; the form replaces the single User ID field with First Name and Last Name inputs. For an ISO doing a recertification walk-through against HR's active-employee list, searching by surname is almost always faster than hunting for the internal User ID, and it eliminates the lookup step that otherwise pulls the ISO into Active Directory.

![Step 2 — Switch the radio to Name for fuzzy lookup](img/ma-02-admin-users-by-name.jpg)

#### Step 3 — Provision a new administrator via Add New Admin User

From Manage Admin Users, click Add New Admin User to open the provisioning form. Capture Title and Description to record the business justification, then Email, User ID, and Mobile for the identity and second-factor channels, and finally Role for the access boundary — Role is the single most important field on this form and must map one-to-one with the access-matrix the ISO has signed off for the requesting business unit.

![Step 3 — Provision a new administrator via Add New Admin User](img/ma-03-add-new-admin-user.jpg)

#### Step 4 — Open Admin Activity and choose your review window

From the left-hand navigator, click Admin Activity to open the audit-log workspace. The two mandatory inputs are Start Date and End Date, which are there by design — every activity extract must be anchored to a specific window so it is reproducible for an examiner, a regulator, or an internal auditor, and so that no two reviewers accidentally work from different windows.

![Step 4 — Open Admin Activity and choose your review window](img/ma-04-admin-activity.jpg)

#### Step 5 — Understand why the Search button is date-gated

If you click Search without filling both date fields, the console returns inline validation — Please select start date and Please select end date — and blocks the query. This is the right default for a control surface: it forces every reviewer to scope their query explicitly, it prevents the accidental dump of the entire admin log, and it makes the resulting extract defensible when it lands on an examiner's desk.

![Step 5 — Understand why the Search button is date-gated](img/ma-05-admin-activity-validation.jpg)
