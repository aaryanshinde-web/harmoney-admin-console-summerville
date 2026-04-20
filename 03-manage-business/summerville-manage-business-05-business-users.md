_Summerville Admin Console  ›  Manage Business  ›  Business Users_

# Manage Business — Business Users

> Diagnose what one commercial user can and can't do — applied permissions and limits.

## Step-by-Step Workflow

### Step 1 — Business User Detail

Every employee of the business who can log in, with their assigned role. Click a user to see inherited entitlements.

![Step 1 — Business User Detail](img/mb-19-business-user-detail.png)

### Step 2 — Role Permissions

Every feature flag the role carries — Bill Pay, Scheduled Transfers, Recipients, Wires, ACH, Manage Transfers and Payments.

![Step 2 — Role Permissions](img/mb-20-role-permissions-modal.png)

### Step 3 — Role Permissions (expanded)

Full hierarchy beneath Manage Transfers and Payments. Same tree the end user sees on their dashboard.

![Step 3 — Role Permissions (expanded)](img/mb-21-role-permissions-expanded.png)

### Step 4 — Role Limits

Dollar ceilings per flow — ACH collections, payroll template, domestic wire. Compare against Business Limits.

![Step 4 — Role Limits](img/mb-22-role-limits-modal.png)

## Summary

Business Users is the diagnostic surface for "X cannot do Y" tickets. Permissions modal shows the feature tree, Limits modal shows the caps — nine times out of ten a missing capability is visible here.

## Key Use Cases

- Controller can't release wires → Role Permissions > Manage Transfers and Payments, check wire-release leaf.
- Payment rejected on limit → compare Role Limits vs Business Limits to find the binding cap.
