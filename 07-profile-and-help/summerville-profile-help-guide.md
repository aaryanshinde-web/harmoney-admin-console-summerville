*Summerville Admin Console › Edit My Profile & Help Docs*

# Edit My Profile & Help Docs

*Maintain your administrator identity record, review your personal
operations footprint, rotate your password, and reach feature
documentation without leaving the admin console.*

## Summary

Edit My Profile and Help Docs are the two personal surfaces in the
Summerville Admin Console — the surfaces every administrator interacts
with every day, regardless of which business-banking module they spend
the rest of their time in. Edit My Profile is where the signed-in
administrator maintains their own identity record, reviews the list of
operations they personally executed, and rotates their password on the
bank's published cadence. Help Docs is the contextual help entry point
that routes the administrator to the feature documentation maintained by
the Product and Content teams, without context-switching to a separate
support portal.

The Edit My Profile workspace is organised around three tabs — My
Profile, My Operations, and Change Password. The design intent is
deliberately narrow: an administrator can see their own record and
rotate their own password, but they cannot edit their own Role or E-Mail
Id, because in a commercial-banking environment self-service changes to
either field would create a segregation-of-duties problem. Those fields
are governed by Manage Administrators under the Information Security
Officer's control.

## Key Use Cases

A newly provisioned Treasury Operations analyst opens Edit My Profile on
their first login to confirm that HR, Identity, and the ISO have
captured them correctly — verifying First Name, Last Name, E-Mail Id,
Username, and Role on the My Profile tab and using the single Edit
button to add the Mobile number, which is the only field the platform
lets them self-maintain.

During the quarterly access review, each administrator attests to their
personal activity on the platform. They open My Operations, pick the
relevant operation from the Choose operation dropdown, set Start Date
and End Date to cover the review window, and run the search — the
returned rows are their personal slice of the Admin Activity log and
become the evidence they sign off on.

On the bank's 90-day rotation cadence the administrator opens Change
Password, enters a New Password and Confirm Password that satisfy the
published Password Requirements (8-25 characters with at least one
numeric, one lowercase, and one uppercase alphabet), and submits. The
Password Requirements panel is rendered alongside the form so the
administrator does not guess the policy and does not loop on rejected
submissions.

A content operator mid-stage on a new Terms and Conditions version
clicks Help Docs in the left-hand navigator to look up the difference
between Forced and Optional acknowledgement — returning to Manage
Content without losing their place. In-console documentation is the kind
of friction removal that matters most on a Friday afternoon when a
change has to go live before the weekend.

## End-to-End Workflow

## Prerequisites

  - A provisioned admin-console user account with valid Username and
    current password.

  - The administrator is signed in to the Summerville admin console in
    the current browser session.

  - For My Operations: at least one completed operation exists in the
    admin activity history for the signed-in user.

  - For Change Password: the current password is known (a forgotten
    password is recovered through Manage Administrators, not
    self-service).

## Step-by-Step Flow

## Step 1: Open Edit My Profile and review the My Profile tab

From the left-hand navigator, click Edit My Profile to land on the My
Profile tab. The tab surfaces the administrator's First Name, Last Name,
E-Mail Id, Username, Mobile, and Role alongside the Enrolled Since
timestamp — the only place in the console where an administrator can see
their canonical identity record, and the only tab with an Edit button to
self-maintain the Mobile field.

![Step 1 — My Profile tab](img/ep-01-my-profile.jpg)

## Step 2: Switch to My Operations and run a date-bounded search

Click the My Operations tab to open the personal-activity workspace.
Pick an operation from the Choose operation dropdown (for example
Enrollment Block Member), set Start Date and End Date to define the
window, and click Search. The return set is the administrator's personal
footprint on the platform for the selected operation type — the correct
evidence when an administrator is asked to attest to their own activity
during a control review.

![Step 2 — My Operations tab](img/ep-02-my-operations.jpg)

**Step 3: Open Change Password, enter a compliant new password, and
submit**

Click the Change Password tab to open the password-rotation form. Enter
New Password and Confirm Password — each field has a Show toggle to
verify what was typed — and cross-check the Password Requirements panel
beside the form (8-25 characters, at least one numeric, one lowercase,
and one uppercase alphabet). Submit to rotate; the platform rejects any
submission that fails the published policy so there is no
guess-and-retry loop.

![Step 3 — Change Password tab](img/ep-03-change-password.jpg)

## Step 4: Use Help Docs for contextual, in-console documentation

From the bottom of the left-hand navigator, click Help Docs to open the
feature documentation that the Product and Content teams maintain for
the admin console. Help Docs is deliberately a link-out surface rather
than an editable module — its value is where it lives, inside the same
console the administrator was already working in, so that a quick
documentation lookup never requires a context switch to a separate
support portal.

*Help Docs does not expose editable content inside the admin console and
therefore does not have a dedicated screenshot in this guide. Its
governance sits with the Product and Content teams, and the
admin-console entry point routes the signed-in administrator to the
bank's published documentation system so that the full history of
feature changes and release notes travels with the console rather than
being maintained separately.*

