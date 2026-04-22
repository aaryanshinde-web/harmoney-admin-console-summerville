# User Roles

_Summerville Admin Console › Manage Business › User Roles_

## Manage Business: User Roles

> The segregation-of-duties layer — each role gets exactly the permissions and dollar caps its function requires, nothing more.

### Step-by-Step Workflow

#### Step 1: User Roles

All roles configured on this business appear as cards: View-only, Basic Role, Business Admin, and any client-specific roles created for this entity. This is your overview of how the business has structured its internal access before you make any changes.

![Step 1: User Roles](../.gitbook/assets/mb-10-user-roles-panel.png)

#### Step 2: Role Permissions

Dual-pane Available / Included editor scoped to a single role. Enable only the capabilities this role's function requires — a payroll processor needs ACH initiation but not wire release, and that distinction matters for BSA/AML compliance.

![Step 2: Role Permissions](../.gitbook/assets/mb-11-role-permissions-edit.png)

#### Step 3: Role Limits

Dollar cap per payment feature inside this role, bounded by the entity-level Business Limits above it. Role limits can be equal to or lower than business limits — they can never exceed them.

![Step 3: Role Limits](../.gitbook/assets/mb-12-role-limits-amounts.png)

#### Step 4: Limit Frequency

Each dollar amount carries a frequency dimension: Max Per Transaction, Max Daily, and Max Monthly. Stack all three for layered defense — a role with a high per-transaction limit but a low daily cap is a meaningful fraud control.

![Step 4: Limit Frequency](../.gitbook/assets/mb-13-role-limits-frequency.png)

#### Step 5: Role Information

The role name and a one-line description that explains its intended function — for example, "Payroll — handles payroll file builds" or "AP Clerk — vendor ACH only." Write these clearly because they're what an auditor reads six months later when reviewing segregation of duties.

![Step 5: Role Information](../.gitbook/assets/mb-14-role-information.png)

#### Step 6: Select Template Role(s)

Seed the role from the central Role Templates catalogue — Payroll, Business Admin, Basic Role, or View-only — then trim and adjust from there. Starting from a template ensures the baseline permissions align with the credit union's standard service tiers before any client-specific customization.

![Step 6: Select Template Role(s)](../.gitbook/assets/mb-15-select-template-role.png)

### Summary

User Roles is the segregation-of-duties control layer for the business. Permissions defines what each role can initiate; Limits and Limit Frequency define the dollar and frequency ceilings on each action. Seeding from a template gives you a compliant baseline, and the Role Information description field is what makes the access model readable and auditable months after it was configured.

### Key Use Cases

* Payroll controller should build ACH files but not release wires: start from the Payroll template, confirm ACH initiation is Included, verify wire release is not, set frequency caps on all three dimensions.
* AP clerk restricted to vendor ACH only: start from Basic Role template, trim to ACH sub-features only, stack per-transaction, daily, and monthly caps to limit exposure.
