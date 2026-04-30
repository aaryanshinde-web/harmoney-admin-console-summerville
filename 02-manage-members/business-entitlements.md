# Business Entitlements

_Manage Members › Member Search › Search Results › Member Profile › Business Permissions_

## Manage Members: Business Entitlements

> Business Entitlements shows a member's per-business permissions and limits directly on the member profile. Use it to answer "why can't this user do X" without leaving the profile.

### Step-by-Step Workflow

#### Step 1: Open the Business Entitlements Tab

This is the fourth blue pill tab on a member's profile, and it only appears for members associated with a business. Open it and use the **Select business** dropdown to scope the view — members who administer multiple businesses have a separate permissions and limits set for each one.

![Step 1: Open the Business Entitlements Tab](../.gitbook/assets/mm-23-business-entitlements-dropdown.png)

#### Step 2: Business Permissions

Pick a business from the dropdown to load its permission tree. Each leaf is a specific capability — View Transfer, Access Bill Pay, Initiate ACH, and so on. The search bar lets you jump directly to a specific permission when you're diagnosing why a user can or can't perform a particular action.

![Step 2: Business Permissions](../.gitbook/assets/mm-24-business-permissions.png)

#### Step 3: Business Limits

The dollar caps that apply to this member through the business — per-transaction, daily, and monthly, broken out by ACH collection, payroll template, wire, and so on. Compare these against the Business Limits to see which cap is binding when a payment is declined.

![Step 3: Business Limits](../.gitbook/assets/mm-25-business-limits.png)

### Summary

Business Entitlements surfaces a member's per-business permissions and limits directly on the member profile. It's the fastest read on what a commercial signer is authorized to do and where their dollar caps sit. Most "my user can't do X" support tickets are resolved here.

### Key Use Cases

* Member calls saying their payroll ACH was declined: open Business Entitlements → Business Limits, check the Max Per Transaction and Daily caps for payroll template against the attempted amount.
* Member's wire-release button is missing: open Business Entitlements → Business Permissions, search the tree for the wire-release capability and confirm whether it's enabled for the member.
