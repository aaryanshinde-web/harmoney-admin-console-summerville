# Business Entitlements

_Summerville Admin Console › Manage Members › Business Entitlements_

## Manage Members: Business Entitlements

> For commercial signers: the permissions they hold and the dollar limits that cap what they can move.

### Step-by-Step Workflow

#### Step 1: Business Entitlements

This is the fourth blue pill tab on the profile, and it only appears for members associated with a business relationship. Open it and use the Select business dropdown to scope the view — members who administer multiple businesses will have a separate permissions and limits set for each one.

![Step 1: Business Entitlements](../.gitbook/assets/mm-23-business-entitlements-dropdown.png)

#### Step 2: Business Permissions

Select a business to load its permission tree. Each leaf node is a specific capability — View Transfer, Access Bill Pay, Initiate ACH, and so on. The search bar lets you jump directly to a specific permission when you're diagnosing why a user can or can't perform a particular action.

![Step 2: Business Permissions](../.gitbook/assets/mm-24-business-permissions.png)

#### Step 3: Business Limits

Shows the count and dollar caps that apply to this member for the selected business — per-transaction, daily, and monthly, broken out by payment flow such as ACH collection, payroll template, and wire. Compare these against the business-level limits to identify which cap is binding when a payment gets declined.

![Step 3: Business Limits](../.gitbook/assets/mm-25-business-limits.png)

### Summary

Business Entitlements is a commercial-only section that surfaces per-business permissions and limits for any member who manages a business relationship. Permissions shows the capability tree — what the member is authorized to do. Limits shows the dollar and frequency ceilings on each flow. This is where nine out of ten "my user can't do X" support tickets get resolved without needing to escalate to operations.

### Key Use Cases

* Compliance audit on a commercial signer's access: open Business Permissions, search the tree for the specific authorization in question, screenshot for the audit file.
* Business owner's payroll ACH was declined: check Business Limits, read the Max Per Transaction and Daily cap for payroll template, compare against the attempted amount.
